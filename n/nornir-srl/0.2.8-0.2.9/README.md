# Comparing `tmp/nornir_srl-0.2.8.tar.gz` & `tmp/nornir_srl-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_srl-0.2.8.tar", max compression
+gzip compressed data, was "nornir_srl-0.2.9.tar", max compression
```

## Comparing `nornir_srl-0.2.8.tar` & `nornir_srl-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1492 2024-02-05 10:34:37.180268 nornir_srl-0.2.8/LICENSE
--rw-r--r--   0        0        0    25356 2024-02-05 10:34:37.180268 nornir_srl-0.2.8/README.md
--rw-r--r--   0        0        0       22 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/connections/__init__.py
--rw-r--r--   0        0        0     4568 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/connections/helpers.py
--rw-r--r--   0        0        0    35533 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/connections/srlinux.py
--rw-r--r--   0        0        0    25909 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/fsc.py
--rw-r--r--   0        0        0        0 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/tasks/__init__.py
--rw-r--r--   0        0        0      374 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/tasks/helpers.py
--rw-r--r--   0        0        0     9178 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/nornir_srl/tasks/srl_config.py
--rw-r--r--   0        0        0      869 2024-02-05 10:34:37.204268 nornir_srl-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    26427 1970-01-01 00:00:00.000000 nornir_srl-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1492 2024-03-12 22:31:13.554062 nornir_srl-0.2.9/LICENSE
+-rw-r--r--   0        0        0    25356 2024-03-12 22:31:13.554062 nornir_srl-0.2.9/README.md
+-rw-r--r--   0        0        0       22 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/connections/__init__.py
+-rw-r--r--   0        0        0     4568 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/connections/helpers.py
+-rw-r--r--   0        0        0    37190 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/connections/srlinux.py
+-rw-r--r--   0        0        0    25909 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/fsc.py
+-rw-r--r--   0        0        0        0 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/tasks/__init__.py
+-rw-r--r--   0        0        0      374 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/tasks/helpers.py
+-rw-r--r--   0        0        0     9178 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/nornir_srl/tasks/srl_config.py
+-rw-r--r--   0        0        0      869 2024-03-12 22:31:13.578062 nornir_srl-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    26427 1970-01-01 00:00:00.000000 nornir_srl-0.2.9/PKG-INFO
```

### Comparing `nornir_srl-0.2.8/LICENSE` & `nornir_srl-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.2.8/README.md` & `nornir_srl-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.2.8/nornir_srl/connections/helpers.py` & `nornir_srl-0.2.9/nornir_srl/connections/helpers.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.2.8/nornir_srl/connections/srlinux.py` & `nornir_srl-0.2.9/nornir_srl/connections/srlinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,34 @@
                     d["_r_state"] = (
                         ("u" if d["used-route"] else "")
                         + ("*" if d["valid-route"] else "")
                         + (">" if d["best-route"] else "")
                     )
                     if d.get("vni", 0) == 0:
                         d["vni"] = "-"
