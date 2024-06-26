# Comparing `tmp/admanage-0.6.tar.gz` & `tmp/admanage-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admanage-0.6.tar", last modified: Sun May  5 15:20:03 2024, max compression
+gzip compressed data, was "admanage-0.7.tar", last modified: Sun May 12 16:52:25 2024, max compression
```

## Comparing `admanage-0.6.tar` & `admanage-0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.597107 admanage-0.6/
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.570706 admanage-0.6/ADmanage/
--rw-rw-rw-   0        0        0    12012 2024-04-12 09:20:05.000000 admanage-0.6/ADmanage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.595087 admanage-0.6/ADmanage.egg-info/
--rw-rw-rw-   0        0        0     7702 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7702 2024-05-05 15:20:03.596087 admanage-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7557 2024-05-05 15:14:58.000000 admanage-0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 15:20:03.597107 admanage-0.6/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-05-05 15:17:39.000000 admanage-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.467577 admanage-0.7/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.444335 admanage-0.7/ADmanage/
+-rw-rw-rw-   0        0        0    13798 2024-05-12 16:51:46.000000 admanage-0.7/ADmanage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.463881 admanage-0.7/ADmanage.egg-info/
+-rw-rw-rw-   0        0        0     7702 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7702 2024-05-12 16:52:25.467577 admanage-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7557 2024-05-12 16:50:02.000000 admanage-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:52:25.467577 admanage-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-05-12 16:50:49.000000 admanage-0.7/setup.py
```

### Comparing `admanage-0.6/ADmanage/__init__.py` & `admanage-0.7/ADmanage/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import ldap3
-from ldap3 import Server, Connection, ALL, SUBTREE, MODIFY_ADD, MODIFY_DELETE, MODIFY_REPLACE
+from ldap3 import Server, Connection, ALL, SUBTREE, MODIFY_ADD, MODIFY_DELETE, MODIFY_REPLACE, NTLM
 from impacket.structure import Structure
 import socket
 import dns.resolver
 import datetime
+import json
 
 class ADclient:
-    def __init__(self, domain, username, password, dc_ip, base_dn=None, secure=False):
+    def __init__(self, domain, username, password, hashes, dc_ip, base_dn=None, secure=False):
         self.domain = domain
         self.username = username
-        self.sam = f"{username}@{domain}"
-        self.password = password
+        self.sam = f"{domain}\\{username}"
+        self.password = password or hashes
         self.dc_ip = dc_ip
         self.base_dn = base_dn
         self.secure = secure
-        self.domainroot = f"DC={domain.split('.')[0]},DC={domain.split('.')[1]}"
-        self.dnsroot = f"DC={domain},CN=MicrosoftDNS,DC=DomainDnsZones,{self.domainroot}"
+        self.domain_root = f"DC={domain.split('.')[0]},DC={domain.split('.')[1]}"
+        self.dnsroot = f"DC={domain},CN=MicrosoftDNS,DC=DomainDnsZones,{self.domain_root}"
         self.conn = self.connect_to_ldap()
 
     def connect_to_ldap(self):
         dc_url = f"ldaps://{self.dc_ip}:636" if self.secure else f"ldap://{self.dc_ip}:389"
         if not self.base_dn:
-            self.base_dn = self.domainroot
+            self.base_dn = self.domain_root
 
         server = Server(dc_url, get_info=ALL)
-        conn = Connection(server, user=self.sam, password=self.password, auto_bind=True)
+        conn = Connection(server, user=self.sam, password=self.password, authentication=NTLM, auto_bind=True)
         return conn
 
     def disconnect(self):
         self.conn.unbind()
 
     class DNS_RECORD(Structure):
         """
@@ -104,36 +105,42 @@
         self.conn.search(search_base=self.dnsroot, search_filter=filter, attributes=['dnsRecord','dNSTombstoned','name'])
         for entry in self.conn.response:
             if entry['type'] != 'searchResEntry':
                 continue
             return entry
 
     def get_DNSentry(self, target):
+        if not self.get_raw_entry(target):
+            return "Entry doesn't exist"
+
         record_data = self.get_raw_entry(target)['raw_attributes']['dnsRecord'][0][-4:]
         parsed_record = self.DNS_RPC_RECORD_A(record_data)
         ip_address = parsed_record.formatCanonical()
         return {'name': self.get_raw_entry(target)['attributes']['name'], 'ip': ip_address}
 
     def add_DNSentry(self, target, data):
         record_dn = f'DC={target},{self.dnsroot}'
         node_data = {
             # Schema is in the root domain (take if from schemaNamingContext to be sure)
-            'objectCategory': f'CN=Dns-Node,CN=Schema,CN=Configuration,{self.domainroot}',
+            'objectCategory': f'CN=Dns-Node,CN=Schema,CN=Configuration,{self.domain_root}',
             'dNSTombstoned': False,
             'name': target
         }
         record = self.new_record(1)
         record['Data'] = self.DNS_RPC_RECORD_A()
         record['Data'].fromCanonical(data)
         node_data['dnsRecord'] = [record.getData()]
         self.conn.add(record_dn, ['top', 'dnsNode'], node_data)
         return self.get_DNSentry(target)
 
     def modify_DNSentry(self, target, data):
         targetentry = self.get_raw_entry(target)
+        if not targetentry:
+            return "Entry doesn't exist"
+
         records = []
         for record in targetentry['raw_attributes']['dnsRecord']:
             dr = self.DNS_RECORD(record)
             if dr['Type'] == 1:
                 targetrecord = dr
             else:
                 records.append(record)
@@ -142,14 +149,17 @@
         targetrecord['Data'].fromCanonical(data)
         records.append(targetrecord.getData())
         self.conn.modify(targetentry['dn'], {'dnsRecord': [(MODIFY_REPLACE, records)]})
         return self.get_DNSentry(target)
 
     def del_DNSentry(self, target):
         targetentry = self.get_raw_entry(target)
+        if not targetentry:
+            return "Entry doesn't exist"
+
         diff = datetime.datetime.today() - datetime.datetime(1601,1,1)
         tstime = int(diff.total_seconds()*10000)
         # Add a null record
         record = self.new_record(0)
         record['Data'] = self.DNS_RPC_RECORD_TS()
         record['Data']['entombedTime'] = tstime
         self.conn.modify(targetentry['dn'], {'dnsRecord': [(MODIFY_REPLACE, [record.getData()])],'dNSTombstoned': [(MODIFY_REPLACE, True)]})
@@ -158,26 +168,33 @@
     def get_ADobjects(self, custom_base_dn=None, custom_filter=None, custom_attributes=None):
         base_dn = custom_base_dn or self.base_dn
         search_filter = custom_filter or "(|(objectClass=user)(objectClass=group)(objectClass=computer))"
         attributes = custom_attributes or ['*']
         self.conn.search(base_dn, search_filter=search_filter,  attributes=attributes, search_scope=SUBTREE)
 
         if self.conn.entries:
-            return self.conn.entries
+            entries = [json.loads(entry.entry_to_json()) for entry in self.conn.entries]
+            for entry in entries:
+                entry['attributes'] = {key: str(value[0]) if isinstance(value, list) and len(value) == 1 else value for key, value in entry["attributes"].items()}
+            return [entry['attributes'] for entry in entries]
 
     # Search for user, group, or computer objects with sAMAccountName value
     def get_ADobject(self, _object):
         search_filter = f"(&(|(objectClass=user)(objectClass=group)(objectClass=computer))(sAMAccountName={_object}))"
         self.conn.search(self.base_dn, search_filter, attributes=['*'])
 
         if self.conn.entries:
-            return self.conn.entries[0]
+            entries = [json.loads(entry.entry_to_json()) for entry in self.conn.entries]
+            for entry in entries:
+                entry['attributes'] = {key: str(value[0]) if isinstance(value, list) and len(value) == 1 else value for key, value in entry["attributes"].items()}
+            return entries[0]['attributes']
 
     # Adding users, computers or groups
     def add_ADobject(self, ou, attributes):
+        attributes = json.loads(str(attributes).replace("'", "\""))
         if attributes['objectClass'] == 'user':
             sam = f"{attributes['givenName'].lower()[0]}{attributes['sn'].lower()}"
             cn = f"{attributes['givenName']} {attributes['sn']}"
 
             password = attributes['password']
             del attributes['password']
 
@@ -219,98 +236,120 @@
 
             self.conn.add(f"cn={cn},{ou}", attributes=attributes)
 
         return self.get_ADobject(sam)
 
     # Removing users, computers or groups
     def del_ADobject(self, _object):
-        _object_dn = self.get_ADobject(_object).distinguishedName
-        if self.conn.delete(_object_dn[0]):
-            return 200
-        else:
-            return None
+        if not self.get_ADobject(_object):
+            return "Object doesn't exist"
+
+        _object_dn = self.get_ADobject(_object)['distinguishedName']
+        self.conn.delete(_object_dn)
+
 
     # List members of group
     def get_member(self, group_name):
         search_filter = f"(&(objectClass=group)(sAMAccountName={group_name}))"
         self.conn.search(self.base_dn, search_filter, attributes=['member'])
 
         if self.conn.entries:
-            return self.conn.entries[0].member
+            return self.conn.entries[0].member.value
 
 
     # List groups of users
     def get_memberOf(self, username):
         search_filter = f"(&(objectClass=user)(sAMAccountName={username}))"
         self.conn.search(self.base_dn, search_filter, attributes=['memberOf'])
 
         if self.conn.entries:
-            return self.conn.entries[0].memberOf
+            return self.conn.entries[0].memberOf.value
 
 
     # Adding users, computers, or groups to groups
     def add_ADobject_to_group(self, _object, group):
-        _object_dn = self.get_ADobject(_object).distinguishedName
-        group_dn = self.get_ADobject(group).distinguishedName
+        if not self.get_ADobject(_object) or not self.get_ADobject(group):
+            return "Group, User or Computer doesn't exist"
 
-        self.conn.modify(group_dn[0], {'member': [(MODIFY_ADD, [_object_dn[0]])]})
+        _object_dn = self.get_ADobject(_object)['distinguishedName']
+        group_dn = self.get_ADobject(group)['distinguishedName']
 
-        return self.get_ADobject(group).member
+        self.conn.modify(group_dn, {'member': [(MODIFY_ADD, [_object_dn])]})
+
+        return self.get_ADobject(group)['member']
 
 
     # Removing users, computers, or groups from groups
     def del_ADobject_from_group(self, _object, group):
-        _object_dn = self.get_ADobject(_object).distinguishedName
-        group_dn = self.get_ADobject(group).distinguishedName
+        if not self.get_ADobject(_object) or not self.get_ADobject(group):
+            return "Group, User or Computer doesn't exist"
 
-        self.conn.modify(group_dn[0], {'member': [(MODIFY_DELETE, _object_dn[0])]})
+        _object_dn = self.get_ADobject(_object)['distinguishedName']
+        group_dn = self.get_ADobject(group)['distinguishedName']
 
-        return self.get_ADobject(group).member
+        self.conn.modify(group_dn, {'member': [(MODIFY_DELETE, _object_dn)]})
+        try:
+            return get_ADobject(group)['member']
+        except KeyError:
+            return None
 
     # Updating user, computer, or group attributes.
     def modify_ADobject_attributes(self, _object, attributes):
-        _object_dn = self.get_ADobject(_object).distinguishedName
+        attributes = json.loads(str(attributes).replace("'", "\""))
+        
+        if not self.get_ADobject(_object):
+            return "Object doesn't exist"
 
-        for key, value in attributes.items():
-            self.conn.modify(_object_dn[0], {key: [(MODIFY_REPLACE, [value])]})
+        _object_dn = self.get_ADobject(_object)['distinguishedName']
 
+        for key, value in attributes.items():
+            self.conn.modify(_object_dn, {key: [(MODIFY_REPLACE, [value])]})
         return self.get_ADobject(_object)
 
 
     # Reset password (Only work with ssl bind)
     def reset_password(self, username, password):
-        user_dn = self.get_ADobject(username).distinguishedName
+        if self.get_ADobject(username):
+            return "User doesn't exist"
+
+        user_dn = self.get_ADobject(username)['distinguishedName']
 
         if self.conn and self.secure:
-            if ldap3.extend.microsoft.modifyPassword.ad_modify_password(self.conn, user_dn[0], password, old_password=None):
+            if ldap3.extend.microsoft.modifyPassword.ad_modify_password(self.conn, user_dn, password, old_password=None):
                 return 200
             else:
                 return None
         else:
             return 401
 
 
     # Enable users or computers
     def enable_ADobject(self, _object):
+        if not self.get_ADobject(_object):
+            return "Object doesn't exist"
+
         uacFlag = 2
-        old_uac = self.get_ADobject(_object).userAccountControl
+        old_uac = self.get_ADobject(_object)['userAccountControl']
         new_uac = int(str(old_uac)) & ~uacFlag
 
         attributes = {
             'userAccountControl': new_uac
         }
 
         self.modify_ADobject_attributes(_object, attributes)
         return self.get_ADobject(_object)
 
 
     # Disable users or computers
     def disable_ADobject(self, _object):
+        if not self.get_ADobject(_object):
+            return "Object doesn't exist"
+
         uacFlag = 2
-        old_uac = self.get_ADobject(_object).userAccountControl
+        old_uac = self.get_ADobject(_object)['userAccountControl']
         new_uac = int(str(old_uac)) | uacFlag
 
         attributes = {
             'userAccountControl': new_uac
         }
 
         self.modify_ADobject_attributes(_object, attributes)
```

### Comparing `admanage-0.6/ADmanage.egg-info/PKG-INFO` & `admanage-0.7/ADmanage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADmanage
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 Requires-Dist: ldap3
 Requires-Dist: impacket
 
 # ADmanage
 
 The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
```

### Comparing `admanage-0.6/PKG-INFO` & `admanage-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADmanage
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 Requires-Dist: ldap3
 Requires-Dist: impacket
 
 # ADmanage
 
 The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
```

### Comparing `admanage-0.6/README.md` & `admanage-0.7/README.md`

 * *Files identical despite different names*