+                    d["_rt"] = ",".join(
+                        [
+                            x_comm.split("target:")[1]
+                            for x_comm in d.get("communities", {}).get(
+                                "ext-community", []
+                            )
+                            if "target:" in x_comm
+                        ]
+                    )
+                    d["_esi_lbl"] = ",".join(
+                        [
+                            str(x_comm.split("esi-label:")[1])
+                            .replace("Single-Active", "S-A")
+                            .replace("All-Active", "A-A")
+                            for x_comm in d.get("communities", {}).get(
+                                "ext-community", []
+                            )
+                            if "esi-label:" in x_comm
+                        ]
+                    )
                     return d
                 else:
                     return {k: augment_routes(v, attribs) for k, v in d.items()}
             else:
                 return d
 
         evpn_path_version = [
@@ -236,19 +256,19 @@
                 ),
                 "RIB_EVPN_JMESPATH_COMMON": '"network-instance"[].{NI:name, Rib:"bgp-rib"."'
                 + ROUTE_FAMILY[route_fam]
                 + '"."rib-in-out"."rib-in-post"."'
                 + ROUTE_TYPE[route_type]  # type: ignore
                 + '"[]',
                 "RIB_EVPN_JMESPATH_ATTRS": {
-                    "1": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, Tag:"ethernet-tag-id",vni:vni, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-                    "2": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "MAC":"mac-address", "IP":"ip-address",vni:vni,"next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-                    "3": '.{RD:"route-distinguisher", peer:neighbor, Tag:"ethernet-tag-id", "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-                    "4": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
-                    "5": '.{RD:"route-distinguisher", peer:neighbor, lpref:"local-pref", "IP-Pfx":"ip-prefix",vni:vni, med:med, "next-hop":"next-hop", GW:"gateway-ip",origin:origin, "0_st":"_r_state"}}',
+                    "1": '.{RD:"route-distinguisher", peer:neighbor, ESI:esi, Tag:"ethernet-tag-id",vni:vni, "NextHop":"next-hop", RT:"_rt", "esi-lbl":"_esi_lbl", "0_st":"_r_state"}}',
+                    "2": '.{RD:"route-distinguisher", RT:"_rt", peer:neighbor, ESI:esi, "MAC":"mac-address", "IP":"ip-address",vni:vni,"next-hop":"next-hop", "0_st":"_r_state"}}',
+                    "3": '.{RD:"route-distinguisher", RT:"_rt", peer:neighbor, Tag:"ethernet-tag-id", "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "4": '.{RD:"route-distinguisher", RT:"_rt", peer:neighbor, ESI:esi, "next-hop":"next-hop", origin:origin, "0_st":"_r_state"}}',
+                    "5": '.{RD:"route-distinguisher", RT:"_rt", peer:neighbor, lpref:"local-pref", "IP-Pfx":"ip-prefix",vni:vni, med:med, "next-hop":"next-hop", GW:"gateway-ip",origin:origin, "0_st":"_r_state"}}',
                 },
             },
         }
         RIB_IP_PATH_VERSIONS = {
             1: {
                 "RIB_IP_PATH": (
                     f"/network-instance[name={network_instance}]/bgp-rib/"
@@ -264,15 +284,15 @@
                     f"/network-instance[name={network_instance}]/bgp-rib/afi-safi[afi-safi-name={ROUTE_FAMILY[route_fam]}]/"
                     f"{ROUTE_FAMILY[route_fam]}/local-rib/routes"
                 ),
                 "RIB_IP_JMESPATH": '"network-instance"[].{NI:name, Rib:"bgp-rib"."afi-safi"[]."'
                 + ROUTE_FAMILY[route_fam]
                 + '"."local-rib"."routes"[]'
                 + '.{neighbor:neighbor, "0_st":"_r_state", "Pfx":prefix, "lpref":"local-pref", med:med, "next-hop":"next-hop","as-path":"as-path".segment[0].member,\
-                      "communities":[communities.community, communities."large-community"][]|join(\',\',@)}}',
+                      "communities":[communities.community, communities."large-community"][]|join(\', \',@)}}',
             },
             3: {
                 "RIB_IP_PATH": (
                     f"/network-instance[name={network_instance}]/bgp-rib/afi-safi[afi-safi-name={ROUTE_FAMILY[route_fam]}]/"
                     f"{ROUTE_FAMILY[route_fam]}/local-rib/route"
                 ),
                 "RIB_IP_JMESPATH": '"network-instance"[].{NI:name, Rib:"bgp-rib"."afi-safi"[]."'
@@ -534,66 +554,70 @@
                         ]
                     else:
                         ni["route-table"]["ipv4-unicast"]["route"] = []
                         ni["_hasrib"] = False
                         continue
                 for route in ni["route-table"]["ipv4-unicast"]["route"]:
                     if route["active"]:
-                        route["active"] = "Yes"
+                        route["active"] = "yes"
                     else:
-                        route["active"] = "No"
+                        route["active"] = "no"
                     if "next-hop-group" in route:
                         leaked = False
                         if "origin-network-instance" in route:
                             nh_ni = route["origin-network-instance"]
                             if nh_ni != ni["name"]:
                                 leaked = True
                                 route["_orig_vrf"] = nh_ni
                         else:
                             nh_ni = ni["name"]
                         route["_next-hop"] = [
                             nh.get("ip-address")
-                            for nh in nhgroup_mapping[nh_ni][route["next-hop-group"]]
+                            for nh in nhgroup_mapping[nh_ni].get(
+                                route["next-hop-group"], {}
+                            )
                         ]
 
                         route["_nh_itf"] = [
                             nh.get("subinterface") + f"@vrf:{nh_ni}"
                             if leaked
                             else nh.get("subinterface")
-                            for nh in nhgroup_mapping[nh_ni][route["next-hop-group"]]
+                            for nh in nhgroup_mapping[nh_ni].get(
+                                route["next-hop-group"], {}
+                            )
                             if nh.get("subinterface")
                         ]
                         if len(route["_nh_itf"]) == 0:
                             route["_nh_itf"] = [
                                 nh.get("tunnel")
-                                for nh in nhgroup_mapping[nh_ni][
-                                    route["next-hop-group"]
-                                ]
+                                for nh in nhgroup_mapping[nh_ni].get(
+                                    route["next-hop-group"], {}
+                                )
                                 if nh.get("tunnel")
                             ]
                         if len(route["_nh_itf"]) == 0:
                             resolving_routes = [
                                 nh.get("resolving-route", {})
-                                for nh in nhgroup_mapping[nh_ni][
-                                    route["next-hop-group"]
-                                ]
+                                for nh in nhgroup_mapping[nh_ni].get(
+                                    route["next-hop-group"], {}
+                                )
                                 if nh.get("resolving-route")
                             ]
         #                            if len(resolving_routes) > 0:
         #                                route["_nh_itf"] = [ rt.get("_nh_itf") for rt in ni["route-table"]["ipv4-unicast"]["route"] if rt.get("ipv4-prefix") in [ res_rt.get("ip-prefix") for res_rt in resolving_routes ] ]
 
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {"ipv4_rib": res}
 
     def get_nwi_itf(self, nw_instance: str = "*") -> Dict[str, Any]:
         SUBITF_PATH = "/interface[name=*]/subinterface"
         path_spec = {
             "path": f"/network-instance[name={nw_instance}]",
             "jmespath": '"network-instance"[].{NI:name,oper:"oper-state",type:type,"router-id":protocols.bgp."router-id",\
-                    itfs: interface[].{Subitf:name,"if-oper":"oper-state", ipv4:ipv4.address[]."ip-prefix",\
+                    itfs: interface[].{Subitf:name,"assoc-ni":"_other_ni","if-oper":"oper-state", ipv4:ipv4.address[]."ip-prefix",\
                         vlan:vlan.encap."single-tagged"."vlan-id", "mtu":"_mtu"}}',
             "datatype": "state",
         }
         subitf = {}
         resp = self.get(paths=[SUBITF_PATH], datatype="state")
         for itf in resp[0].get("interface", []):
             for si in itf.get("subinterface", []):
@@ -605,29 +629,39 @@
 
         resp = self.get(
             paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
         )
         for ni in resp[0].get("network-instance", {}):
             for ni_itf in ni.get("interface", []):
                 ni_itf.update(subitf.get(ni_itf["name"], {}))
+                if ni_itf["name"].startswith("irb"):
+                    ni_itf["_other_ni"] = " ".join(
+                        f"{vrf['name']}"
+                        for vrf in resp[0].get("network-instance", {})
+                        if ni_itf["name"] in [i["name"] for i in vrf["interface"]]
+                        and vrf["name"] != ni["name"]
+                    )
 
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {"nwi_itfs": res}
 
     def get_lag(self, lag_id: str = "*") -> Dict[str, Any]:
         path_spec = {
             "path": f"/interface[name=lag{lag_id}]",
-            "jmespath": '"interface"[].{lag:name, oper:"oper-state",mtu:mtu,num:lag.member|length(@),"min":lag."min-links",desc:description, type:lag."lag-type", speed:lag."lag-speed","stby-sig":ethernet."standby-signaling",\
+            "jmespath": '"interface"[].{lag:name, oper:"oper-state",mtu:mtu,"min":lag."min-links",desc:description, type:lag."lag-type", speed:lag."lag-speed","stby-sig":ethernet."standby-signaling",\
                   "lacp-key":lag.lacp."admin-key","lacp-itvl":lag.lacp.interval,"lacp-mode":lag.lacp."lacp-mode","lacp-sysid":lag.lacp."system-id-mac","lacp-prio":lag.lacp."system-priority",\
                     members:lag.member[].{"member-itf":name, "member-oper":"oper-state","act":lacp."activity"}}',
             "datatype": "state",
         }
         resp = self.get(
             paths=[path_spec.get("path", "")], datatype=path_spec["datatype"]
         )
+        for itf in resp[0].get("interface", []):
+            for member in itf.get("lag", {}).get("member", []):
+                member["name"] = str(member.get("name", "")).replace("ethernet", "et")
         res = jmespath.search(path_spec["jmespath"], resp[0])
         return {"lag": res}
 
     def get_es(self) -> Dict[str, Any]:
         path_spec = {
             "path": f"/system/network-instance/protocols/evpn/ethernet-segments",
             "jmespath": '"system/network-instance/protocols/evpn/ethernet-segments"."bgp-instance"[]."ethernet-segment"[].{name:name, esi:esi, "mh-mode":"multi-homing-mode",\
```

### Comparing `nornir_srl-0.2.8/nornir_srl/fsc.py` & `nornir_srl-0.2.9/nornir_srl/fsc.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.2.8/nornir_srl/tasks/srl_config.py` & `nornir_srl-0.2.9/nornir_srl/tasks/srl_config.py`

 * *Files identical despite different names*

### Comparing `nornir_srl-0.2.8/pyproject.toml` & `nornir_srl-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir-srl"
-version = "0.2.8"
+version = "0.2.9"
 description = "Nornir connection plugin for SRLinux"
 authors = ["Walter De Smedt <walter.de.smedt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/srl-labs/nornir-srl"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nornir_srl-0.2.8/PKG-INFO` & `nornir_srl-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-srl
-Version: 0.2.8
+Version: 0.2.9
 Summary: Nornir connection plugin for SRLinux
 Home-page: https://github.com/srl-labs/nornir-srl
 Author: Walter De Smedt
 Author-email: walter.de.smedt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

