# Comparing `tmp/cs2solutions-0.7.5.tar.gz` & `tmp/cs2solutions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dejan/eth/CSII/cs2solutions/dist/.tmp-39lyk24a/cs2solutions-0.7.5.tar", last modified: Tue Apr 23 07:25:49 2024, max compression
+gzip compressed data, was "cs2solutions-0.8.0.tar", last modified: Mon Apr 29 19:48:34 2024, max compression
```

## Comparing `cs2solutions-0.7.5.tar` & `cs2solutions-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 07:25:49.921583 cs2solutions-0.7.5/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    35149 2024-02-20 16:57:23.000000 cs2solutions-0.7.5/LICENSE
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42320 2024-04-23 07:25:49.921583 cs2solutions-0.7.5/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      706 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/README.md
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     1294 2024-04-23 07:25:37.000000 cs2solutions-0.7.5/pyproject.toml
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       38 2024-04-23 07:25:49.921583 cs2solutions-0.7.5/setup.cfg
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 07:25:49.917583 cs2solutions-0.7.5/src/
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 07:25:49.921583 cs2solutions-0.7.5/src/cs2solutions/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      151 2024-04-22 07:50:49.000000 cs2solutions-0.7.5/src/cs2solutions/__init__.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     6885 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/aircraft.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        0 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/cs.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     5975 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/cs2bot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10851 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/decomp.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    21154 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/discretization.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10908 2024-04-16 07:25:19.000000 cs2solutions-0.7.5/src/cs2solutions/duckiebot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     7763 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/intro.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    15366 2024-04-16 15:23:07.000000 cs2solutions-0.7.5/src/cs2solutions/intromimo.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13252 2024-04-16 07:25:19.000000 cs2solutions-0.7.5/src/cs2solutions/lqg.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10752 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/lqrfeedback.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13341 2024-03-25 18:09:11.000000 cs2solutions-0.7.5/src/cs2solutions/morse.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    15555 2024-04-22 07:50:49.000000 cs2solutions-0.7.5/src/cs2solutions/norms.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       90 2024-02-20 16:57:23.000000 cs2solutions-0.7.5/src/cs2solutions/plot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       68 2024-02-20 16:57:23.000000 cs2solutions-0.7.5/src/cs2solutions/test.py
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 07:25:49.921583 cs2solutions-0.7.5/src/cs2solutions.egg-info/
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42320 2024-04-23 07:25:49.000000 cs2solutions-0.7.5/src/cs2solutions.egg-info/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      645 2024-04-23 07:25:49.000000 cs2solutions-0.7.5/src/cs2solutions.egg-info/SOURCES.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        1 2024-04-23 07:25:49.000000 cs2solutions-0.7.5/src/cs2solutions.egg-info/dependency_links.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       44 2024-04-23 07:25:49.000000 cs2solutions-0.7.5/src/cs2solutions.egg-info/requires.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       13 2024-04-23 07:25:49.000000 cs2solutions-0.7.5/src/cs2solutions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.784990 cs2solutions-0.8.0/
+-rw-rw-rw-   0        0        0    35823 2024-02-17 10:04:18.000000 cs2solutions-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0    43040 2024-04-29 19:48:34.780651 cs2solutions-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/README.md
+-rw-rw-rw-   0        0        0     1294 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 19:48:34.784990 cs2solutions-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.701973 cs2solutions-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.751672 cs2solutions-0.8.0/src/cs2solutions/
+-rw-rw-rw-   0        0        0      163 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/__init__.py
+-rw-rw-rw-   0        0        0     7065 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/aircraft.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/cs.py
+-rw-rw-rw-   0        0        0     6142 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/cs2bot.py
+-rw-rw-rw-   0        0        0    11149 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/decomp.py
+-rw-rw-rw-   0        0        0    21713 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/discretization.py
+-rw-rw-rw-   0        0        0    11230 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/duckiebot.py
+-rw-rw-rw-   0        0        0     3480 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/inf_pkg.py
+-rw-rw-rw-   0        0        0     7967 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/intro.py
+-rw-rw-rw-   0        0        0    15791 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/intromimo.py
+-rw-rw-rw-   0        0        0    13575 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/lqg.py
+-rw-rw-rw-   0        0        0    11049 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/lqrfeedback.py
+-rw-rw-rw-   0        0        0    13739 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/morse.py
+-rw-rw-rw-   0        0        0    16030 2024-04-29 19:47:44.000000 cs2solutions-0.8.0/src/cs2solutions/norms.py
+-rw-rw-rw-   0        0        0       93 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/plot.py
+-rw-rw-rw-   0        0        0       68 2024-02-21 18:21:30.000000 cs2solutions-0.8.0/src/cs2solutions/test.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:48:34.768512 cs2solutions-0.8.0/src/cs2solutions.egg-info/
+-rw-rw-rw-   0        0        0    43040 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 19:48:34.000000 cs2solutions-0.8.0/src/cs2solutions.egg-info/top_level.txt
```

### Comparing `cs2solutions-0.7.5/LICENSE` & `cs2solutions-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `cs2solutions-0.7.5/PKG-INFO` & `cs2solutions-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,720 +1,720 @@
-Metadata-Version: 2.1
-Name: cs2solutions
-Version: 0.7.5
-Summary: A package containing solutions for the CS2 lecture at ETH Zürich
-Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
-Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://idsc.ethz.ch/education/lectures/control-systems-ii.html
-Project-URL: Repository, https://github.com/idsc-frazzoli/cs2solutions
-Project-URL: Notebooks, https://github.com/idsc-frazzoli/CS2-2024-notebooks
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: control
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: sympy
-Requires-Dist: pandas
-
-# [cs2solutions]
-
-Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
-Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
-
-## pip Installation
-The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
-
-```bash
-pip install cs2solutions
-```
-
-Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
-
-## Features
-Contains:
-- Utility functions for control systems, such as plotting and generic formulas
-- Solutions for all notebooks
-- Unit tests to check student implementations of code
-
-
+Metadata-Version: 2.1
+Name: cs2solutions
+Version: 0.8.0
+Summary: A package containing solutions for the CS2 lecture at ETH Zürich
+Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
+Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://idsc.ethz.ch/education/lectures/control-systems-ii.html
+Project-URL: Repository, https://github.com/idsc-frazzoli/cs2solutions
+Project-URL: Notebooks, https://github.com/idsc-frazzoli/CS2-2024-notebooks
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: control
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: sympy
+Requires-Dist: pandas
+
+# [cs2solutions]
+
+Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
+Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
+
+## pip Installation
+The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
+
+```bash
+pip install cs2solutions
+```
+
+Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
+
+## Features
+Contains:
+- Utility functions for control systems, such as plotting and generic formulas
+- Solutions for all notebooks
+- Unit tests to check student implementations of code
+
+
```

### Comparing `cs2solutions-0.7.5/README.md` & `cs2solutions-0.8.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# [cs2solutions]
-
-Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
-Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
-
-## pip Installation
-The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
-
-```bash
-pip install cs2solutions
-```
-
-Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
-
-## Features
-Contains:
-- Utility functions for control systems, such as plotting and generic formulas
-- Solutions for all notebooks
-- Unit tests to check student implementations of code
-
-
+# [cs2solutions]
+
+Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
+Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
+
+## pip Installation
+The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
+
+```bash
+pip install cs2solutions
+```
+
+Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
+
+## Features
+Contains:
+- Utility functions for control systems, such as plotting and generic formulas
+- Solutions for all notebooks
+- Unit tests to check student implementations of code
+
+
```

### Comparing `cs2solutions-0.7.5/pyproject.toml` & `cs2solutions-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/solutions"]
 
 [project]
 name = "cs2solutions"
-version = "0.7.5"
+version = "0.8.0"
 dependencies =[
     "control",
     "matplotlib",
     "numpy",
     "scipy",
     "sympy",
     "pandas"
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/aircraft.py` & `cs2solutions-0.8.0/src/cs2solutions/aircraft.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-def sol_aircraft_state_space() -> ct.StateSpace:
-    """
-    Produce the linear state space model of the aircraft.
-  
-    Parameters:
-    - None
-
-    Returns:
-    - () -> StateSpace: The state space model of the aircraft.
-    """
-    A_sol = np.array([
-    [-15.5801, 4.7122, -38.7221, 0],
-    [-0.5257, -0.0166, 2.3501, -9.7847],
-    [4.4044, -1.5325, -18.1615, -0.7044],
-    [0.9974, 0, 0, 0]
-    ])
-
-    B_sol = np.array([
-        [-421.2001],
-        [1.3231],
-        [-17.3812],
-        [0]
-    ])
-
-    C_sol = np.array([[0, 0, 0, 1]])
-
-    D_sol = np.array([[0]])
-
-    return ct.StateSpace(A_sol, B_sol, C_sol, D_sol)
-
-
-def test_aircraft_state_space(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's state space model with the solution state space model.
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's state space model.
-    - ``actual_sol`` (function): A function that returns the solution state space model.
-    - ``shouldprint`` (bool): A boolean indicating whether to print the state space models. Default is True.
-
-    Raises:
-    - AssertionError: If the input is not an instance of the StateSpace class.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the student's state space model is equal to the solution state space model.
-    """
-
-    # Create a state space model using the student's code
-    student_model = student_sol()
-    # Create a state space model using the solution code
-    sol_model = actual_sol()
-
-    # Check if the student's state space model is an instance of the StateSpace class
-    assert not isinstance(student_model, type(None)), f"Please make sure to return a StateSpace object. Got {type(student_model)} instead."
-    assert isinstance(student_model, ct.StateSpace), f"Expected a StateSpace object, but got {type(student_model)}"
-
-    # Check if the student's state space model is equal to the solution state space model
-    if shouldprint:
-        print("Student's state space model:")
-        print(student_model)
-        print("\nSolution state space model:")
-        print(sol_model)
-
-    assert np.array_equal(student_model.A, sol_model.A), "The state space model A matrix is incorrect."
-    assert np.array_equal(student_model.B, sol_model.B), "The state space model B matrix is incorrect."
-    assert np.array_equal(student_model.C, sol_model.C), "The state space model C matrix is incorrect."
-    assert np.array_equal(student_model.D, sol_model.D), "The state space model D matrix is incorrect."
-
-    return True
-
-
-def sol_is_system_stable(sys: ct.StateSpace) -> bool:
-    """
-    Determine if the given state space system is stable.
-
-    Parameters:
-    - ``sys`` (StateSpace): The state space model of the system.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the system is stable.
-    """
-    return np.all(np.linalg.eigvals(sys.A) < 0)
-
-
-def test_is_system_stable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's stability check with the solution stability check.
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's stability check.
-    - ``actual_sol`` (function): A function that returns the solution stability check.
-    - ``shouldprint`` (bool): A boolean indicating whether to print the stability checks. Default is True.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the student's stability check is equal to the solution stability check.
-    """
-
-    passed_tests = 0
-
-    # Conduct four unit tests
-    # Test 0: Check if is_system_stable doesn't return None
-    sys_dummy = ct.StateSpace(np.array([[1, 0], [0, 1]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
-    result = student_sol(sys_dummy)
-    print("Test failed: is_system_stable should return a boolean value." if result is None else "")
-    print("Student's result: ", result)
-    print("Expected result: ", actual_sol(sys_dummy))
-    passed_tests += 1 if result == actual_sol(sys_dummy) else 0
-
-    # Test 1: Check if is_system_stable returns False for an unstable system
-    sys_unstable = ct.StateSpace(np.array([[1, 1], [0, 1]]), np.array([[1], [0]]), np.array([[1, 0]]), np.array([[0]]))
-    result = student_sol(sys_unstable)
-    print("Student's result: ", result)
-    print("Expected result: ", actual_sol(sys_unstable))
-    passed_tests += 1 if result == actual_sol(sys_unstable) else 0
-
-    # Test 2: Marginally stable system
-    sys_marginally_stable = ct.StateSpace(np.array([[0, 1], [-1, 0]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
-    result = student_sol(sys_marginally_stable)
-    print("Student's result: ", result)
-    print("Expected result: ", actual_sol(sys_marginally_stable))
-    passed_tests += 1 if result == actual_sol(sys_marginally_stable) else 0
-
-    # Test 3: Stable system
-    sys_stable = ct.StateSpace(np.array([[-0.5, 0], [0, -1]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
-    result = student_sol(sys_stable)
-    print("Student's result: ", result)
-    print("Expected result: ", actual_sol(sys_stable))
-    passed_tests += 1 if result == actual_sol(sys_stable) else 0
-
-    # Test 4: Check aircraft stability
-    sys_aircraft = sol_aircraft_state_space()
-    result = student_sol(sys_aircraft)
-    print("Student's result: ", result)
-    print("Expected result: ", actual_sol(sys_aircraft))
-    passed_tests += 1 if result == actual_sol(sys_aircraft) else 0
-
-    print("Passed tests: ", passed_tests, "/5")
-    return passed_tests == 5
-
-
-def sol_plot_initial_conditions_response(sys: ct.StateSpace, initial_conditions: np.array) -> None:
-    """
-    Plot the system response to the given initial conditions.
-    
-    Parameters:
-    - ``sys`` (ct.StateSpace): The state space representation of the system.
-    - ``initial_conditions`` (np.array): The initial conditions of the system.
-
-    Returns:
-        None
-    """
-    
-    # Simulate the system response to the given initial conditions
-    print(initial_conditions)
-    time, response = ct.initial_response(sys, X0 = initial_conditions, T=250)
-
-    # Plot the response
-    plt.figure(figsize=(10, 6))
-
-    # Plot pitch rate (q)
-    plt.plot(time, response)
-    plt.xlabel('Time (s)')
-    plt.ylabel('System output')
-    plt.title('Initial condition response')
-    plt.show()
-
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+def sol_aircraft_state_space() -> ct.StateSpace:
+    """
+    Produce the linear state space model of the aircraft.
+  
+    Parameters:
+    - None
+
+    Returns:
+    - () -> StateSpace: The state space model of the aircraft.
+    """
+    A_sol = np.array([
+    [-15.5801, 4.7122, -38.7221, 0],
+    [-0.5257, -0.0166, 2.3501, -9.7847],
+    [4.4044, -1.5325, -18.1615, -0.7044],
+    [0.9974, 0, 0, 0]
+    ])
+
+    B_sol = np.array([
+        [-421.2001],
+        [1.3231],
+        [-17.3812],
+        [0]
+    ])
+
+    C_sol = np.array([[0, 0, 0, 1]])
+
+    D_sol = np.array([[0]])
+
+    return ct.StateSpace(A_sol, B_sol, C_sol, D_sol)
+
+
+def test_aircraft_state_space(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's state space model with the solution state space model.
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's state space model.
+    - ``actual_sol`` (function): A function that returns the solution state space model.
+    - ``shouldprint`` (bool): A boolean indicating whether to print the state space models. Default is True.
+
+    Raises:
+    - AssertionError: If the input is not an instance of the StateSpace class.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the student's state space model is equal to the solution state space model.
+    """
+
+    # Create a state space model using the student's code
+    student_model = student_sol()
+    # Create a state space model using the solution code
+    sol_model = actual_sol()
+
+    # Check if the student's state space model is an instance of the StateSpace class
+    assert not isinstance(student_model, type(None)), f"Please make sure to return a StateSpace object. Got {type(student_model)} instead."
+    assert isinstance(student_model, ct.StateSpace), f"Expected a StateSpace object, but got {type(student_model)}"
+
+    # Check if the student's state space model is equal to the solution state space model
+    if shouldprint:
+        print("Student's state space model:")
+        print(student_model)
+        print("\nSolution state space model:")
+        print(sol_model)
+
+    assert np.array_equal(student_model.A, sol_model.A), "The state space model A matrix is incorrect."
+    assert np.array_equal(student_model.B, sol_model.B), "The state space model B matrix is incorrect."
+    assert np.array_equal(student_model.C, sol_model.C), "The state space model C matrix is incorrect."
+    assert np.array_equal(student_model.D, sol_model.D), "The state space model D matrix is incorrect."
+
+    return True
+
+
+def sol_is_system_stable(sys: ct.StateSpace) -> bool:
+    """
+    Determine if the given state space system is stable.
+
+    Parameters:
+    - ``sys`` (StateSpace): The state space model of the system.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the system is stable.
+    """
+    return np.all(np.linalg.eigvals(sys.A) < 0)
+
+
+def test_is_system_stable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's stability check with the solution stability check.
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's stability check.
+    - ``actual_sol`` (function): A function that returns the solution stability check.
+    - ``shouldprint`` (bool): A boolean indicating whether to print the stability checks. Default is True.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the student's stability check is equal to the solution stability check.
+    """
+
+    passed_tests = 0
+
+    # Conduct four unit tests
+    # Test 0: Check if is_system_stable doesn't return None
+    sys_dummy = ct.StateSpace(np.array([[1, 0], [0, 1]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
+    result = student_sol(sys_dummy)
+    print("Test failed: is_system_stable should return a boolean value." if result is None else "")
+    print("Student's result: ", result)
+    print("Expected result: ", actual_sol(sys_dummy))
+    passed_tests += 1 if result == actual_sol(sys_dummy) else 0
+
+    # Test 1: Check if is_system_stable returns False for an unstable system
+    sys_unstable = ct.StateSpace(np.array([[1, 1], [0, 1]]), np.array([[1], [0]]), np.array([[1, 0]]), np.array([[0]]))
+    result = student_sol(sys_unstable)
+    print("Student's result: ", result)
+    print("Expected result: ", actual_sol(sys_unstable))
+    passed_tests += 1 if result == actual_sol(sys_unstable) else 0
+
+    # Test 2: Marginally stable system
+    sys_marginally_stable = ct.StateSpace(np.array([[0, 1], [-1, 0]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
+    result = student_sol(sys_marginally_stable)
+    print("Student's result: ", result)
+    print("Expected result: ", actual_sol(sys_marginally_stable))
+    passed_tests += 1 if result == actual_sol(sys_marginally_stable) else 0
+
+    # Test 3: Stable system
+    sys_stable = ct.StateSpace(np.array([[-0.5, 0], [0, -1]]), np.array([[1], [0]]), np.array([[0, 1]]), np.array([[0]]))
+    result = student_sol(sys_stable)
+    print("Student's result: ", result)
+    print("Expected result: ", actual_sol(sys_stable))
+    passed_tests += 1 if result == actual_sol(sys_stable) else 0
+
+    # Test 4: Check aircraft stability
+    sys_aircraft = sol_aircraft_state_space()
+    result = student_sol(sys_aircraft)
+    print("Student's result: ", result)
+    print("Expected result: ", actual_sol(sys_aircraft))
+    passed_tests += 1 if result == actual_sol(sys_aircraft) else 0
+
+    print("Passed tests: ", passed_tests, "/5")
+    return passed_tests == 5
+
+
+def sol_plot_initial_conditions_response(sys: ct.StateSpace, initial_conditions: np.array) -> None:
+    """
+    Plot the system response to the given initial conditions.
+    
+    Parameters:
+    - ``sys`` (ct.StateSpace): The state space representation of the system.
+    - ``initial_conditions`` (np.array): The initial conditions of the system.
+
+    Returns:
+        None
+    """
+    
+    # Simulate the system response to the given initial conditions
+    print(initial_conditions)
+    time, response = ct.initial_response(sys, X0 = initial_conditions, T=250)
+
+    # Plot the response
+    plt.figure(figsize=(10, 6))
+
+    # Plot pitch rate (q)
+    plt.plot(time, response)
+    plt.xlabel('Time (s)')
+    plt.ylabel('System output')
+    plt.title('Initial condition response')
+    plt.show()
+
     return None
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/cs2bot.py` & `cs2solutions-0.8.0/src/cs2solutions/cs2bot.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-def sol_get_xdot(t: float, x: np.array, u: np.array, params: dict) -> np.array:
-    """
-    Solution: Return the derivative of the state vector, aka x\dot.
-
-    Parameters:
-    - ``t`` (float): The current time.	
-    - ``x`` (np.array): The current state.
-    - ``u`` (np.array): The current input.
-    - ``params`` (dict): A dictionary of parameters.
-
-    Returns:
-    - np.array: The derivative of the state.
-    """
-
-     # Return the derivative of the state
-    max_omega = params.get('max_omega', 0.05)
-    omega = np.clip(u[1], -max_omega, max_omega)
-    return np.array([
-        u[0] * np.cos(x[2]),    # xdot = v cos(theta)
-        u[0] * np.sin(x[2]),    # ydot = v sin(theta)
-        omega     # thdot = w
-    ])
-
-def assert_almost_equal(actual: float, expected: float, tolerance=1e-5) -> bool:
-    try:
-        almost_equal = np.all(np.abs(actual - expected) < tolerance)
-        return almost_equal
-    except Exception:
-        return False
-
-def test_xdot(student_sol: callable, actual_sol: callable, tolerance: float = 1e-5) -> bool:
-    """
-    Tests the student solution for get_xdot.
-
-    Parameters:
-    - ``student_sol`` (function): Student solution.	
-    - ``actual_sol`` (function): Expected solution function.
-    - ``tolerance`` (float): Tolerance for float equality.
-
-    Returns:
-    - bool: Whether all unit tests passed.
-    """
-    passed_tests = 0
-
-    # Test 0: Check correct return value
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])   # initial state [x, y, theta]
-    u = np.array([1.0, 0.1])        # input [v, omega]
-    result = student_sol(0.0, x, u, params)
-    solution = actual_sol(0.0, x, u, params)
-    print("Test failed: get_xdot should a np.array" if result is None else "")
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    # Test 1: Check forward motion
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])  # initial state [x, y, theta]
-    u = np.array([2.0, 0.0])       # input [v, omega]
-    result = student_sol(0.0, x, u, params)
-    solution = actual_sol(0.0, x, u, params)
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    # Test 2: Check rotation
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])
-    u = np.array([0.0, 0.01])
-    result = student_sol(0.0, x, u, params)
-    solution = np.array([0.0, 0.0, 0.01])
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    # Test 3: Check clipping omega
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])
-    u = np.array([0.0, 0.1])  # omega exceeds max_omega
-    result = student_sol(0.0, x, u, params)
-    solution = np.array([0.0, 0.0, params['max_omega']])
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    # Test 4: Check combined motion
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, np.pi/4])
-    u = np.array([1.0, 0.1])
-    result = student_sol(0.0, x, u, params)
-    solution = np.array([np.cos(np.pi/4), np.sin(np.pi/4), 0.05])
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    print("Passed tests: ", passed_tests, "/5")
-    return passed_tests == 5
-
-
-def sol_get_y(t: float, x: np.array, u: np.array, params: dict) -> np.array:
-    """
-    Solution: Returns the state vector, aka [x, y, \omega].
-
-    Parameters:
-    - ``t`` (float): The current time.	
-    - ``x`` (np.array): The current state.
-    - ``u`` (np.array): The current input.
-    - ``params`` (dict): A dictionary of parameters.
-
-    Returns:
-    - np.array: The the state vector
-    """
-    # Returns the state vector
-    return x[0:2]
-
-
-def test_y(student_sol: callable, actual_sol: callable, tolerance: float = 1e-5) -> bool:
-    """
-    Tests the student solution for get_y.
-
-    Parameters:
-    - ``student_sol`` (function): Student solution.	
-    - ``actual_sol`` (function): Expected solution function.
-    - ``tolerance`` (float): Tolerance for float equality.
-
-    Returns:
-    - bool: Whether all unit tests passed.
-    """
-    passed_tests = 0
-
-    # Test 0: Check correct return value
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])   # initial state [x, y, theta]
-    u = np.array([1.0, 0.1])        # input [v, omega]
-    result = student_sol(0.0, x, u, params)
-    solution = actual_sol(0.0, x, u, params)
-    print("Test failed: get_y should return a np.array" if result is None else "")
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    # Test 1: Check forward motion
-    params = {'max_omega': 0.05}
-    x = np.array([1.0, 2.0, 0.0])  # initial state [x, y, theta]
-    u = np.array([2.0, 0.0])       # input [v, omega]
-    result = student_sol(0.0, x, u, params)
-    solution = np.array([1.0, 2.0])
-    print("Student's result: ", result)
-    print("Expected result: ", solution)
-    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
-
-    print("Passed tests: ", passed_tests, "/2")
-    return passed_tests == 2
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+def sol_get_xdot(t: float, x: np.array, u: np.array, params: dict) -> np.array:
+    """
+    Solution: Return the derivative of the state vector, aka x\dot.
+
+    Parameters:
+    - ``t`` (float): The current time.	
+    - ``x`` (np.array): The current state.
+    - ``u`` (np.array): The current input.
+    - ``params`` (dict): A dictionary of parameters.
+
+    Returns:
+    - np.array: The derivative of the state.
+    """
+
+     # Return the derivative of the state
+    max_omega = params.get('max_omega', 0.05)
+    omega = np.clip(u[1], -max_omega, max_omega)
+    return np.array([
+        u[0] * np.cos(x[2]),    # xdot = v cos(theta)
+        u[0] * np.sin(x[2]),    # ydot = v sin(theta)
+        omega     # thdot = w
+    ])
+
+def assert_almost_equal(actual: float, expected: float, tolerance=1e-5) -> bool:
+    try:
+        almost_equal = np.all(np.abs(actual - expected) < tolerance)
+        return almost_equal
+    except Exception:
+        return False
+
+def test_xdot(student_sol: callable, actual_sol: callable, tolerance: float = 1e-5) -> bool:
+    """
+    Tests the student solution for get_xdot.
+
+    Parameters:
+    - ``student_sol`` (function): Student solution.	
+    - ``actual_sol`` (function): Expected solution function.
+    - ``tolerance`` (float): Tolerance for float equality.
+
+    Returns:
+    - bool: Whether all unit tests passed.
+    """
+    passed_tests = 0
+
+    # Test 0: Check correct return value
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])   # initial state [x, y, theta]
+    u = np.array([1.0, 0.1])        # input [v, omega]
+    result = student_sol(0.0, x, u, params)
+    solution = actual_sol(0.0, x, u, params)
+    print("Test failed: get_xdot should a np.array" if result is None else "")
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    # Test 1: Check forward motion
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])  # initial state [x, y, theta]
+    u = np.array([2.0, 0.0])       # input [v, omega]
+    result = student_sol(0.0, x, u, params)
+    solution = actual_sol(0.0, x, u, params)
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    # Test 2: Check rotation
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])
+    u = np.array([0.0, 0.01])
+    result = student_sol(0.0, x, u, params)
+    solution = np.array([0.0, 0.0, 0.01])
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    # Test 3: Check clipping omega
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])
+    u = np.array([0.0, 0.1])  # omega exceeds max_omega
+    result = student_sol(0.0, x, u, params)
+    solution = np.array([0.0, 0.0, params['max_omega']])
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    # Test 4: Check combined motion
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, np.pi/4])
+    u = np.array([1.0, 0.1])
+    result = student_sol(0.0, x, u, params)
+    solution = np.array([np.cos(np.pi/4), np.sin(np.pi/4), 0.05])
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    print("Passed tests: ", passed_tests, "/5")
+    return passed_tests == 5
+
+
+def sol_get_y(t: float, x: np.array, u: np.array, params: dict) -> np.array:
+    """
+    Solution: Returns the state vector, aka [x, y, \omega].
+
+    Parameters:
+    - ``t`` (float): The current time.	
+    - ``x`` (np.array): The current state.
+    - ``u`` (np.array): The current input.
+    - ``params`` (dict): A dictionary of parameters.
+
+    Returns:
+    - np.array: The the state vector
+    """
+    # Returns the state vector
+    return x[0:2]
+
+
+def test_y(student_sol: callable, actual_sol: callable, tolerance: float = 1e-5) -> bool:
+    """
+    Tests the student solution for get_y.
+
+    Parameters:
+    - ``student_sol`` (function): Student solution.	
+    - ``actual_sol`` (function): Expected solution function.
+    - ``tolerance`` (float): Tolerance for float equality.
+
+    Returns:
+    - bool: Whether all unit tests passed.
+    """
+    passed_tests = 0
+
+    # Test 0: Check correct return value
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])   # initial state [x, y, theta]
+    u = np.array([1.0, 0.1])        # input [v, omega]
+    result = student_sol(0.0, x, u, params)
+    solution = actual_sol(0.0, x, u, params)
+    print("Test failed: get_y should return a np.array" if result is None else "")
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    # Test 1: Check forward motion
+    params = {'max_omega': 0.05}
+    x = np.array([1.0, 2.0, 0.0])  # initial state [x, y, theta]
+    u = np.array([2.0, 0.0])       # input [v, omega]
+    result = student_sol(0.0, x, u, params)
+    solution = np.array([1.0, 2.0])
+    print("Student's result: ", result)
+    print("Expected result: ", solution)
+    passed_tests += 1 if assert_almost_equal(result, solution, tolerance) else 0
+
+    print("Passed tests: ", passed_tests, "/2")
+    return passed_tests == 2
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/decomp.py` & `cs2solutions-0.8.0/src/cs2solutions/decomp.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-
-def print_nice(state: List[np.ndarray]) -> None:
-    """
-    Prints the state-space matrices in a nice format.
-
-    Parameters:
-    - ``state`` (List[np.ndarray]): A list of state-space matrices.
-    """
-    matrix_names = ["A", "B", "C", "D"]
-    for mat, name in zip(state, matrix_names):
-        print(f"Matrix {name}:")
-        print(np.array2string(mat, precision=3, suppress_small=True))
-        print()
-
-def sol_diagonalize_system(A: np.array, B: np.array, C: np.array, D: np.array) -> tuple[np.array]:
-    """
-    Diagonalizes a linear time-invariant system represented by its state-space matrices.
-
-    Parameters:
-    - ``A`` (np.array): State matrix of the system.
-    - ``B`` (np.array): Input matrix of the system.
-    - ``C`` (np.array): Output matrix of the system.
-    - ``D`` (np.array): Feedthrough matrix of the system.
-
-    Returns:
-    - ``A_tilde`` (np.array): Diagonalized state matrix.
-    - ``B_tilde`` (np.array): Diagonalized input matrix.
-    - ``C_tilde`` (np.array): Diagonalized output matrix.
-    - ``D_tilde`` (np.array): Diagonalized feedthrough matrix.
-    """
-    # Preliminary safety checks
-    D = np.array(D)
-    if not all(isinstance(mat, np.ndarray) for mat in [A, B, C, D]):
-        raise TypeError("All input matrices must be numpy arrays.")
-    if A.shape[0] != A.shape[1]:
-        raise ValueError("Matrix A must be square.")
-
-    # Compute the eigenvalues and eigenvectors of matrix A
-    eigenvalues, eigenvectors = np.linalg.eig(A)
-
-    # Compute the transformed state-space representation
-    # The diagonal matrix A_tilde contains the eigenvalues of A
-    A_tilde = np.diag(eigenvalues)
-    
-    # The input matrix B_tilde is obtained by transforming the input matrix B
-    # using the inverse of the eigenvector matrix
-    B_tilde = np.linalg.inv(eigenvectors) @ B
-    
-    # The output matrix C_tilde is obtained by transforming the output matrix C
-    # using the eigenvector matrix
-    C_tilde = C @ eigenvectors
-    
-    # The feedthrough matrix D_tilde remains the same
-    D_tilde = D
-    
-    return A_tilde, B_tilde, C_tilde, D_tilde
-
-
-def test_diagonalize_system(student_sol: callable, actual_sol: callable, A3: np.array, B3: np.array, C3: np.array, D3: np.array, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's diagonalized system with the solution diagonalized system.
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's diagonalized system.
-    - ``actual_sol`` (function): A function that returns the solution diagonalized system.
-    - ``A3`` (np.array): State matrix of the system.
-    - ``B3`` (np.array): Input matrix of the system.
-    - ``C3`` (np.array): Output matrix of the system.
-    - ``D3`` (np.array): Feedthrough matrix of the system.
-    - ``shouldprint`` (bool): A boolean indicating whether to print the diagonalized systems. Default is True.
-
-    Raises:
-    - AssertionError: If the input matrices are not numpy arrays.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the student's diagonalized system is equal to the solution diagonalized system.
-    """
-    passed_tests = 0
-
-    # Already diagonalized system
-    A1 = np.array([[1, 0], [0, 2]])
-    B1 = np.array([[1], [1]])
-    C1 = np.array([[1, 0]])
-    D1 = np.array([[0]])
-    try:
-        student1 = student_sol(A1, B1, C1, D1)
-    except Exception as e:
-        print("Error in diagonalize_system:", e)
-        student1 = None
-    solution1 = actual_sol(A1, B1, C1, D1)
-    if shouldprint: print("Student 1:")
-    if shouldprint: print_nice(student1)
-    if shouldprint: print("Solution 1:")
-    if shouldprint: print_nice(solution1)
-    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student1, solution1)) else 0
-
-    # Random system
-    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]]);
-    B2 = np.array([[0], [0], [1], [0]])
-    C2 = np.array([1, 0, 0, 0])
-    D2 = np.array([0])
-    try:
-        student2 = student_sol(A2, B2, C2, D2)
-    except Exception as e:
-        print("Error in diagonalize_system:", e)
-        student2 = None
-    solution2 = actual_sol(A2, B2, C2, D2)
-    if shouldprint: print("Student 2:")
-    if shouldprint: print_nice(student2)
-    if shouldprint: print("Solution 2:")
-    if shouldprint: print_nice(solution2)
-    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student2, solution2)) else 0
-
-    # Aircraft System
-    D3 = np.array(D3)
-    try:
-        student3 = student_sol(A3, B3, C3, D3)
-    except Exception as e:
-        print("Error in diagonalize_system:", e)
-        student3 = None
-    solution3 = actual_sol(A3, B3, C3, D3)
-    if shouldprint: print("Student 3:")
-    if shouldprint: print_nice(student3)
-    if shouldprint: print("Solution 3:")
-    if shouldprint: print_nice(solution3)
-    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student3, solution3)) else 0
-
-    print("Passed tests:", passed_tests, " out of 3")
-    return passed_tests == 3
-
-
-def sol_controllable(A: np.array, B: np.array) -> bool:
-    """
-    Check the controllability of a system given the state-space representation.
-
-    Parameters:
-    - ``A`` (np.array): The state matrix.
-    - ``B`` (np.array): The input matrix.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the system is controllable.
-    """
-    
-    n = A.shape[0]  # Get the number of rows in matrix A.
-    R = B  # Initialize the controllability matrix R with matrix B, since the first column of R is always B.
-    
-    for i in range(1, n):  # Iterate from 1 to n-1.
-        # Calculate the reachability matrix for each power of A and concatenate it horizontally to R.
-        R = np.hstack((R, np.linalg.matrix_power(A, i) @ B))
-    
-    rank = np.linalg.matrix_rank(R)
-    
-    if rank == A.shape[0]:
-        print(f"The system is controllable with rank {rank}.")
-    else:
-        print(f"The system is not controllable with rank {rank}.")
-    return rank == n
-
-
-def sol_observable(A: np.array, C: np.array) -> None:
-    """
-    Check the observability of a system given the state-space representation.
-
-    Parameters:
-    - ``A`` (np.array): The state matrix.
-    - ``C`` (np.array): The output matrix.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the system is observable.
-    """
-
-    n = A.shape[0]  # Get the number of rows in matrix A.
-    O = C  # Initialize the observability matrix O with matrix C, since the first row of O is always C.
-    
-    """
-    Same as above, maybe show how to extract the first row programmatically (e.g. O = C[0,:])
-    """
-    
-    for i in range(1, n):  # Iterate from 1 to n-1.
-        # Calculate the observability matrix for each power of A and concatenate it vertically to O.
-        O = np.vstack((O, C @ np.linalg.matrix_power(A, i)))
-    
-    rank = np.linalg.matrix_rank(O)
-    
-    if rank == A.shape[0]:
-        print(f"The system is observable with rank {rank}.")
-    else:
-        print(f"The system is not observable with rank {rank}.")
-    return rank == n
-
-
-def test_controllable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's controllability check with the solution controllability check.
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's controllability check.
-    - ``actual_sol`` (function): A function that returns the solution controllability check.
-    - ``shouldprint`` (bool): A boolean indicating whether to print the controllability checks. Default is True.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the student's controllability check is equal to the solution controllability check.
-    """
-    passed_tests = 0
-
-    # Controllable system
-    A1 = np.array([[1, 0], [0, 2]])
-    B1 = np.array([[1], [1]])
-    print("Student solution:")
-    try:
-        student1 = student_sol(A1, B1)
-        print(student1)
-    except Exception as e:
-        print("Error in controllable:", e)
-        student1 = None
-    print("Master solution:")
-    solution1 = actual_sol(A1, B1)
-    print(solution1)
-    passed_tests += 1 if student1 == solution1 else 0
-
-    # Controllable system
-    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]])
-    B2 = np.array([[0], [0], [1], [0]])
-    print("Student solution:")
-    try:
-        student2 = student_sol(A2, B2)
-        print(student2)
-    except Exception as e:
-        print("Error in controllable:", e)
-        student2 = None
-    print("Master solution:")
-    solution2 = actual_sol(A2, B2)
-    print(solution2)
-    passed_tests += 1 if student2 == solution2 else 0
-
-    print("Passed tests:", passed_tests, " out of 2")
-    return passed_tests == 2
-
-
-def test_observable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's observability check with the solution observability check.
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's observability check.
-    - ``actual_sol`` (function): A function that returns the solution observability check.
-    - ``shouldprint`` (bool): A boolean indicating whether to print the observability checks. Default is True.
-
-    Returns:
-    - () -> bool: A boolean indicating whether the student's observability check is equal to the solution observability check.
-    """
-    passed_tests = 0
-
-    # Observable system
-    A1 = np.array([[1, 0], [0, 2]])
-    C1 = np.array([[1, 1]])
-    print("Student solution:")
-    try:
-        student1 = student_sol(A1, C1)
-        print(student1)
-    except Exception as e:
-        print("Error in observable:", e)
-        student1 = None
-    print("Master solution:")
-    solution1 = actual_sol(A1, C1)
-    print(solution1)
-    passed_tests += 1 if student1 == solution1 else 0
-
-    # Unobservable system
-    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]])
-    C2 = np.array([[0, 0, 0, 0]])
-    print("Student solution:")
-    try:
-        student2 = student_sol(A2, C2)
-        print(student2)
-    except Exception as e:
-        print("Error in observable:", e)
-        student2 = None
-    print("Master solution:")
-    solution2 = actual_sol(A2, C2)
-    print(solution2)
-    passed_tests += 1 if student2 == solution2 else 0
-
-    print("Passed tests:", passed_tests, " out of 2")
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+
+def print_nice(state: List[np.ndarray]) -> None:
+    """
+    Prints the state-space matrices in a nice format.
+
+    Parameters:
+    - ``state`` (List[np.ndarray]): A list of state-space matrices.
+    """
+    matrix_names = ["A", "B", "C", "D"]
+    for mat, name in zip(state, matrix_names):
+        print(f"Matrix {name}:")
+        print(np.array2string(mat, precision=3, suppress_small=True))
+        print()
+
+def sol_diagonalize_system(A: np.array, B: np.array, C: np.array, D: np.array) -> tuple[np.array]:
+    """
+    Diagonalizes a linear time-invariant system represented by its state-space matrices.
+
+    Parameters:
+    - ``A`` (np.array): State matrix of the system.
+    - ``B`` (np.array): Input matrix of the system.
+    - ``C`` (np.array): Output matrix of the system.
+    - ``D`` (np.array): Feedthrough matrix of the system.
+
+    Returns:
+    - ``A_tilde`` (np.array): Diagonalized state matrix.
+    - ``B_tilde`` (np.array): Diagonalized input matrix.
+    - ``C_tilde`` (np.array): Diagonalized output matrix.
+    - ``D_tilde`` (np.array): Diagonalized feedthrough matrix.
+    """
+    # Preliminary safety checks
+    D = np.array(D)
+    if not all(isinstance(mat, np.ndarray) for mat in [A, B, C, D]):
+        raise TypeError("All input matrices must be numpy arrays.")
+    if A.shape[0] != A.shape[1]:
+        raise ValueError("Matrix A must be square.")
+
+    # Compute the eigenvalues and eigenvectors of matrix A
+    eigenvalues, eigenvectors = np.linalg.eig(A)
+
+    # Compute the transformed state-space representation
+    # The diagonal matrix A_tilde contains the eigenvalues of A
+    A_tilde = np.diag(eigenvalues)
+    
+    # The input matrix B_tilde is obtained by transforming the input matrix B
+    # using the inverse of the eigenvector matrix
+    B_tilde = np.linalg.inv(eigenvectors) @ B
+    
+    # The output matrix C_tilde is obtained by transforming the output matrix C
+    # using the eigenvector matrix
+    C_tilde = C @ eigenvectors
+    
+    # The feedthrough matrix D_tilde remains the same
+    D_tilde = D
+    
+    return A_tilde, B_tilde, C_tilde, D_tilde
+
+
+def test_diagonalize_system(student_sol: callable, actual_sol: callable, A3: np.array, B3: np.array, C3: np.array, D3: np.array, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's diagonalized system with the solution diagonalized system.
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's diagonalized system.
+    - ``actual_sol`` (function): A function that returns the solution diagonalized system.
+    - ``A3`` (np.array): State matrix of the system.
+    - ``B3`` (np.array): Input matrix of the system.
+    - ``C3`` (np.array): Output matrix of the system.
+    - ``D3`` (np.array): Feedthrough matrix of the system.
+    - ``shouldprint`` (bool): A boolean indicating whether to print the diagonalized systems. Default is True.
+
+    Raises:
+    - AssertionError: If the input matrices are not numpy arrays.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the student's diagonalized system is equal to the solution diagonalized system.
+    """
+    passed_tests = 0
+
+    # Already diagonalized system
+    A1 = np.array([[1, 0], [0, 2]])
+    B1 = np.array([[1], [1]])
+    C1 = np.array([[1, 0]])
+    D1 = np.array([[0]])
+    try:
+        student1 = student_sol(A1, B1, C1, D1)
+    except Exception as e:
+        print("Error in diagonalize_system:", e)
+        student1 = None
+    solution1 = actual_sol(A1, B1, C1, D1)
+    if shouldprint: print("Student 1:")
+    if shouldprint: print_nice(student1)
+    if shouldprint: print("Solution 1:")
+    if shouldprint: print_nice(solution1)
+    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student1, solution1)) else 0
+
+    # Random system
+    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]]);
+    B2 = np.array([[0], [0], [1], [0]])
+    C2 = np.array([1, 0, 0, 0])
+    D2 = np.array([0])
+    try:
+        student2 = student_sol(A2, B2, C2, D2)
+    except Exception as e:
+        print("Error in diagonalize_system:", e)
+        student2 = None
+    solution2 = actual_sol(A2, B2, C2, D2)
+    if shouldprint: print("Student 2:")
+    if shouldprint: print_nice(student2)
+    if shouldprint: print("Solution 2:")
+    if shouldprint: print_nice(solution2)
+    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student2, solution2)) else 0
+
+    # Aircraft System
+    D3 = np.array(D3)
+    try:
+        student3 = student_sol(A3, B3, C3, D3)
+    except Exception as e:
+        print("Error in diagonalize_system:", e)
+        student3 = None
+    solution3 = actual_sol(A3, B3, C3, D3)
+    if shouldprint: print("Student 3:")
+    if shouldprint: print_nice(student3)
+    if shouldprint: print("Solution 3:")
+    if shouldprint: print_nice(solution3)
+    passed_tests += 1 if all(np.allclose(a, b) for a, b in zip(student3, solution3)) else 0
+
+    print("Passed tests:", passed_tests, " out of 3")
+    return passed_tests == 3
+
+
+def sol_controllable(A: np.array, B: np.array) -> bool:
+    """
+    Check the controllability of a system given the state-space representation.
+
+    Parameters:
+    - ``A`` (np.array): The state matrix.
+    - ``B`` (np.array): The input matrix.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the system is controllable.
+    """
+    
+    n = A.shape[0]  # Get the number of rows in matrix A.
+    R = B  # Initialize the controllability matrix R with matrix B, since the first column of R is always B.
+    
+    for i in range(1, n):  # Iterate from 1 to n-1.
+        # Calculate the reachability matrix for each power of A and concatenate it horizontally to R.
+        R = np.hstack((R, np.linalg.matrix_power(A, i) @ B))
+    
+    rank = np.linalg.matrix_rank(R)
+    
+    if rank == A.shape[0]:
+        print(f"The system is controllable with rank {rank}.")
+    else:
+        print(f"The system is not controllable with rank {rank}.")
+    return rank == n
+
+
+def sol_observable(A: np.array, C: np.array) -> None:
+    """
+    Check the observability of a system given the state-space representation.
+
+    Parameters:
+    - ``A`` (np.array): The state matrix.
+    - ``C`` (np.array): The output matrix.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the system is observable.
+    """
+
+    n = A.shape[0]  # Get the number of rows in matrix A.
+    O = C  # Initialize the observability matrix O with matrix C, since the first row of O is always C.
+    
+    """
+    Same as above, maybe show how to extract the first row programmatically (e.g. O = C[0,:])
+    """
+    
+    for i in range(1, n):  # Iterate from 1 to n-1.
+        # Calculate the observability matrix for each power of A and concatenate it vertically to O.
+        O = np.vstack((O, C @ np.linalg.matrix_power(A, i)))
+    
+    rank = np.linalg.matrix_rank(O)
+    
+    if rank == A.shape[0]:
+        print(f"The system is observable with rank {rank}.")
+    else:
+        print(f"The system is not observable with rank {rank}.")
+    return rank == n
+
+
+def test_controllable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's controllability check with the solution controllability check.
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's controllability check.
+    - ``actual_sol`` (function): A function that returns the solution controllability check.
+    - ``shouldprint`` (bool): A boolean indicating whether to print the controllability checks. Default is True.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the student's controllability check is equal to the solution controllability check.
+    """
+    passed_tests = 0
+
+    # Controllable system
+    A1 = np.array([[1, 0], [0, 2]])
+    B1 = np.array([[1], [1]])
+    print("Student solution:")
+    try:
+        student1 = student_sol(A1, B1)
+        print(student1)
+    except Exception as e:
+        print("Error in controllable:", e)
+        student1 = None
+    print("Master solution:")
+    solution1 = actual_sol(A1, B1)
+    print(solution1)
+    passed_tests += 1 if student1 == solution1 else 0
+
+    # Controllable system
+    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]])
+    B2 = np.array([[0], [0], [1], [0]])
+    print("Student solution:")
+    try:
+        student2 = student_sol(A2, B2)
+        print(student2)
+    except Exception as e:
+        print("Error in controllable:", e)
+        student2 = None
+    print("Master solution:")
+    solution2 = actual_sol(A2, B2)
+    print(solution2)
+    passed_tests += 1 if student2 == solution2 else 0
+
+    print("Passed tests:", passed_tests, " out of 2")
+    return passed_tests == 2
+
+
+def test_observable(student_sol: callable, actual_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's observability check with the solution observability check.
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's observability check.
+    - ``actual_sol`` (function): A function that returns the solution observability check.
+    - ``shouldprint`` (bool): A boolean indicating whether to print the observability checks. Default is True.
+
+    Returns:
+    - () -> bool: A boolean indicating whether the student's observability check is equal to the solution observability check.
+    """
+    passed_tests = 0
+
+    # Observable system
+    A1 = np.array([[1, 0], [0, 2]])
+    C1 = np.array([[1, 1]])
+    print("Student solution:")
+    try:
+        student1 = student_sol(A1, C1)
+        print(student1)
+    except Exception as e:
+        print("Error in observable:", e)
+        student1 = None
+    print("Master solution:")
+    solution1 = actual_sol(A1, C1)
+    print(solution1)
+    passed_tests += 1 if student1 == solution1 else 0
+
+    # Unobservable system
+    A2 = np.array([[0, 0, 1, 0], [0, 0, 0, 1], [-2, 1, 0, 0], [1, -1, 0, 0]])
+    C2 = np.array([[0, 0, 0, 0]])
+    print("Student solution:")
+    try:
+        student2 = student_sol(A2, C2)
+        print(student2)
+    except Exception as e:
+        print("Error in observable:", e)
+        student2 = None
+    print("Master solution:")
+    solution2 = actual_sol(A2, C2)
+    print(solution2)
+    passed_tests += 1 if student2 == solution2 else 0
+
+    print("Passed tests:", passed_tests, " out of 2")
     return passed_tests == 2
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/discretization.py` & `cs2solutions-0.8.0/src/cs2solutions/discretization.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,560 +1,560 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-# Plotting Functions
-        
-def plot_helpers() -> None:
-  """
-  This function sets up the plot with appropriate labels and legend.
-  
-  Parameters: 
-   - None
-
-  Returns: 
-   - None
-  """
-  plt.xlabel('Time')
-  plt.ylabel('Output')
-  plt.legend()
-
-
-def plot_step_responses(t_stable_cont: np.array, y_stable_cont: np.array,
-                        t_stable_eulerf: np.array, y_stable_eulerf: np.array,
-                        t_stable_eulerb: np.array, y_stable_eulerb: np.array,
-                        t_stable_tust: np.array, y_stable_tust: np.array,
-                        t_stable_zoh: np.array, y_stable_zoh: np.array) -> None:
-    """
-    This function plots the step responses of a systems using different discretization methods. Plotted: Continuous, Forward Euler, Backward Euler, Tustin, and Zero Order Hold.
-
-    Parameters:
-    - ``t_stable_cont`` (np.array): Time array for the continuous system.
-    - ``y_stable_cont`` (np.array): Output array for the continuous system.
-    - ``t_stable_eulerf`` (np.array): Time array for the Forward Euler system.
-    - ``y_stable_eulerf`` (np.array): Output array for the Forward Euler system.
-    - ``t_stable_eulerb`` (np.array): Time array for the Backward Euler system.
-    - ``y_stable_eulerb`` (np.array): Output array for the Backward Euler system.
-    - ``t_stable_tust`` (np.array): Time array for the Tustin system.
-    - ``y_stable_tust`` (np.array): Output array for the Tustin system.
-    - ``t_stable_zoh`` (np.array): Time array for the Zero Order Hold system.
-    - ``y_stable_zoh`` (np.array): Output array for the Zero Order Hold system.
-
-    Returns:
-    - None
-    """
-    
-    plt.figure(figsize=[24, 16])
-    plt.subplot(3, 2, 1)
-    plt.plot(t_stable_cont, y_stable_cont, label='Continuous System')
-    plt.step(t_stable_eulerf, y_stable_eulerf, label='Forward Euler')
-    plt.step(t_stable_eulerb, y_stable_eulerb, label='Backward Euler')
-    plt.step(t_stable_tust, y_stable_tust, label='Tustin')
-    plt.step(t_stable_zoh, y_stable_zoh, label='Zero Order Hold')
-
-    # Adding labels and title to the plot.
-    
-    plt.title('Step Response Combined')
-    plot_helpers()
-    
-
-    plt.subplot(3, 2, 2)
-    plt.plot(t_stable_cont, y_stable_cont, label='Continuous System', color = 'C0')
-
-    # Adding labels and title to the plot.
-    plt.title('Step Response Continuous')
-    plot_helpers()
-
-
-    plt.subplot(3, 2, 3)
-    plt.step(t_stable_eulerf, y_stable_eulerf, label='Forward Euler', color = 'C1')
-
-    # Adding labels and title to the plot.
-    plt.title('Step Response Forward Euler')
-    plot_helpers()
-
-
-    plt.subplot(3, 2, 4)
-    plt.step(t_stable_eulerb, y_stable_eulerb, label='Backward Euler', color = 'C2')
-
-    # Adding labels and title to the plot.
-    plt.title('Step Response Backward Euler')
-    plot_helpers()
-
-
-    plt.subplot(3, 2, 5)
-    plt.step(t_stable_tust, y_stable_tust, label='Tustin', color = 'C3')
-
-    # Adding labels and title to the plot.
-    plt.title('Step Response Tustin')
-    plot_helpers()
-
-
-    plt.subplot(3, 2, 6)
-    plt.step(t_stable_zoh, y_stable_zoh, label='Zero Order Hold', color = 'C4')
-
-    # Adding labels and title to the plot.
-    plt.title('Step Response Zero Order Hold')
-    plot_helpers()
-
-    return None
-    
-
-def plot_disc_stepresponses(t_cont: np.array, y_cont: np.array,
-              t_eulerf: np.array, y_eulerf: np.array,
-              t_eulerb: np.array, y_eulerb: np.array,
-              t_tust: np.array, y_tust: np.array,
-              t_zoh: np.array, y_zoh: np.array, Ts: float) -> None:
-  """
-  Plots the step responses of a discrete system along with the continuous system.
-  
-  Parameters:
-   - ``t_cont`` (np.array): Time array for the continuous system.
-   - ``y_cont`` (np.array): Output array for the continuous system.
-   - ``t_eulerf`` (np.array): Time array for the forward Euler method.
-   - ``y_eulerf`` (np.array): Output array for the forward Euler method.
-   - ``t_eulerb`` (np.array): Time array for the backward Euler method.
-   - ``y_eulerb`` (np.array): Output array for the backward Euler method.
-   - ``t_tust`` (np.array): Time array for the Tustin method.
-   - ``y_tust`` (np.array): Output array for the Tustin method.
-   - ``t_zoh`` (np.array): Time array for the Zero Order Hold method.
-   - ``y_zoh`` (np.array): Output array for the Zero Order Hold method.
-   - ``Ts`` (float): Sampling time of the discrete system.
-  
-  Returns:
-   - None
-  """
-  plt.figure(figsize=(10, 6))
-  
-  # Inserting initial values for step response plotting
-  t_eulerf = np.insert(np.squeeze(t_eulerf)+Ts,0,0)
-  y_eulerf = np.insert(np.squeeze(y_eulerf), 0, 0)
-  t_eulerb = np.insert(np.squeeze(t_eulerb)+Ts,0,0)
-  y_eulerb = np.insert(np.squeeze(y_eulerb), 0, 0)
-  t_tust = np.insert(np.squeeze(t_tust)+Ts,0,0)
-  y_tust = np.insert(np.squeeze(y_tust), 0, 0)
-  t_zoh = np.insert(np.squeeze(t_zoh)+Ts,0,0)
-  y_zoh = np.insert(np.squeeze(y_zoh), 0, 0)
-  
-  # Plotting the step responses
-  plt.ylim(-50, 50)
-  plt.plot(t_cont, y_cont, label='Continuous System')
-  plt.step(t_eulerf, y_eulerf, label='Forward Euler')
-  plt.step(t_eulerb, y_eulerb, label='Backward Euler')
-  plt.step(t_tust, y_tust, label='Tustin')
-  plt.step(t_zoh, y_zoh, label='Zero Order Hold')
-  plt.title('Discrete Step Response')
-  plt.xlabel('Time (s)')
-  plt.ylabel('Output')
-  plt.legend()
-  plt.show()
-
-  return None
-        
-
-# Exercise 1a: Solutions
-
-def cont_solution (A: np.array, B: np.array, C:np.array, D:np.array) -> Tuple[np.array, np.array]:
-    """
-    Calculates the step response of a continuous-time linear time-invariant system.
-    
-    Parameters:
-     - ``A`` (np.array): State matrix of the system.
-     - ``B`` (np.array): Input matrix of the system.
-     - ``C`` (np.array): Output matrix of the system.
-     - ``D`` (np.array): Direct transmission matrix of the system.
-    
-    Returns:
-     - Tuple[np.array, np.array]: A tuple containing the time values and the corresponding output values of the step response.
-    """
-    
-    sysc = sig.lti(A, B, C, D)
-
-    t_cont, y_cont = sysc.step(T = np.linspace(0, 25, 1000))
-    
-    return [t_cont, y_cont]
-
-def disc_solution(A: np.array, B: np.array, C: np.array, D: np.array, Ts: float) -> Tuple[np.array, np.array, np.array, np.array, np.array, np.array, np.array, np.array]:
-    """
-    Calculates the discrete-time step response using different methods.
-
-    Parameters:
-     - ``A`` (np.array): State matrix of the continuous-time system.
-     - ``B`` (np.array): Input matrix of the continuous-time system.
-     - ``C`` (np.array): Output matrix of the continuous-time system.
-     - ``D`` (np.array): Feedthrough matrix of the continuous-time system.
-     - ``Ts`` (float): Sampling time.
-
-    Returns:
-    Tuple[np.array, np.array, np.array, np.array, np.array, np.array, np.array, np.array]: A tuple containing the time and output arrays for each method:
-        - ``t_eulerf``: Time array for the forward Euler method.
-        - ``y_eulerf``: Output array for the forward Euler method.
-        - ``t_eulerb``: Time array for the backward difference method.
-        - ``y_eulerb``: Output array for the backward difference method.
-        - ``t_tust``: Time array for the Tustin method.
-        - ``y_tust``: Output array for the Tustin method.
-        - ``t_zoh``: Time array for the zero-order hold method.
-        - ``y_zoh``: Output array for the zero-order hold method.
-    """
-        
-    sysd_eulerf = sig.cont2discrete((A, B, C, D), Ts, method='euler')
-    t_eulerf, y_eulerf = sig.dstep(sysd_eulerf, t=np.arange(0, 25, Ts))
-
-    sysd_eulerb = sig.cont2discrete((A, B, C, D), Ts, method='backward_diff')
-    t_eulerb, y_eulerb = sig.dstep(sysd_eulerb, t=np.arange(0, 25, Ts))
-
-    sysd_tust = sig.cont2discrete((A, B, C, D), Ts, method='bilinear')
-    t_tust, y_tust = sig.dstep(sysd_tust, t=np.arange(0, 25, Ts))
-
-    sysd_zoh = sig.cont2discrete((A, B, C, D), Ts, method='zoh')
-    t_zoh, y_zoh = sig.dstep(sysd_zoh, t=np.arange(0, 25, Ts))
-    
-    return [t_eulerf, y_eulerf, t_eulerb, y_eulerb, t_tust, y_tust, t_zoh, y_zoh]
-
-
-# Ackermann's Formula
-
-def feedforward_kr(A: np.array, B: np.array, C: np.array, K: np.array) -> np.array:
-    """
-    Calculates the feedforward gain (kr) for a given system.
-
-    Parameters:
-     - ``A`` (np.array): The state matrix of the system.
-     - ``B`` (np.array): The input matrix of the system.
-     - ``C`` (np.array): The output matrix of the system.
-     - ``K`` (np.array): The feedback gain matrix of the system.
-
-    Returns:
-     - ``kr`` (np.array): The feedforward gain (kr) of the system.
-    """
-
-    ABK = A - B @ K
-    ABK_inv = np.linalg.inv(ABK)
-    den = C @ ABK_inv @ B
-    kr = - 1/den
-
-    return kr
-
-
-def acker(A: np.array, B: np.array, poles: List[float]) -> np.array:
-    """
-    Calculates the state feedback gain matrix K using the Ackermann's formula.
-
-    Parameters:
-     - ``A`` (np.array): State matrix of the system.
-     - ``B`` (np.array): Input matrix of the system.
-     - ``poles`` (List[float]): List of desired closed-loop poles.
-
-    Returns:
-     - ``K`` (np.array): State feedback gain matrix K.
-    """
-
-    AB = A @ B
-    R = np.concatenate((B, AB), axis=1)
-    R_inv = np.linalg.inv(R)
-    gamma = np.array([[0, 1]]) @ R_inv
-
-    p_1 = poles[0]*(-1)
-    p_2 = poles[1]*(-1)
-    ab = p_1 + p_2
-    b = p_1*p_2
-    p_cl = A @ A + ab*A + b*np.identity(2)
-
-    K = gamma @ p_cl
-
-    return K
-
-
-def place_poles_Ackermann(A: np.array, B: np.array, C: np.array,
-                          D: float, poles: List) -> np.array:
-    """
-    Computes the controller gains and closed loop system dynamics using the Ackermann method
-    to place the poles of the system at desired locations.
-    
-    Parameters:
-     - ``A`` (np.array): State matrix of the system.
-     - ``B`` (np.array): Input matrix of the system.
-     - ``C`` (np.array): Output matrix of the system.
-     - ``D`` (float): Direct transmission matrix of the system.
-     - ``poles`` (List): List of desired pole locations.
-        
-    Returns:
-     - ``clsys`` (np.array): Updated system dynamics using new poles and feedforward gain.
-    """
-    
-    K=ct.acker(A, B, poles)
-    
-    # Create a new system representing the closed loop response.
-    clsys = ct.StateSpace(A - B @ K, B, C, D)
-
-    # Compute the feedforward gain.
-    kr = feedforward_kr(A, B, C, K)
-    
-    # Scale the input by the feedforward gain.
-    clsys *= kr
-
-    # Return gains and closed loop system dynamics.
-    return clsys
-
-
-# CURRENTLY UNABLE TO UPDATE ACKERMANN!
-
-
-# Discretization Functions
-
-def euler_forward(system, dt) -> ct.StateSpace:
-    """
-    Discretize a continuous-time system using the Euler forward method.
-
-    Parameters:
-     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
-     - ``dt`` (float): Time step for discretization.
-
-    Returns:
-     - StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
-    """
-    A, B, C, D = system.A, system.B, system.C, system.D
-    I = np.eye(A.shape[0])
-    Ad = I + dt * A
-    Bd = dt * B
-    Cd = C
-    Dd = D
-    return ct.StateSpace(Ad, Bd, Cd, Dd)
-
-
-def euler_backward(system, dt) -> ct.StateSpace:
-    """
-    Discretize a continuous-time system using the Euler backward method.
-
-    Parameters:
-     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
-     - ``dt`` (float): Time step for discretization.
-
-    Returns:
-     -   StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
-    """
-    A, B, C, D = system.A, system.B, system.C, system.D
-    I = np.eye(A.shape[0])
-    Ad = np.linalg.inv(I - dt * A)
-    Bd = np.dot(Ad, dt * B)
-    Cd = C
-    Dd = D
-    return ct.StateSpace(Ad, Bd, Cd, Dd)
-
-
-def tustin_method(system, dt) -> ct.StateSpace:
-    """
-    Discretize a continuous-time system using Tustin's method (bilinear transformation).
-    
-    Parameters:
-     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
-     - ``dt`` (float): Time step for discretization.
-    
-    Returns:
-     - StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
-    """
-    A, B, C, D = system.A, system.B, system.C, system.D
-    I = np.eye(A.shape[0])
-    pre_matrix = np.linalg.inv(I - (dt / 2) * A)
-    Ad = np.dot(pre_matrix, I + (dt / 2) * A)
-    Bd = np.dot(pre_matrix, dt * B)
-    Cd = C
-    Dd = D
-    return ct.StateSpace(Ad, Bd, Cd, Dd)
-
-
-def discretize(system: ct.StateSpace, dt: float) -> Tuple[ct.StateSpace, ct.StateSpace, ct.StateSpace]:
-    """
-    Discretizes a continuous-time system into discrete-time systems using three methods: 
-    Euler Forward, Euler Backward, and Tustin's method.
-
-    Parameters:
-     - ``system`` (ct.StateSpace): A continuous-time system represented as a ct.StateSpace object.
-     - ``dt`` (float): Time step for discretization.
-
-    Returns:
-     - Tuple[ct.StateSpace, ct.StateSpace, ct.StateSpace]: A tuple of discretized systems (dt_forward, dt_backward, dt_tustin), each representing 
-              the input system discretized using Euler Forward, Euler Backward, and Tustin's method, respectively.
-    """
-    # Discretize using each method
-    dt_forward = euler_forward(system, dt)
-    dt_backward = euler_backward(system, dt)
-    dt_tustin = tustin_method(system, dt)
-    
-    return dt_forward, dt_backward, dt_tustin
-
-
-def plot_eigenvalues(system, method_name):
-        """
-        Plots the eigenvalues of the discretized system's A matrix on the complex plane.
-
-        Parameters:
-         - ``system`` (ct.StateSpace): A discrete-time system represented as a ct.StateSpace object, 
-                                                          whose eigenvalues are to be plotted.
-         - ``method_name`` (str): The name of the discretization method used for this system. 
-                                                  This name is used as a label in the plot.
-
-        Returns:
-         - None
-
-        The function calculates the eigenvalues of the system's A matrix, prints them,
-        and plots them on the complex plane. Each set of eigenvalues is labeled according 
-        to the discretization method used.
-        """
-        Ad = system.A
-        eigenvalues = np.linalg.eigvals(Ad)
-        print("Eigenvalues using " + method_name)
-        print(eigenvalues)
-        print("Magnitude")
-        print(np.linalg.norm(eigenvalues[0]))
-        print("\n")
-
-        plt.scatter(eigenvalues.real, eigenvalues.imag, label=method_name)
-
-        return None
-
-
-def plot_table(dt_forward, dt_backward, dt_tustin):
-    """
-    Plots the eigenvalues of three discretized systems on the complex plane to compare their stability.
-
-    Parameters:
-     - ``dt_forward`` (ct.StateSpace): Discretized system using the Euler Forward method (StateSpace object).
-     - ``dt_backward`` (ct.StateSpace): Discretized system using the Euler Backward method (StateSpace object).
-     - ``dt_tustin`` (ct.StateSpace): Discretized system using Tustin's method (StateSpace object).
-
-    This function visualizes the eigenvalues of the given discretized systems on the complex plane.
-    It helps in comparing the stability characteristics of the systems discretized using different methods.
-    The function plots each set of eigenvalues with a different label corresponding to the discretization method.
-    It also includes a unit circle for reference, aiding in the assessment of stability (eigenvalues inside the 
-    unit circle indicate stability in discrete-time systems).
-
-    Returns:
-     - None
-    """
-    plt.figure(figsize=(8, 6))
-    
-    plot_eigenvalues(dt_forward, 'Euler Forward')
-    plot_eigenvalues(dt_backward, 'Euler Backward')
-    plot_eigenvalues(dt_tustin, 'Tustin')
-    
-    plt.axhline(y=0, color='k')
-    plt.axvline(x=0, color='k')
-    plt.xlabel('Real Part')
-    plt.ylabel('Imaginary Part')
-    plt.title('Eigenvalues of Discretized Systems')
-    plt.legend(loc='upper right', bbox_to_anchor=(1.15, 1.15))
-    plt.grid(True)
-
-    # adding unit circle for visualization
-    theta = np.linspace(0, 2 * np.pi, 100)  # 100 points between 0 and 2*pi
-    x = np.cos(theta)  # x coordinates on the circle
-    y = np.sin(theta)  # y coordinates on the circle
-    plt.plot(x, y, linestyle='--', color='grey')
-
-    plt.show()
-
-    return None
-
-
-def simulate_step_response(system, dt, label, n=100):
-    """
-    Simulates and plots the step response of a discretized system.
-
-    Parameters:
-     - ``system`` (ct.StateSpace): A StateSpace object representing the discretized system.
-     - ``dt`` (float): The sampling time step used for the discretization.
-     - ``label`` (str): A string label to identify the step response in the plot.
-     - ``n`` (int): The number of time steps to simulate (default is 100).
-
-    This function calculates the step response of a given discretized system using the provided time step (dt) over 'n' time steps. 
-    It then plots the response using matplotlib, labeling the plot with the given label for easy identification. 
-    The step response is visualized using a step plot, which shows how the system's output evolves over time in response to a unit step input.
-
-    Returns:
-     - None
-    """
-    lti = sig.dlti(system.A, system.B, system.C, system.D, dt=dt)
-    t, y = sig.dstep(lti, n=n)
-    plt.step(t, np.squeeze(y), label=label)
-
-    return None
-
-
-# Exercise 1b: Test Ackermann + Discretization
-
-def test_ackermann_discrete(A: np.array, 
-                              B: np.array, 
-                              C: np.array,
-                              D: np.array, 
-                              p_des: Tuple[complex, complex] = [-0.5+3j, -0.5-3j], 
-                              Ts: float = 0.25) -> None:
-    """
-    Test the user's implementations of the closed-loop system dynamics and step response calculations.
-
-    This function computes the closed-loop system dynamics using Ackermann's formula and
-    calculates the step response of both the continuous and discrete closed-loop systems
-    using different discretization schemes. It then plots the step responses.
-
-    Parameters:
-     - ``A`` (np.array): numpy array representing the system matrix A.
-     - ``B`` (np.array): numpy array representing the input matrix B.
-     - ``C`` (np.array): numpy array representing the output matrix C.
-     - ``D`` (np.array): float representing the direct transmission matrix D.
-     - ``p_des`` (List[complex, complex]): List of complex numbers representing the desired poles of the closed-loop system. Default value is [-0.5+3j, -0.5-3j].
-     - ``Ts`` (float): float representing the sampling time for the discrete closed-loop system. Default value is 0.25.
-
-    Returns:
-     - None
-    """
-
-    # Compute the closed loop system dynamics using Ackermann's formula.
-    clsys_p = place_poles_Ackermann(A=A, B=B, C=C, D=0,
-                                        poles=p_des)
-    t_p, y_p = ct.step_response(clsys_p, input=0, output=0)
-
-    # Define the system matrices and sampling time
-    A_stable = clsys_p.A
-    B_stable = clsys_p.B
-    C_stable = clsys_p.C
-    D_stable = clsys_p.D
-
-
-
-    # Compute the step response of the continuous closed loop system. 
-    # If you couldn't solve the previous exercise, you can use the solution. For that replace the function call with the following:
-    # [t_stable_cont, y_stable_cont] = cont_solution(A_stable, B_stable, C_stable, D_stable)
-    t_stable_cont, y_stable_cont = continuous_step_response(A_stable, B_stable, C_stable, D_stable)
-
-
-
-    # Compute the step response of the discrete closed loop system using the different discretization schemes. 
-    # If you couldn't solve the previous exercise, you can use the solution. For that replace the function call with the following:
-    # [t_stable_eulerf, y_stable_eulerf, t_stable_eulerb, y_stable_eulerb, t_stable_tust, y_stable_tust, t_stable_zoh, y_stable_zoh] = disc_solution(A_stable, B_stable, C_stable, D_stable, Ts)
-    t_stable_eulerf, y_stable_eulerf = discrete_step_response_euler_forward(A_stable, B_stable, C_stable, D_stable, Ts)
-    t_stable_eulerb, y_stable_eulerb = discrete_step_response_euler_backward(A_stable, B_stable, C_stable, D_stable, Ts)
-    t_stable_tust, y_stable_tust = discrete_step_response_tustin(A_stable, B_stable, C_stable, D_stable, Ts)
-    t_stable_zoh, y_stable_zoh = discrete_step_response_zoh(A_stable, B_stable, C_stable, D_stable, Ts)
-
-
-
-    # Package the results for plotting.
-    values_to_plot = [t_stable_cont, y_stable_cont,
-                    t_stable_eulerf, y_stable_eulerf,
-                    t_stable_eulerb, y_stable_eulerb,
-                    t_stable_tust, y_stable_tust,
-                    t_stable_zoh, y_stable_zoh]
-
-    # Plot the step responses.
-    plot_step_responses(*values_to_plot)
-
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+# Plotting Functions
+        
+def plot_helpers() -> None:
+  """
+  This function sets up the plot with appropriate labels and legend.
+  
+  Parameters: 
+   - None
+
+  Returns: 
+   - None
+  """
+  plt.xlabel('Time')
+  plt.ylabel('Output')
+  plt.legend()
+
+
+def plot_step_responses(t_stable_cont: np.array, y_stable_cont: np.array,
+                        t_stable_eulerf: np.array, y_stable_eulerf: np.array,
+                        t_stable_eulerb: np.array, y_stable_eulerb: np.array,
+                        t_stable_tust: np.array, y_stable_tust: np.array,
+                        t_stable_zoh: np.array, y_stable_zoh: np.array) -> None:
+    """
+    This function plots the step responses of a systems using different discretization methods. Plotted: Continuous, Forward Euler, Backward Euler, Tustin, and Zero Order Hold.
+
+    Parameters:
+    - ``t_stable_cont`` (np.array): Time array for the continuous system.
+    - ``y_stable_cont`` (np.array): Output array for the continuous system.
+    - ``t_stable_eulerf`` (np.array): Time array for the Forward Euler system.
+    - ``y_stable_eulerf`` (np.array): Output array for the Forward Euler system.
+    - ``t_stable_eulerb`` (np.array): Time array for the Backward Euler system.
+    - ``y_stable_eulerb`` (np.array): Output array for the Backward Euler system.
+    - ``t_stable_tust`` (np.array): Time array for the Tustin system.
+    - ``y_stable_tust`` (np.array): Output array for the Tustin system.
+    - ``t_stable_zoh`` (np.array): Time array for the Zero Order Hold system.
+    - ``y_stable_zoh`` (np.array): Output array for the Zero Order Hold system.
+
+    Returns:
+    - None
+    """
+    
+    plt.figure(figsize=[24, 16])
+    plt.subplot(3, 2, 1)
+    plt.plot(t_stable_cont, y_stable_cont, label='Continuous System')
+    plt.step(t_stable_eulerf, y_stable_eulerf, label='Forward Euler')
+    plt.step(t_stable_eulerb, y_stable_eulerb, label='Backward Euler')
+    plt.step(t_stable_tust, y_stable_tust, label='Tustin')
+    plt.step(t_stable_zoh, y_stable_zoh, label='Zero Order Hold')
+
+    # Adding labels and title to the plot.
+    
+    plt.title('Step Response Combined')
+    plot_helpers()
+    
+
+    plt.subplot(3, 2, 2)
+    plt.plot(t_stable_cont, y_stable_cont, label='Continuous System', color = 'C0')
+
+    # Adding labels and title to the plot.
+    plt.title('Step Response Continuous')
+    plot_helpers()
+
+
+    plt.subplot(3, 2, 3)
+    plt.step(t_stable_eulerf, y_stable_eulerf, label='Forward Euler', color = 'C1')
+
+    # Adding labels and title to the plot.
+    plt.title('Step Response Forward Euler')
+    plot_helpers()
+
+
+    plt.subplot(3, 2, 4)
+    plt.step(t_stable_eulerb, y_stable_eulerb, label='Backward Euler', color = 'C2')
+
+    # Adding labels and title to the plot.
+    plt.title('Step Response Backward Euler')
+    plot_helpers()
+
+
+    plt.subplot(3, 2, 5)
+    plt.step(t_stable_tust, y_stable_tust, label='Tustin', color = 'C3')
+
+    # Adding labels and title to the plot.
+    plt.title('Step Response Tustin')
+    plot_helpers()
+
+
+    plt.subplot(3, 2, 6)
+    plt.step(t_stable_zoh, y_stable_zoh, label='Zero Order Hold', color = 'C4')
+
+    # Adding labels and title to the plot.
+    plt.title('Step Response Zero Order Hold')
+    plot_helpers()
+
+    return None
+    
+
+def plot_disc_stepresponses(t_cont: np.array, y_cont: np.array,
+              t_eulerf: np.array, y_eulerf: np.array,
+              t_eulerb: np.array, y_eulerb: np.array,
+              t_tust: np.array, y_tust: np.array,
+              t_zoh: np.array, y_zoh: np.array, Ts: float) -> None:
+  """
+  Plots the step responses of a discrete system along with the continuous system.
+  
+  Parameters:
+   - ``t_cont`` (np.array): Time array for the continuous system.
+   - ``y_cont`` (np.array): Output array for the continuous system.
+   - ``t_eulerf`` (np.array): Time array for the forward Euler method.
+   - ``y_eulerf`` (np.array): Output array for the forward Euler method.
+   - ``t_eulerb`` (np.array): Time array for the backward Euler method.
+   - ``y_eulerb`` (np.array): Output array for the backward Euler method.
+   - ``t_tust`` (np.array): Time array for the Tustin method.
+   - ``y_tust`` (np.array): Output array for the Tustin method.
+   - ``t_zoh`` (np.array): Time array for the Zero Order Hold method.
+   - ``y_zoh`` (np.array): Output array for the Zero Order Hold method.
+   - ``Ts`` (float): Sampling time of the discrete system.
+  
+  Returns:
+   - None
+  """
+  plt.figure(figsize=(10, 6))
+  
+  # Inserting initial values for step response plotting
+  t_eulerf = np.insert(np.squeeze(t_eulerf)+Ts,0,0)
+  y_eulerf = np.insert(np.squeeze(y_eulerf), 0, 0)
+  t_eulerb = np.insert(np.squeeze(t_eulerb)+Ts,0,0)
+  y_eulerb = np.insert(np.squeeze(y_eulerb), 0, 0)
+  t_tust = np.insert(np.squeeze(t_tust)+Ts,0,0)
+  y_tust = np.insert(np.squeeze(y_tust), 0, 0)
+  t_zoh = np.insert(np.squeeze(t_zoh)+Ts,0,0)
+  y_zoh = np.insert(np.squeeze(y_zoh), 0, 0)
+  
+  # Plotting the step responses
+  plt.ylim(-50, 50)
+  plt.plot(t_cont, y_cont, label='Continuous System')
+  plt.step(t_eulerf, y_eulerf, label='Forward Euler')
+  plt.step(t_eulerb, y_eulerb, label='Backward Euler')
+  plt.step(t_tust, y_tust, label='Tustin')
+  plt.step(t_zoh, y_zoh, label='Zero Order Hold')
+  plt.title('Discrete Step Response')
+  plt.xlabel('Time (s)')
+  plt.ylabel('Output')
+  plt.legend()
+  plt.show()
+
+  return None
+        
+
+# Exercise 1a: Solutions
+
+def cont_solution (A: np.array, B: np.array, C:np.array, D:np.array) -> Tuple[np.array, np.array]:
+    """
+    Calculates the step response of a continuous-time linear time-invariant system.
+    
+    Parameters:
+     - ``A`` (np.array): State matrix of the system.
+     - ``B`` (np.array): Input matrix of the system.
+     - ``C`` (np.array): Output matrix of the system.
+     - ``D`` (np.array): Direct transmission matrix of the system.
+    
+    Returns:
+     - Tuple[np.array, np.array]: A tuple containing the time values and the corresponding output values of the step response.
+    """
+    
+    sysc = sig.lti(A, B, C, D)
+
+    t_cont, y_cont = sysc.step(T = np.linspace(0, 25, 1000))
+    
+    return [t_cont, y_cont]
+
+def disc_solution(A: np.array, B: np.array, C: np.array, D: np.array, Ts: float) -> Tuple[np.array, np.array, np.array, np.array, np.array, np.array, np.array, np.array]:
+    """
+    Calculates the discrete-time step response using different methods.
+
+    Parameters:
+     - ``A`` (np.array): State matrix of the continuous-time system.
+     - ``B`` (np.array): Input matrix of the continuous-time system.
+     - ``C`` (np.array): Output matrix of the continuous-time system.
+     - ``D`` (np.array): Feedthrough matrix of the continuous-time system.
+     - ``Ts`` (float): Sampling time.
+
+    Returns:
+    Tuple[np.array, np.array, np.array, np.array, np.array, np.array, np.array, np.array]: A tuple containing the time and output arrays for each method:
+        - ``t_eulerf``: Time array for the forward Euler method.
+        - ``y_eulerf``: Output array for the forward Euler method.
+        - ``t_eulerb``: Time array for the backward difference method.
+        - ``y_eulerb``: Output array for the backward difference method.
+        - ``t_tust``: Time array for the Tustin method.
+        - ``y_tust``: Output array for the Tustin method.
+        - ``t_zoh``: Time array for the zero-order hold method.
+        - ``y_zoh``: Output array for the zero-order hold method.
+    """
+        
+    sysd_eulerf = sig.cont2discrete((A, B, C, D), Ts, method='euler')
+    t_eulerf, y_eulerf = sig.dstep(sysd_eulerf, t=np.arange(0, 25, Ts))
+
+    sysd_eulerb = sig.cont2discrete((A, B, C, D), Ts, method='backward_diff')
+    t_eulerb, y_eulerb = sig.dstep(sysd_eulerb, t=np.arange(0, 25, Ts))
+
+    sysd_tust = sig.cont2discrete((A, B, C, D), Ts, method='bilinear')
+    t_tust, y_tust = sig.dstep(sysd_tust, t=np.arange(0, 25, Ts))
+
+    sysd_zoh = sig.cont2discrete((A, B, C, D), Ts, method='zoh')
+    t_zoh, y_zoh = sig.dstep(sysd_zoh, t=np.arange(0, 25, Ts))
+    
+    return [t_eulerf, y_eulerf, t_eulerb, y_eulerb, t_tust, y_tust, t_zoh, y_zoh]
+
+
+# Ackermann's Formula
+
+def feedforward_kr(A: np.array, B: np.array, C: np.array, K: np.array) -> np.array:
+    """
+    Calculates the feedforward gain (kr) for a given system.
+
+    Parameters:
+     - ``A`` (np.array): The state matrix of the system.
+     - ``B`` (np.array): The input matrix of the system.
+     - ``C`` (np.array): The output matrix of the system.
+     - ``K`` (np.array): The feedback gain matrix of the system.
+
+    Returns:
+     - ``kr`` (np.array): The feedforward gain (kr) of the system.
+    """
+
+    ABK = A - B @ K
+    ABK_inv = np.linalg.inv(ABK)
+    den = C @ ABK_inv @ B
+    kr = - 1/den
+
+    return kr
+
+
+def acker(A: np.array, B: np.array, poles: List[float]) -> np.array:
+    """
+    Calculates the state feedback gain matrix K using the Ackermann's formula.
+
+    Parameters:
+     - ``A`` (np.array): State matrix of the system.
+     - ``B`` (np.array): Input matrix of the system.
+     - ``poles`` (List[float]): List of desired closed-loop poles.
+
+    Returns:
+     - ``K`` (np.array): State feedback gain matrix K.
+    """
+
+    AB = A @ B
+    R = np.concatenate((B, AB), axis=1)
+    R_inv = np.linalg.inv(R)
+    gamma = np.array([[0, 1]]) @ R_inv
+
+    p_1 = poles[0]*(-1)
+    p_2 = poles[1]*(-1)
+    ab = p_1 + p_2
+    b = p_1*p_2
+    p_cl = A @ A + ab*A + b*np.identity(2)
+
+    K = gamma @ p_cl
+
+    return K
+
+
+def place_poles_Ackermann(A: np.array, B: np.array, C: np.array,
+                          D: float, poles: List) -> np.array:
+    """
+    Computes the controller gains and closed loop system dynamics using the Ackermann method
+    to place the poles of the system at desired locations.
+    
+    Parameters:
+     - ``A`` (np.array): State matrix of the system.
+     - ``B`` (np.array): Input matrix of the system.
+     - ``C`` (np.array): Output matrix of the system.
+     - ``D`` (float): Direct transmission matrix of the system.
+     - ``poles`` (List): List of desired pole locations.
+        
+    Returns:
+     - ``clsys`` (np.array): Updated system dynamics using new poles and feedforward gain.
+    """
+    
+    K=ct.acker(A, B, poles)
+    
+    # Create a new system representing the closed loop response.
+    clsys = ct.StateSpace(A - B @ K, B, C, D)
+
+    # Compute the feedforward gain.
+    kr = feedforward_kr(A, B, C, K)
+    
+    # Scale the input by the feedforward gain.
+    clsys *= kr
+
+    # Return gains and closed loop system dynamics.
+    return clsys
+
+
+# CURRENTLY UNABLE TO UPDATE ACKERMANN!
+
+
+# Discretization Functions
+
+def euler_forward(system, dt) -> ct.StateSpace:
+    """
+    Discretize a continuous-time system using the Euler forward method.
+
+    Parameters:
+     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
+     - ``dt`` (float): Time step for discretization.
+
+    Returns:
+     - StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
+    """
+    A, B, C, D = system.A, system.B, system.C, system.D
+    I = np.eye(A.shape[0])
+    Ad = I + dt * A
+    Bd = dt * B
+    Cd = C
+    Dd = D
+    return ct.StateSpace(Ad, Bd, Cd, Dd)
+
+
+def euler_backward(system, dt) -> ct.StateSpace:
+    """
+    Discretize a continuous-time system using the Euler backward method.
+
+    Parameters:
+     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
+     - ``dt`` (float): Time step for discretization.
+
+    Returns:
+     -   StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
+    """
+    A, B, C, D = system.A, system.B, system.C, system.D
+    I = np.eye(A.shape[0])
+    Ad = np.linalg.inv(I - dt * A)
+    Bd = np.dot(Ad, dt * B)
+    Cd = C
+    Dd = D
+    return ct.StateSpace(Ad, Bd, Cd, Dd)
+
+
+def tustin_method(system, dt) -> ct.StateSpace:
+    """
+    Discretize a continuous-time system using Tustin's method (bilinear transformation).
+    
+    Parameters:
+     - ``system`` (ct.StateSpace): State-space system (instance of ct.StateSpace).
+     - ``dt`` (float): Time step for discretization.
+    
+    Returns:
+     - StateSpace(Ad, Bd, Cd, Dd): Discretized state-space matrices.
+    """
+    A, B, C, D = system.A, system.B, system.C, system.D
+    I = np.eye(A.shape[0])
+    pre_matrix = np.linalg.inv(I - (dt / 2) * A)
+    Ad = np.dot(pre_matrix, I + (dt / 2) * A)
+    Bd = np.dot(pre_matrix, dt * B)
+    Cd = C
+    Dd = D
+    return ct.StateSpace(Ad, Bd, Cd, Dd)
+
+
+def discretize(system: ct.StateSpace, dt: float) -> Tuple[ct.StateSpace, ct.StateSpace, ct.StateSpace]:
+    """
+    Discretizes a continuous-time system into discrete-time systems using three methods: 
+    Euler Forward, Euler Backward, and Tustin's method.
+
+    Parameters:
+     - ``system`` (ct.StateSpace): A continuous-time system represented as a ct.StateSpace object.
+     - ``dt`` (float): Time step for discretization.
+
+    Returns:
+     - Tuple[ct.StateSpace, ct.StateSpace, ct.StateSpace]: A tuple of discretized systems (dt_forward, dt_backward, dt_tustin), each representing 
+              the input system discretized using Euler Forward, Euler Backward, and Tustin's method, respectively.
+    """
+    # Discretize using each method
+    dt_forward = euler_forward(system, dt)
+    dt_backward = euler_backward(system, dt)
+    dt_tustin = tustin_method(system, dt)
+    
+    return dt_forward, dt_backward, dt_tustin
+
+
+def plot_eigenvalues(system, method_name):
+        """
+        Plots the eigenvalues of the discretized system's A matrix on the complex plane.
+
+        Parameters:
+         - ``system`` (ct.StateSpace): A discrete-time system represented as a ct.StateSpace object, 
+                                                          whose eigenvalues are to be plotted.
+         - ``method_name`` (str): The name of the discretization method used for this system. 
+                                                  This name is used as a label in the plot.
+
+        Returns:
+         - None
+
+        The function calculates the eigenvalues of the system's A matrix, prints them,
+        and plots them on the complex plane. Each set of eigenvalues is labeled according 
+        to the discretization method used.
+        """
+        Ad = system.A
+        eigenvalues = np.linalg.eigvals(Ad)
+        print("Eigenvalues using " + method_name)
+        print(eigenvalues)
+        print("Magnitude")
+        print(np.linalg.norm(eigenvalues[0]))
+        print("\n")
+
+        plt.scatter(eigenvalues.real, eigenvalues.imag, label=method_name)
+
+        return None
+
+
+def plot_table(dt_forward, dt_backward, dt_tustin):
+    """
+    Plots the eigenvalues of three discretized systems on the complex plane to compare their stability.
+
+    Parameters:
+     - ``dt_forward`` (ct.StateSpace): Discretized system using the Euler Forward method (StateSpace object).
+     - ``dt_backward`` (ct.StateSpace): Discretized system using the Euler Backward method (StateSpace object).
+     - ``dt_tustin`` (ct.StateSpace): Discretized system using Tustin's method (StateSpace object).
+
+    This function visualizes the eigenvalues of the given discretized systems on the complex plane.
+    It helps in comparing the stability characteristics of the systems discretized using different methods.
+    The function plots each set of eigenvalues with a different label corresponding to the discretization method.
+    It also includes a unit circle for reference, aiding in the assessment of stability (eigenvalues inside the 
+    unit circle indicate stability in discrete-time systems).
+
+    Returns:
+     - None
+    """
+    plt.figure(figsize=(8, 6))
+    
+    plot_eigenvalues(dt_forward, 'Euler Forward')
+    plot_eigenvalues(dt_backward, 'Euler Backward')
+    plot_eigenvalues(dt_tustin, 'Tustin')
+    
+    plt.axhline(y=0, color='k')
+    plt.axvline(x=0, color='k')
+    plt.xlabel('Real Part')
+    plt.ylabel('Imaginary Part')
+    plt.title('Eigenvalues of Discretized Systems')
+    plt.legend(loc='upper right', bbox_to_anchor=(1.15, 1.15))
+    plt.grid(True)
+
+    # adding unit circle for visualization
+    theta = np.linspace(0, 2 * np.pi, 100)  # 100 points between 0 and 2*pi
+    x = np.cos(theta)  # x coordinates on the circle
+    y = np.sin(theta)  # y coordinates on the circle
+    plt.plot(x, y, linestyle='--', color='grey')
+
+    plt.show()
+
+    return None
+
+
+def simulate_step_response(system, dt, label, n=100):
+    """
+    Simulates and plots the step response of a discretized system.
+
+    Parameters:
+     - ``system`` (ct.StateSpace): A StateSpace object representing the discretized system.
+     - ``dt`` (float): The sampling time step used for the discretization.
+     - ``label`` (str): A string label to identify the step response in the plot.
+     - ``n`` (int): The number of time steps to simulate (default is 100).
+
+    This function calculates the step response of a given discretized system using the provided time step (dt) over 'n' time steps. 
+    It then plots the response using matplotlib, labeling the plot with the given label for easy identification. 
+    The step response is visualized using a step plot, which shows how the system's output evolves over time in response to a unit step input.
+
+    Returns:
+     - None
+    """
+    lti = sig.dlti(system.A, system.B, system.C, system.D, dt=dt)
+    t, y = sig.dstep(lti, n=n)
+    plt.step(t, np.squeeze(y), label=label)
+
+    return None
+
+
+# Exercise 1b: Test Ackermann + Discretization
+
+def test_ackermann_discrete(A: np.array, 
+                              B: np.array, 
+                              C: np.array,
+                              D: np.array, 
+                              p_des: Tuple[complex, complex] = [-0.5+3j, -0.5-3j], 
+                              Ts: float = 0.25) -> None:
+    """
+    Test the user's implementations of the closed-loop system dynamics and step response calculations.
+
+    This function computes the closed-loop system dynamics using Ackermann's formula and
+    calculates the step response of both the continuous and discrete closed-loop systems
+    using different discretization schemes. It then plots the step responses.
+
+    Parameters:
+     - ``A`` (np.array): numpy array representing the system matrix A.
+     - ``B`` (np.array): numpy array representing the input matrix B.
+     - ``C`` (np.array): numpy array representing the output matrix C.
+     - ``D`` (np.array): float representing the direct transmission matrix D.
+     - ``p_des`` (List[complex, complex]): List of complex numbers representing the desired poles of the closed-loop system. Default value is [-0.5+3j, -0.5-3j].
+     - ``Ts`` (float): float representing the sampling time for the discrete closed-loop system. Default value is 0.25.
+
+    Returns:
+     - None
+    """
+
+    # Compute the closed loop system dynamics using Ackermann's formula.
+    clsys_p = place_poles_Ackermann(A=A, B=B, C=C, D=0,
+                                        poles=p_des)
+    t_p, y_p = ct.step_response(clsys_p, input=0, output=0)
+
+    # Define the system matrices and sampling time
+    A_stable = clsys_p.A
+    B_stable = clsys_p.B
+    C_stable = clsys_p.C
+    D_stable = clsys_p.D
+
+
+
+    # Compute the step response of the continuous closed loop system. 
+    # If you couldn't solve the previous exercise, you can use the solution. For that replace the function call with the following:
+    # [t_stable_cont, y_stable_cont] = cont_solution(A_stable, B_stable, C_stable, D_stable)
+    t_stable_cont, y_stable_cont = continuous_step_response(A_stable, B_stable, C_stable, D_stable)
+
+
+
+    # Compute the step response of the discrete closed loop system using the different discretization schemes. 
+    # If you couldn't solve the previous exercise, you can use the solution. For that replace the function call with the following:
+    # [t_stable_eulerf, y_stable_eulerf, t_stable_eulerb, y_stable_eulerb, t_stable_tust, y_stable_tust, t_stable_zoh, y_stable_zoh] = disc_solution(A_stable, B_stable, C_stable, D_stable, Ts)
+    t_stable_eulerf, y_stable_eulerf = discrete_step_response_euler_forward(A_stable, B_stable, C_stable, D_stable, Ts)
+    t_stable_eulerb, y_stable_eulerb = discrete_step_response_euler_backward(A_stable, B_stable, C_stable, D_stable, Ts)
+    t_stable_tust, y_stable_tust = discrete_step_response_tustin(A_stable, B_stable, C_stable, D_stable, Ts)
+    t_stable_zoh, y_stable_zoh = discrete_step_response_zoh(A_stable, B_stable, C_stable, D_stable, Ts)
+
+
+
+    # Package the results for plotting.
+    values_to_plot = [t_stable_cont, y_stable_cont,
+                    t_stable_eulerf, y_stable_eulerf,
+                    t_stable_eulerb, y_stable_eulerb,
+                    t_stable_tust, y_stable_tust,
+                    t_stable_zoh, y_stable_zoh]
+
+    # Plot the step responses.
+    plot_step_responses(*values_to_plot)
+
     return None
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/duckiebot.py` & `cs2solutions-0.8.0/src/cs2solutions/duckiebot.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,322 +1,322 @@
-#(c) 2024 ETH Zurich
-
-try:
-    # Import the required python libraries
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-except ImportError as e:
-    print(f"Error importing libraries: {e}")
-
-
-def unicycle_update(t: float, x: np.array, u: np.array, params: dict) -> np.array:
-    # Return the derivative of the state
-    max_omega = params.get('max_omega', 0.05)
-    omega = np.clip(u[1], -max_omega, max_omega)
-    return np.array([
-        u[0] * np.cos(x[2]),    # xdot = v cos(theta)
-        u[0] * np.sin(x[2]),    # ydot = v sin(theta)
-        omega     # thdot = w
-    ])
-
-def unicycle_output(t: float, x: np.array, u: np.array, params: dict) -> np.array:
-    return x[0:2]
-
-#@title
-def plot_track(x_coord_ref: np.array, y_coord_ref: np.array,
-               theta_ref: np.array, t: np.array,
-               w_curvy: np.array,
-               y_ctr: Optional[np.array] = None,
-               w_ctr: Optional[np.array] = None) -> None:
-    # Configure matplotlib plots to be a bit bigger and optimize layout
-    plt.figure(figsize=[9, 4.5])
-    # Plot the resulting trajectory (and some road boundaries)
-    plt.subplot(1, 4, 2)
-    plt.plot(y_coord_ref, x_coord_ref)
-    plt.legend(['reference'])
-    if y_ctr is not None:
-        plt.plot(y_ctr, x_coord_ref, 'r', linewidth=1)
-        plt.legend(['reference', 'controller'])
-    else:
-        plt.legend(['reference'])
-    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
-    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-
-
-
-    plt.xlabel('y [m]')
-    plt.ylabel('x [m]');
-    plt.axis('Equal')
-
-    # Plot the lateral position
-    plt.subplot(2, 2, 2)
-    plt.plot(t, y_coord_ref)
-    if y_ctr is not None:
-        plt.plot(t, y_ctr, 'r')
-        plt.legend(['reference', 'controller'])
-    else:
-        plt.legend(['reference'])
-    plt.ylabel('Lateral position $y$ [m]')
-
-    # Plot the control input
-    plt.subplot(2, 2, 4)
-    plt.plot(t, w_curvy)
-    if w_ctr is not None:
-        plt.plot(t, w_ctr, 'r')
-        plt.legend(['reference', 'controller'])
-    else:
-        plt.legend(['reference'])
-    plt.ylabel('$\\omega$ [rad/s]')
-    plt.xlabel('Time t [sec]')
-    plt.tight_layout()
-
-
-def plot_track_multiple_controller(x_coord_ref: np.array, y_coord_ref: np.array, 
-               theta_ref: np.array, t: np.array, 
-               w_curvy: np.array, 
-               y_ctr: List[np.array],
-               w_ctr: Optional[np.array],
-               ctr_name: Optional[np.array]) -> None:
-    # Configure matplotlib plots to be a bit bigger and optimize layout
-    number_ctr = len(y_ctr)
-    plt.figure(figsize=[14, 6])
-    # Plot the resulting trajectory (and some road boundaries)
-
-    plt.subplot(1, 4, 2)
-    plt.plot(y_coord_ref, x_coord_ref)
-    plt.legend(['Reference'])
-    legend_list = ['Reference']
-    for i in range(number_ctr):
-        plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
-        legend_list.append(ctr_name[i])
-    
-    plt.legend(legend_list, loc='upper left')
-    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
-    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-    
-    
-    
-    plt.xlabel('y [m]')
-    plt.ylabel('x [m]')
-    plt.axis('Equal')
-
-    # Plot the lateral position
-    plt.subplot(2, 2, 2)
-    plt.plot(t, y_coord_ref)
-    legend_list = ['Reference']
-    for i in range(number_ctr):
-        plt.plot(t, y_ctr[i], linewidth=1)
-        legend_list.append(ctr_name[i])
-    plt.legend(legend_list)
-    plt.ylabel('Lateral position $y$ [m]')
-
-    # Plot the control input
-    plt.subplot(2, 2, 4)
-    plt.plot(t, w_curvy)
-    for i in range(number_ctr):
-        plt.plot(t, w_ctr[i], linewidth=1)
-        legend_list.append(ctr_name[i])
-    plt.legend(legend_list)
-    plt.ylabel('$\\omega$ [rad/s]')
-    plt.xlabel('Time t [sec]')
-    plt.tight_layout()
-
-# Updated plot_track_multiple_controller function specifically for the notebook "CS2-2024-unicycle-state-estimation.ipynb"
-def plot_track_multiple_controller2(x_coord_ref: np.array, y_coord_ref: np.array,
-               theta_ref: np.array, t: List[np.array],
-               w_curvy: np.array,
-               y_ctr: List[np.array],
-               w_ctr: Optional[np.array]) -> None:
-    # Configure matplotlib plots to be a bit bigger and optimize layout
-    number_ctr = len(t)
-    plt.figure(figsize=[14, 6])
-    # Plot the resulting trajectory (and some road boundaries)
-
-    plt.subplot(1, 4, 2)
-    plt.plot(y_coord_ref, x_coord_ref)
-    plt.legend(['reference'])
-    legend_list = ['reference']
-    for i in range(number_ctr):
-      plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
-      if number_ctr == 4:
-        if i == 0:
-          legend_list.append('aggressive_controller')
-        elif i == 1:
-          legend_list.append('easy_controller')
-        elif i == 2:
-          legend_list.append('complex_1_controller')
-        elif i == 3:
-          legend_list.append('complex_2_controller')
-        else:
-          legend_list.append(f'controller_{i-4}')
-      else:
-        legend_list.append(f'controller_{i+1}')
-
-    plt.legend(legend_list, loc='upper left')
-    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
-    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-
-
-
-    plt.xlabel('y [m]')
-    plt.ylabel('x [m]');
-    plt.axis('Equal')
-
-    # Plot the lateral position
-    plt.subplot(2, 2, 2)
-    plt.plot(t[0], y_coord_ref)
-    legend_list = ['reference']
-    for i in range(number_ctr):
-      plt.plot(t[i], y_ctr[i], linewidth=1)
-      if number_ctr == 4:
-        if i == 0:
-          legend_list.append('aggressive_controller')
-        elif i == 1:
-          legend_list.append('easy_controller')
-        elif i == 2:
-          legend_list.append('complex_1_controller')
-        elif i == 3:
-          legend_list.append('complex_2_controller')
-        else:
-          legend_list.append(f'controller_{i-4}')
-      else:
-        legend_list.append(f'controller_{i+1}')
-    plt.legend(legend_list)
-    plt.ylabel('Lateral position $y$ [m]')
-
-    # Plot the control input
-    plt.subplot(2, 2, 4)
-    plt.plot(t[0], w_curvy)
-    for i in range(number_ctr):
-      plt.plot(t[i], y_ctr[i], linewidth=1)
-      if number_ctr == 4:
-        if i == 0:
-          legend_list.append('aggressive_controller')
-        elif i == 1:
-          legend_list.append('easy_controller')
-        elif i == 2:
-          legend_list.append('complex_1_controller')
-        elif i == 3:
-          legend_list.append('complex_2_controller')
-        else:
-          legend_list.append(f'controller_{i-4}')
-      else:
-        legend_list.append(f'controller_{i+1}')
-    plt.legend(legend_list)
-    plt.ylabel('$\\omega$ [rad/s]')
-    plt.xlabel('Time t [sec]')
-    plt.tight_layout()
-
-# Updated plot_track_multiple_controller function specifically for the notebook "CS2-2024-LQG.ipynb"
-def plot_track_multiple_controller3(x_coord_ref: np.array, y_coord_ref: np.array,
-               theta_ref: np.array, t: List[np.array],
-               w_curvy: np.array,
-               y_ctr: List[np.array],
-               w_ctr: Optional[np.array]) -> None:
-    # Configure matplotlib plots to be a bit bigger and optimize layout
-    number_ctr = len(t)
-    plt.figure(figsize=[14, 6])
-    # Plot the resulting trajectory (and some road boundaries)
-
-    plt.subplot(1, 4, 2)
-    plt.plot(y_coord_ref, x_coord_ref)
-    plt.legend(['reference'])
-    legend_list = ['reference']
-    for i in range(number_ctr):
-        plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
-        if i == 0:
-          legend_list.append('controller_without_noise')
-        elif i == 1:
-          legend_list.append('controller_with_noise')
-        else:
-          legend_list.append(f'controller_{i-1}')
-
-    plt.legend(legend_list, loc='upper left')
-    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
-    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
-
-    plt.xlabel('y [m]')
-    plt.ylabel('x [m]')
-    plt.axis('Equal')
-
-    # Plot the lateral position
-    plt.subplot(2, 2, 2)
-    plt.plot(t[0], y_coord_ref)
-    legend_list = ['reference']
-    for i in range(number_ctr):
-        plt.plot(t[i], y_ctr[i], linewidth=1)
-        if i ==0:
-          legend_list.append('controller_without_noise')
-        elif i == 1:
-          legend_list.append('controller_with_noise')
-        else:
-          legend_list.append(f'controller_{i-1}')
-    plt.legend(legend_list)
-    plt.ylabel('Lateral position $y$ [m]')
-
-    # Plot the control input
-    plt.subplot(2, 2, 4)
-    plt.plot(t[0], w_curvy)
-    for i in range(number_ctr):
-        plt.plot(t[i], w_ctr[i], linewidth=1)
-        if i ==0:
-          legend_list.append('controller_without_noise')
-        elif i == 1:
-          legend_list.append('controller_with_noise')
-        else:
-          legend_list.append(f'controller_{i-1}')
-    plt.legend(legend_list)
-    plt.ylabel('$\\omega$ [rad/s]')
-    plt.xlabel('Time t [sec]')
-    plt.tight_layout()
-
-# Utility function to plot the step response
-def plot_step_response(t: np.array, y: np.array, u: np.array) -> None:
-    axes_out = plt.subplot(2, 1, 1)
-    plt.sca(axes_out)
-    plt.plot(t, y)
-    plt.ylabel('Lateral position $y$ in [m]')
-    plt.plot([0, 20], [0.95, 0.95], 'k--')
-    plt.plot([0, 20], [1.05, 1.05], 'k--')
-
-    axes_input = plt.subplot(2, 1, 2)
-    plt.sca(axes_input)
-    plt.xlabel('Time t [sec]')
-    plt.ylabel('$\omega$ [rad/s]')
-    plt.plot(t, u[0])
-
-def plot_sim_results(y_ref: np.array, y: np.array,
-                     theta_ref: np.array, theta: np.array,
-                     t: np.array, w_ref: np.array,
-                     w: np.array) -> None:
-    # Configure matplotlib plots to be a bit bigger and optimize layout
-    plt.figure(figsize=[15, 4.5])
-
-    # Plot the actual and estimated states
-    ax = plt.subplot(1, 2, 1)
-    plt.plot(t, y)
-    plt.plot(t, y_ref, 'k-.')
-    ax.set(xlim=[0, 30])
-    plt.legend(['state feedback', 'y', 'reference'])
-    plt.xlabel('Time t [sec]')
-    plt.ylabel('Lateral position $y$ [m]')
-
-    ax = plt.subplot(2, 2, 2)
-    plt.plot(t, theta)
-    # plt.plot(t, x[3])
-    plt.plot(t, theta_ref, 'k-.')
-    ax.set(xlim=[0, 15])
-    plt.ylabel('Angle $\\theta$ [rad]')
-
-    ax = plt.subplot(2, 2, 4)
-    plt.plot(t, w)
-    # plt.plot(t, u_ofb[0])
-    plt.plot(t, w_ref, 'k-.')
-    ax.set(xlim=[0, 15])
-    plt.xlabel('Time t [sec]')
-    plt.ylabel('$\\omega$ [rad/s]')
+#(c) 2024 ETH Zurich
+
+try:
+    # Import the required python libraries
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+except ImportError as e:
+    print(f"Error importing libraries: {e}")
+
+
+def unicycle_update(t: float, x: np.array, u: np.array, params: dict) -> np.array:
+    # Return the derivative of the state
+    max_omega = params.get('max_omega', 0.05)
+    omega = np.clip(u[1], -max_omega, max_omega)
+    return np.array([
+        u[0] * np.cos(x[2]),    # xdot = v cos(theta)
+        u[0] * np.sin(x[2]),    # ydot = v sin(theta)
+        omega     # thdot = w
+    ])
+
+def unicycle_output(t: float, x: np.array, u: np.array, params: dict) -> np.array:
+    return x[0:2]
+
+#@title
+def plot_track(x_coord_ref: np.array, y_coord_ref: np.array,
+               theta_ref: np.array, t: np.array,
+               w_curvy: np.array,
+               y_ctr: Optional[np.array] = None,
+               w_ctr: Optional[np.array] = None) -> None:
+    # Configure matplotlib plots to be a bit bigger and optimize layout
+    plt.figure(figsize=[9, 4.5])
+    # Plot the resulting trajectory (and some road boundaries)
+    plt.subplot(1, 4, 2)
+    plt.plot(y_coord_ref, x_coord_ref)
+    plt.legend(['reference'])
+    if y_ctr is not None:
+        plt.plot(y_ctr, x_coord_ref, 'r', linewidth=1)
+        plt.legend(['reference', 'controller'])
+    else:
+        plt.legend(['reference'])
+    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
+    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+
+
+
+    plt.xlabel('y [m]')
+    plt.ylabel('x [m]');
+    plt.axis('Equal')
+
+    # Plot the lateral position
+    plt.subplot(2, 2, 2)
+    plt.plot(t, y_coord_ref)
+    if y_ctr is not None:
+        plt.plot(t, y_ctr, 'r')
+        plt.legend(['reference', 'controller'])
+    else:
+        plt.legend(['reference'])
+    plt.ylabel('Lateral position $y$ [m]')
+
+    # Plot the control input
+    plt.subplot(2, 2, 4)
+    plt.plot(t, w_curvy)
+    if w_ctr is not None:
+        plt.plot(t, w_ctr, 'r')
+        plt.legend(['reference', 'controller'])
+    else:
+        plt.legend(['reference'])
+    plt.ylabel('$\\omega$ [rad/s]')
+    plt.xlabel('Time t [sec]')
+    plt.tight_layout()
+
+
+def plot_track_multiple_controller(x_coord_ref: np.array, y_coord_ref: np.array, 
+               theta_ref: np.array, t: np.array, 
+               w_curvy: np.array, 
+               y_ctr: List[np.array],
+               w_ctr: Optional[np.array],
+               ctr_name: Optional[np.array]) -> None:
+    # Configure matplotlib plots to be a bit bigger and optimize layout
+    number_ctr = len(y_ctr)
+    plt.figure(figsize=[14, 6])
+    # Plot the resulting trajectory (and some road boundaries)
+
+    plt.subplot(1, 4, 2)
+    plt.plot(y_coord_ref, x_coord_ref)
+    plt.legend(['Reference'])
+    legend_list = ['Reference']
+    for i in range(number_ctr):
+        plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
+        legend_list.append(ctr_name[i])
+    
+    plt.legend(legend_list, loc='upper left')
+    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
+    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+    
+    
+    
+    plt.xlabel('y [m]')
+    plt.ylabel('x [m]')
+    plt.axis('Equal')
+
+    # Plot the lateral position
+    plt.subplot(2, 2, 2)
+    plt.plot(t, y_coord_ref)
+    legend_list = ['Reference']
+    for i in range(number_ctr):
+        plt.plot(t, y_ctr[i], linewidth=1)
+        legend_list.append(ctr_name[i])
+    plt.legend(legend_list)
+    plt.ylabel('Lateral position $y$ [m]')
+
+    # Plot the control input
+    plt.subplot(2, 2, 4)
+    plt.plot(t, w_curvy)
+    for i in range(number_ctr):
+        plt.plot(t, w_ctr[i], linewidth=1)
+        legend_list.append(ctr_name[i])
+    plt.legend(legend_list)
+    plt.ylabel('$\\omega$ [rad/s]')
+    plt.xlabel('Time t [sec]')
+    plt.tight_layout()
+
+# Updated plot_track_multiple_controller function specifically for the notebook "CS2-2024-unicycle-state-estimation.ipynb"
+def plot_track_multiple_controller2(x_coord_ref: np.array, y_coord_ref: np.array,
+               theta_ref: np.array, t: List[np.array],
+               w_curvy: np.array,
+               y_ctr: List[np.array],
+               w_ctr: Optional[np.array]) -> None:
+    # Configure matplotlib plots to be a bit bigger and optimize layout
+    number_ctr = len(t)
+    plt.figure(figsize=[14, 6])
+    # Plot the resulting trajectory (and some road boundaries)
+
+    plt.subplot(1, 4, 2)
+    plt.plot(y_coord_ref, x_coord_ref)
+    plt.legend(['reference'])
+    legend_list = ['reference']
+    for i in range(number_ctr):
+      plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
+      if number_ctr == 4:
+        if i == 0:
+          legend_list.append('aggressive_controller')
+        elif i == 1:
+          legend_list.append('easy_controller')
+        elif i == 2:
+          legend_list.append('complex_1_controller')
+        elif i == 3:
+          legend_list.append('complex_2_controller')
+        else:
+          legend_list.append(f'controller_{i-4}')
+      else:
+        legend_list.append(f'controller_{i+1}')
+
+    plt.legend(legend_list, loc='upper left')
+    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
+    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+
+
+
+    plt.xlabel('y [m]')
+    plt.ylabel('x [m]');
+    plt.axis('Equal')
+
+    # Plot the lateral position
+    plt.subplot(2, 2, 2)
+    plt.plot(t[0], y_coord_ref)
+    legend_list = ['reference']
+    for i in range(number_ctr):
+      plt.plot(t[i], y_ctr[i], linewidth=1)
+      if number_ctr == 4:
+        if i == 0:
+          legend_list.append('aggressive_controller')
+        elif i == 1:
+          legend_list.append('easy_controller')
+        elif i == 2:
+          legend_list.append('complex_1_controller')
+        elif i == 3:
+          legend_list.append('complex_2_controller')
+        else:
+          legend_list.append(f'controller_{i-4}')
+      else:
+        legend_list.append(f'controller_{i+1}')
+    plt.legend(legend_list)
+    plt.ylabel('Lateral position $y$ [m]')
+
+    # Plot the control input
+    plt.subplot(2, 2, 4)
+    plt.plot(t[0], w_curvy)
+    for i in range(number_ctr):
+      plt.plot(t[i], y_ctr[i], linewidth=1)
+      if number_ctr == 4:
+        if i == 0:
+          legend_list.append('aggressive_controller')
+        elif i == 1:
+          legend_list.append('easy_controller')
+        elif i == 2:
+          legend_list.append('complex_1_controller')
+        elif i == 3:
+          legend_list.append('complex_2_controller')
+        else:
+          legend_list.append(f'controller_{i-4}')
+      else:
+        legend_list.append(f'controller_{i+1}')
+    plt.legend(legend_list)
+    plt.ylabel('$\\omega$ [rad/s]')
+    plt.xlabel('Time t [sec]')
+    plt.tight_layout()
+
+# Updated plot_track_multiple_controller function specifically for the notebook "CS2-2024-LQG.ipynb"
+def plot_track_multiple_controller3(x_coord_ref: np.array, y_coord_ref: np.array,
+               theta_ref: np.array, t: List[np.array],
+               w_curvy: np.array,
+               y_ctr: List[np.array],
+               w_ctr: Optional[np.array]) -> None:
+    # Configure matplotlib plots to be a bit bigger and optimize layout
+    number_ctr = len(t)
+    plt.figure(figsize=[14, 6])
+    # Plot the resulting trajectory (and some road boundaries)
+
+    plt.subplot(1, 4, 2)
+    plt.plot(y_coord_ref, x_coord_ref)
+    plt.legend(['reference'])
+    legend_list = ['reference']
+    for i in range(number_ctr):
+        plt.plot(y_ctr[i], x_coord_ref, linewidth=1)
+        if i == 0:
+          legend_list.append('controller_without_noise')
+        elif i == 1:
+          legend_list.append('controller_with_noise')
+        else:
+          legend_list.append(f'controller_{i-1}')
+
+    plt.legend(legend_list, loc='upper left')
+    plt.plot(y_coord_ref - 0.9/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+    plt.plot(y_coord_ref - 0.3/np.cos(theta_ref), x_coord_ref, 'k--', linewidth=1)
+    plt.plot(y_coord_ref + 0.3/np.cos(theta_ref), x_coord_ref, 'k-', linewidth=1)
+
+    plt.xlabel('y [m]')
+    plt.ylabel('x [m]')
+    plt.axis('Equal')
+
+    # Plot the lateral position
+    plt.subplot(2, 2, 2)
+    plt.plot(t[0], y_coord_ref)
+    legend_list = ['reference']
+    for i in range(number_ctr):
+        plt.plot(t[i], y_ctr[i], linewidth=1)
+        if i ==0:
+          legend_list.append('controller_without_noise')
+        elif i == 1:
+          legend_list.append('controller_with_noise')
+        else:
+          legend_list.append(f'controller_{i-1}')
+    plt.legend(legend_list)
+    plt.ylabel('Lateral position $y$ [m]')
+
+    # Plot the control input
+    plt.subplot(2, 2, 4)
+    plt.plot(t[0], w_curvy)
+    for i in range(number_ctr):
+        plt.plot(t[i], w_ctr[i], linewidth=1)
+        if i ==0:
+          legend_list.append('controller_without_noise')
+        elif i == 1:
+          legend_list.append('controller_with_noise')
+        else:
+          legend_list.append(f'controller_{i-1}')
+    plt.legend(legend_list)
+    plt.ylabel('$\\omega$ [rad/s]')
+    plt.xlabel('Time t [sec]')
+    plt.tight_layout()
+
+# Utility function to plot the step response
+def plot_step_response(t: np.array, y: np.array, u: np.array) -> None:
+    axes_out = plt.subplot(2, 1, 1)
+    plt.sca(axes_out)
+    plt.plot(t, y)
+    plt.ylabel('Lateral position $y$ in [m]')
+    plt.plot([0, 20], [0.95, 0.95], 'k--')
+    plt.plot([0, 20], [1.05, 1.05], 'k--')
+
+    axes_input = plt.subplot(2, 1, 2)
+    plt.sca(axes_input)
+    plt.xlabel('Time t [sec]')
+    plt.ylabel('$\omega$ [rad/s]')
+    plt.plot(t, u[0])
+
+def plot_sim_results(y_ref: np.array, y: np.array,
+                     theta_ref: np.array, theta: np.array,
+                     t: np.array, w_ref: np.array,
+                     w: np.array) -> None:
+    # Configure matplotlib plots to be a bit bigger and optimize layout
+    plt.figure(figsize=[15, 4.5])
+
+    # Plot the actual and estimated states
+    ax = plt.subplot(1, 2, 1)
+    plt.plot(t, y)
+    plt.plot(t, y_ref, 'k-.')
+    ax.set(xlim=[0, 30])
+    plt.legend(['state feedback', 'y', 'reference'])
+    plt.xlabel('Time t [sec]')
+    plt.ylabel('Lateral position $y$ [m]')
+
+    ax = plt.subplot(2, 2, 2)
+    plt.plot(t, theta)
+    # plt.plot(t, x[3])
+    plt.plot(t, theta_ref, 'k-.')
+    ax.set(xlim=[0, 15])
+    plt.ylabel('Angle $\\theta$ [rad]')
+
+    ax = plt.subplot(2, 2, 4)
+    plt.plot(t, w)
+    # plt.plot(t, u_ofb[0])
+    plt.plot(t, w_ref, 'k-.')
+    ax.set(xlim=[0, 15])
+    plt.xlabel('Time t [sec]')
+    plt.ylabel('$\\omega$ [rad/s]')
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/intro.py` & `cs2solutions-0.8.0/src/cs2solutions/intro.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-#(c) 2024 ETH Zurich
-
-try:
-    import control as ct
-    
-except ImportError:
-    print('Error: Could not import control library. Please install it using the command "!pip install control"')
-
-try:
-    import matplotlib.pyplot as plt
-except ImportError:
-    print('Error: Could not import matplotlib library. Please install it using the command "!pip install matplotlib"')
-
-try:
-    import numpy as np
-except ImportError:
-    print('Error: Could not import numpy library. Please install it using the command "!pip install numpy"')
-
-try:
-    import unittest as unit
-except ImportError:
-    print('Error: Could not import unittest library. Please install it using the command "!pip install unittest"')
-
-#solution function definitions
-
-def sol_create_transfer_function() -> ct.TransferFunction:
-    """
-    Solution: Create a TransferFunction object to represent the transfer function s/(s^2+2*s+1).
-
-    Returns:
-    TransferFunction: The created TransferFunction object.
-    """
-    # Define system parameters
-    numerator_coeffs = [1,0]
-    denominator_coeffs = [1, 2, 1]
-
-    # Create a transfer function
-    tf = ct.TransferFunction(numerator_coeffs, denominator_coeffs)
-    return tf
-
-def test_create_transfer_function(student_sol: callable, sol_tf: callable, shouldprint: bool = True) -> bool:
-    """
-    Test function to compare the student's transfer function with the solution transfer function.
-
-    Parameters:
-    - student_sol: A function that returns the student's transfer function.
-    - sol: A function that returns the solution transfer function.
-    - shouldprint: A boolean indicating whether to print the transfer functions. Default is True.
-
-    Raises:
-        AssertionError: If the input is not an instance of the TransferFunction class.
-
-    Returns:
-    - A boolean indicating whether the student's transfer function is equal to the solution transfer function.
-    """
-    # Create a transfer function using the student's code
-    student_tf = student_sol()
-    # Create a transfer function using the solution code
-    sol_tf = sol_tf()
-
-    # Check if the student's transfer function is an instance of the TransferFunction class
-    assert isinstance(student_tf, ct.TransferFunction), "The function should return an instance of the TransferFunction class."
-    assert isinstance(sol_tf, ct.TransferFunction), "The function should return an instance of the TransferFunction class."
-
-    # Check if the student's transfer function is equal to the solution transfer function
-    if (shouldprint):
-        print("Student's transfer function: ", student_tf)
-        print("Solution transfer function: ", sol_tf)
-
-    return np.array_equal(student_tf.num, sol_tf.num) and np.array_equal(student_tf.den, sol_tf.den)
-
-
-def sol_plot_step_response(tf: ct.TransferFunction) -> None:
-    """
-    Solution: Plot the step response of the given transfer function.
-
-    Parameters:
-    tf (TransferFunction): The transfer function to plot the step response for.
-
-    Raises:
-        AssertionError: If the input is not an instance of the TransferFunction class.
-
-    Returns:
-    None
-    """
-    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
-
-    # Compute the step response of the system
-    time, response = ct.step_response(tf)
-
-    # Plot the step response
-    plt.figure()
-    plt.plot(time, response)
-    plt.title('Step Response of the System')
-    plt.xlabel('Time')
-    plt.ylabel('Amplitude')
-    plt.grid(True)
-    plt.show()
-
-    return None
-
-def test_plot_step_response(student_plot: callable, sol_plot: callable, tf: ct.TransferFunction, shouldprint: bool = True) -> None:
-    """
-    Test function to compare the student's step response plot with the solution step response plot.
-
-    Parameters:
-    - student_plot: A function that plots the student's step response.
-    - sol_plot: A function that plots the solution step response.
-    - shouldprint: A boolean indicating whether to print the plots. Default is True.
-
-    Raises:
-        AssertionError: If the input is not an instance of the TransferFunction class.
-
-    Returns:
-    - A boolean indicating whether the student's step response plot is equal to the solution step response plot.
-    """
-    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
-
-    # Plot the step response using the student's code
-    print("Student's plot:") if shouldprint else None
-    student_plot(tf)
-    # Plot the step response using the solution code
-    print("Solution plot:") if shouldprint else None
-    sol_plot(sol_create_transfer_function())
-
-    return None
-
-
-def sol_bode_plot(tf: ct.TransferFunction) -> None:
-    """
-    Solution: Plot the Bode magnitude and phase plots for a given transfer function.
-
-    Parameters:
-        tf (ct.TransferFunction): The transfer function to plot.
-
-    Raises:
-        AssertionError: If the input is not an instance of the TransferFunction class.
-    """
-    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
-
-    mag, phase, omega = ct.bode_plot(tf)
-    return None
-
-
-def sol_get_filter_tf(omega_c: float, is_verbose : bool = False) -> ct.TransferFunction:
-    """
-    Creates a transfer function for a low pass filter.
-
-    Parameters:
-    omega_c (float): The cutoff frequency of the filter.
-    is_verbose (bool, optional): If True, prints additional information about the filter. Default is False.
-
-    Returns:
-    ct.TransferFunction: The transfer function of the low pass filter.
-    """
-    assert isinstance(omega_c, float) or isinstance(omega_c, int), "The cutoff frequency should be a number."
-    assert omega_c > 0, "The cutoff frequency should be greater than 0."
-
-    if is_verbose:
-        print("It can be show that the parameter \"a\" from Exercise 4.1 is equal to (omega_c)^-1.\nTherefore, the TF of the low pass filter is:")
-
-    # Define system parameters
-    numerator_coeffs = [1.0]
-    denominator_coeffs = [1.0 / omega_c, 1.0]
-
-    # Create a transfer function
-    tf = ct.TransferFunction(numerator_coeffs, denominator_coeffs)
-    return tf
-
-def test_create_filter_tf(student_filter: callable, sol_filter: callable, omega_c: float, shouldprint: bool = True) -> bool:
-    """
-    Test the create_filter_tf function.
-
-    Parameters:
-    student_filter (function): The student's implementation of the filter function.
-    sol_filter (function): The solution's implementation of the filter function.
-    omega_c (float): The cutoff frequency.
-    shouldprint (bool, optional): Whether to print the test results. Defaults to True.
-
-    Returns:
-    bool: True if the student's implementation matches the solution's implementation, False otherwise.
-    """
-    assert isinstance(omega_c, float) or isinstance(omega_c, int), "The cutoff frequency should be a number."
-    assert isinstance(student_filter(omega_c), ct.TransferFunction), "The function should return an instance of the TransferFunction class."
-    assert isinstance(sol_filter(omega_c), ct.TransferFunction), "The function should return an instance of the TransferFunction class."
-
-    student_tf = student_filter(omega_c)
-    sol_tf = sol_filter(omega_c)
-
-    return np.array_equal(student_tf.num, sol_tf.num) and np.array_equal(student_tf.den, sol_tf.den)
-
-#test function definitions
-
-def test(answer: callable, solution: callable, is_verbose: bool = True) -> None:
-    #this is a very simple test to check correct inputs and plotting
-    if(is_verbose):
-        print(f"Your answer: {answer()}")
-        print(f"Expected answer: {solution()}")
-    else:
-        print("Your answer: ")
-        answer()
-        print("Expected answer: ")
-        solution()
-    return None
+#(c) 2024 ETH Zurich
+
+try:
+    import control as ct
+    
+except ImportError:
+    print('Error: Could not import control library. Please install it using the command "!pip install control"')
+
+try:
+    import matplotlib.pyplot as plt
+except ImportError:
+    print('Error: Could not import matplotlib library. Please install it using the command "!pip install matplotlib"')
+
+try:
+    import numpy as np
+except ImportError:
+    print('Error: Could not import numpy library. Please install it using the command "!pip install numpy"')
+
+try:
+    import unittest as unit
+except ImportError:
+    print('Error: Could not import unittest library. Please install it using the command "!pip install unittest"')
+
+#solution function definitions
+
+def sol_create_transfer_function() -> ct.TransferFunction:
+    """
+    Solution: Create a TransferFunction object to represent the transfer function s/(s^2+2*s+1).
+
+    Returns:
+    TransferFunction: The created TransferFunction object.
+    """
+    # Define system parameters
+    numerator_coeffs = [1,0]
+    denominator_coeffs = [1, 2, 1]
+
+    # Create a transfer function
+    tf = ct.TransferFunction(numerator_coeffs, denominator_coeffs)
+    return tf
+
+def test_create_transfer_function(student_sol: callable, sol_tf: callable, shouldprint: bool = True) -> bool:
+    """
+    Test function to compare the student's transfer function with the solution transfer function.
+
+    Parameters:
+    - student_sol: A function that returns the student's transfer function.
+    - sol: A function that returns the solution transfer function.
+    - shouldprint: A boolean indicating whether to print the transfer functions. Default is True.
+
+    Raises:
+        AssertionError: If the input is not an instance of the TransferFunction class.
+
+    Returns:
+    - A boolean indicating whether the student's transfer function is equal to the solution transfer function.
+    """
+    # Create a transfer function using the student's code
+    student_tf = student_sol()
+    # Create a transfer function using the solution code
+    sol_tf = sol_tf()
+
+    # Check if the student's transfer function is an instance of the TransferFunction class
+    assert isinstance(student_tf, ct.TransferFunction), "The function should return an instance of the TransferFunction class."
+    assert isinstance(sol_tf, ct.TransferFunction), "The function should return an instance of the TransferFunction class."
+
+    # Check if the student's transfer function is equal to the solution transfer function
+    if (shouldprint):
+        print("Student's transfer function: ", student_tf)
+        print("Solution transfer function: ", sol_tf)
+
+    return np.array_equal(student_tf.num, sol_tf.num) and np.array_equal(student_tf.den, sol_tf.den)
+
+
+def sol_plot_step_response(tf: ct.TransferFunction) -> None:
+    """
+    Solution: Plot the step response of the given transfer function.
+
+    Parameters:
+    tf (TransferFunction): The transfer function to plot the step response for.
+
+    Raises:
+        AssertionError: If the input is not an instance of the TransferFunction class.
+
+    Returns:
+    None
+    """
+    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
+
+    # Compute the step response of the system
+    time, response = ct.step_response(tf)
+
+    # Plot the step response
+    plt.figure()
+    plt.plot(time, response)
+    plt.title('Step Response of the System')
+    plt.xlabel('Time')
+    plt.ylabel('Amplitude')
+    plt.grid(True)
+    plt.show()
+
+    return None
+
+def test_plot_step_response(student_plot: callable, sol_plot: callable, tf: ct.TransferFunction, shouldprint: bool = True) -> None:
+    """
+    Test function to compare the student's step response plot with the solution step response plot.
+
+    Parameters:
+    - student_plot: A function that plots the student's step response.
+    - sol_plot: A function that plots the solution step response.
+    - shouldprint: A boolean indicating whether to print the plots. Default is True.
+
+    Raises:
+        AssertionError: If the input is not an instance of the TransferFunction class.
+
+    Returns:
+    - A boolean indicating whether the student's step response plot is equal to the solution step response plot.
+    """
+    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
+
+    # Plot the step response using the student's code
+    print("Student's plot:") if shouldprint else None
+    student_plot(tf)
+    # Plot the step response using the solution code
+    print("Solution plot:") if shouldprint else None
+    sol_plot(sol_create_transfer_function())
+
+    return None
+
+
+def sol_bode_plot(tf: ct.TransferFunction) -> None:
+    """
+    Solution: Plot the Bode magnitude and phase plots for a given transfer function.
+
+    Parameters:
+        tf (ct.TransferFunction): The transfer function to plot.
+
+    Raises:
+        AssertionError: If the input is not an instance of the TransferFunction class.
+    """
+    assert isinstance(tf, ct.TransferFunction), "The input should be an instance of the TransferFunction class."
+
+    mag, phase, omega = ct.bode_plot(tf)
+    return None
+
+
+def sol_get_filter_tf(omega_c: float, is_verbose : bool = False) -> ct.TransferFunction:
+    """
+    Creates a transfer function for a low pass filter.
+
+    Parameters:
+    omega_c (float): The cutoff frequency of the filter.
+    is_verbose (bool, optional): If True, prints additional information about the filter. Default is False.
+
+    Returns:
+    ct.TransferFunction: The transfer function of the low pass filter.
+    """
+    assert isinstance(omega_c, float) or isinstance(omega_c, int), "The cutoff frequency should be a number."
+    assert omega_c > 0, "The cutoff frequency should be greater than 0."
+
+    if is_verbose:
+        print("It can be show that the parameter \"a\" from Exercise 4.1 is equal to (omega_c)^-1.\nTherefore, the TF of the low pass filter is:")
+
+    # Define system parameters
+    numerator_coeffs = [1.0]
+    denominator_coeffs = [1.0 / omega_c, 1.0]
+
+    # Create a transfer function
+    tf = ct.TransferFunction(numerator_coeffs, denominator_coeffs)
+    return tf
+
+def test_create_filter_tf(student_filter: callable, sol_filter: callable, omega_c: float, shouldprint: bool = True) -> bool:
+    """
+    Test the create_filter_tf function.
+
+    Parameters:
+    student_filter (function): The student's implementation of the filter function.
+    sol_filter (function): The solution's implementation of the filter function.
+    omega_c (float): The cutoff frequency.
+    shouldprint (bool, optional): Whether to print the test results. Defaults to True.
+
+    Returns:
+    bool: True if the student's implementation matches the solution's implementation, False otherwise.
+    """
+    assert isinstance(omega_c, float) or isinstance(omega_c, int), "The cutoff frequency should be a number."
+    assert isinstance(student_filter(omega_c), ct.TransferFunction), "The function should return an instance of the TransferFunction class."
+    assert isinstance(sol_filter(omega_c), ct.TransferFunction), "The function should return an instance of the TransferFunction class."
+
+    student_tf = student_filter(omega_c)
+    sol_tf = sol_filter(omega_c)
+
+    return np.array_equal(student_tf.num, sol_tf.num) and np.array_equal(student_tf.den, sol_tf.den)
+
+#test function definitions
+
+def test(answer: callable, solution: callable, is_verbose: bool = True) -> None:
+    #this is a very simple test to check correct inputs and plotting
+    if(is_verbose):
+        print(f"Your answer: {answer()}")
+        print(f"Expected answer: {solution()}")
+    else:
+        print("Your answer: ")
+        answer()
+        print("Expected answer: ")
+        solution()
+    return None
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/intromimo.py` & `cs2solutions-0.8.0/src/cs2solutions/intromimo.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,425 +1,425 @@
-from typing import Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import sympy as sp
-    import matplotlib.pyplot as plt
-    import control as ct
-    import signal
-    from scipy import signal as signal
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-
-def sol_sys_matrices():
-    """
-    Produce the system matrices for the CS2Bot system.
-  
-    Parameters:
-    - None
-
-    Returns:
-    - () -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]: The system matrices A, B, C, and D.
-    """
-    A = np.array([[0, 3], [0, 0]], dtype=int)
-    B = np.array([[0, 0], [0, 1]], dtype=int)
-    C = np.array([[1, 0], [0, 1]], dtype=int)
-    D = np.array([[0, 0], [0, 0]], dtype=int)
-
-    return A, B, C, D
-
-
-def test_sys_matrices(student_sol: callable, master_sol: callable) -> bool:
-    """
-    Check if the student solution is correct for sys_matrices().
-
-    Parameters:
-    - ``student_sol`` (function): A function that returns the student's solution.
-    - ``master_sol`` (function): A function that returns the master solution.
-
-    Returns:
-    - bool: A boolean indicating if the student solution is correct.
-    """
-    try:
-        student = student_sol()
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol()
-    assert np.allclose(student[0], master[0]), "A matrix is incorrect."
-    assert np.allclose(student[1], master[1]), "B matrix is incorrect."
-    assert np.allclose(student[2], master[2]), "C matrix is incorrect."
-    assert np.allclose(student[3], master[3]), "D matrix is incorrect."
-
-    print("Student solution is correct.")
-    return True
-
-
-def sol_poles(A_: np.ndarray, B_: np.ndarray, C_: np.array, D_=np.array) -> np.array:
-    """
-    Determine the poles the system.
-
-    Parameters:
-    - ``A_`` (np.ndarray): The A matrix of the system.
-    - ``B_`` (np.ndarray): The B matrix of the system.
-    - ``C_`` (np.ndarray): The C matrix of the system.
-    - ``D_`` (np.ndarray): The D matrix of the system.
-
-    Returns:
-    - np.array: The poles of the system.
-    """
-    return ct.poles(ct.StateSpace(A_, B_, C_, D_))
-
-
-def test_poles(student_sol: callable, master_sol: callable) -> bool:
-    """
-    Unit tests for checking the implementation of sol_poles. This function should calculate the poles of the system.
-    """
-
-    passed_tests = 0
-    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
-    B1 = np.array([[1, 2], [5, 6], [3, 4]])
-    C1 = np.array([[1, -2, 1]])
-    D1 = np.array([[1, 3]])
-    try:
-        student = student_sol(A1, B1, C1, D1)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A1, B1, C1, D1)
-    if not np.array_equal(student, master, equal_nan=True):
-        print("Test failed: The poles are incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    A2 = np.array([[0, 3], [0, 0]], dtype=int)
-    B2 = np.array([[0, 0], [0, 1]], dtype=int)
-    C2 = np.array([[1, 0], [0, 1]], dtype=int)
-    D2 = np.array([[0, 0], [0, 0]], dtype=int)
-    try:
-        student = student_sol(A2, B2, C2, D2)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A2, B2, C2, D2)
-    if not np.array_equal(student, master, equal_nan=True):
-        print("Test failed: The poles are incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
-    B3 = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
-    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
-    D3 = np.array([[0, 0], [0, 0], [0, 0]], dtype=int)
-    try:
-        student = student_sol(A3, B3, C3, D3)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A3, B3, C3, D3)
-    if not np.array_equal(student, master, equal_nan=True):
-        print("Test failed: The poles are incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    print("Passed tests:", passed_tests, " out of 3")
-    return passed_tests == 3
-
-
-def sol_num_inputs(B_: np.ndarray) -> int:
-    """
-    Determine the number of inputs for the system.
-
-    Parameters:
-    - ``B_`` (np.ndarray): The B matrix of the system.
-
-    Returns:
-    - int: The number of inputs for the system.
-    """
-    return B_.shape[1]
-
-
-def sol_num_outputs(C_: np.ndarray) -> int:
-    """
-    Determine the number of outputs for the system.
-
-    Parameters:
-    - ``C_`` (np.ndarray): The C matrix of the system.
-
-    Returns:
-    - int: The number of outputs for the system.
-    """
-    return C_.shape[0]
-
-
-def test_num_inputs_outputs(student_num_inputs: callable, student_num_outputs: callable, master_num_inputs: callable,
-                            master_num_outputs: callable) -> bool:
-    """
-    Check if the student solution is correct for num_inputs() and num_outputs().
-
-    Parameters:
-    - ``student_num_inputs`` (function): A function that returns the student's solution for num_inputs().
-    - ``student_num_outputs`` (function): A function that returns the student's solution for num_outputs().
-    - ``master_num_inputs`` (function): A function that returns the master solution for num_inputs().
-    - ``master_num_outputs`` (function): A function that returns the master solution for num_outputs().
-
-    Returns:
-    - bool: A boolean indicating if the student solution is correct.
-    """
-    B_ = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
-    C_ = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
-
-    try:
-        student_inputs = student_num_inputs(B_)
-        student_outputs = student_num_outputs(C_)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-
-    master_inputs = master_num_inputs(B_)
-    master_outputs = master_num_outputs(C_)
-    assert student_inputs == master_inputs, "The number of inputs is incorrect: {student_inputs} != {master_inputs}"
-    assert student_outputs == master_outputs, "The number of outputs is incorrect: {student_outputs} != {master_outputs}"
-
-    print("Student solution is correct.")
-    return True
-
-
-def sol_calc_tf_symb(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray) -> sp.Matrix:
-    """
-    Calculate the transfer function of the system using symbolic mathematics.
-
-    Parameters:
-    - ``A`` (np.ndarray): The A matrix of the system.
-    - ``B`` (np.ndarray): The B matrix of the system.
-    - ``C`` (np.ndarray): The C matrix of the system.
-    - ``D`` (np.ndarray): The D matrix of the system.
-
-    Returns:
-    - sp.Matrix: The transfer function of the system.
-    """
-    # Check dimensions of A, B, C, D
-    assert A.shape[0] == A.shape[1], "A must be a square matrix"
-    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
-    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
-    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
-
-    # define identity matrix of appropriate size
-    s = sp.symbols('s')
-    I = np.eye(A.shape[0])
-
-    # calculate the inverse of (s*I - A)
-    term = sp.Matrix(s * I - A)
-    inv_term = term.inv()
-
-    # calculate P_s
-    transferfunction = np.dot(C, np.dot(inv_term, B)) + D
-
-    # simplify the answer so that there are no double fractions
-    transferfunction = sp.simplify(transferfunction)
-
-    return transferfunction
-
-
-def test_calc_tf_symb(student_sol: callable, master_sol: callable) -> bool:
-    """
-    Unit tests for checking the implementation of calc_symb_sol(). This function should symbolically calculate the MIMO transfer function given A, B, C, and D matrices.
-    """
-
-    passed_tests = 0
-    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
-    B1 = np.array([[1, 2], [5, 6], [3, 4]])
-    C1 = np.array([[1, -2, 1]])
-    D1 = np.array([[1, 3]])
-    try:
-        student = student_sol(A1, B1, C1, D1)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A1, B1, C1, D1)
-    if (student != master):
-        print("Test failed: The transfer function is incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    A2 = np.array([[0, 3], [0, 0]], dtype=int)
-    B2 = np.array([[0, 0], [0, 1]], dtype=int)
-    C2 = np.array([[1, 0], [0, 1]], dtype=int)
-    D2 = np.array([[0, 0], [0, 0]], dtype=int)
-    try:
-        student = student_sol(A2, B2, C2, D2)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A2, B2, C2, D2)
-    if (student != master):
-        print("Test failed: The transfer function is incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
-    B3 = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
-    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
-    D3 = np.array([[0, 0], [0, 0], [0, 0]], dtype=int)
-    try:
-        student = student_sol(A3, B3, C3, D3)
-    except Exception as e:
-        print(f"Error: {e}")
-        return False
-    master = master_sol(A3, B3, C3, D3)
-    if (student != master):
-        print("Test failed: The transfer function is incorrect.")
-        print("Student's result: ", student)
-        print("Expected result: ", master)
-    else:
-        passed_tests += 1
-
-    print("Passed tests:", passed_tests, " out of 3")
-    return passed_tests == 3
-
-
-def sol_calc_tf_ctrl(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, outputnumber: int = 0) -> Tuple[
-    np.ndarray, np.ndarray, Optional[float]]:
-    """
-    Calculate the transfer function of the system using signal library.
-
-    Parameters:
-    - ``A`` (np.ndarray): The A matrix of the system.
-    - ``B`` (np.ndarray): The B matrix of the system.
-    - ``C`` (np.ndarray): The C matrix of the system.
-    - ``D`` (np.ndarray): The D matrix of the system.
-
-    Returns:
-    - Tuple[np.ndarray, np.ndarray, Optional[float]]: The transfer function of the system.
-    """
-    # Check dimensions of A, B, C, D
-    assert A.shape[0] == A.shape[1], "A must be a square matrix"
-    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
-    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
-    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
-
-    transferfunction = signal.ss2tf(A, B, C, D, outputnumber)
-
-    return transferfunction
-
-
-def test_calc_tf_ctrl(student_sol: callable, master_sol: callable) -> bool:
-    """
-    Unit tests for checking the implementation of calc_tf_ctrl(). This function should calculate the MIMO transfer function given A, B, C, and D matrices.
-    """
-
-    passed_tests = 0
-    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
-    B1 = np.array([[1, 2], [5, 6], [3, 4]])
-    C1 = np.array([[1, -2, 1]])
-    D1 = np.array([[1, 3]])
-    num_outputs = 1
-    for i in range(num_outputs):
-        try:
-            student = student_sol(A1, B1, C1, D1, i)
-        except Exception as e:
-            print(f"Error: {e}")
-            return False
-        master = master_sol(A1, B1, C1, D1, i)
-        if (compare_tuples(student, master) == False):
-            print("Test failed: The transfer function for output {i} is incorrect.")
-            print("Student's result: ", student)
-            print("Expected result: ", master)
-        else:
-            passed_tests += 1
-    print("First test series passed")
-
-    A2 = np.array([[0, 3], [0, 0]], dtype=int)
-    B2 = np.array([[0, 0], [0, 1]], dtype=int)
-    C2 = np.array([[1, 0], [0, 1]], dtype=int)
-    D2 = np.array([[0, 0], [0, 0]], dtype=int)
-    num_outputs = 2
-    for i in range(num_outputs):
-        try:
-            student = student_sol(A2, B2, C2, D2, i)
-        except Exception as e:
-            print(f"Error: {e}")
-            return False
-        master = master_sol(A2, B2, C2, D2, i)
-        if (compare_tuples(student, master) == False):
-            print("Test failed: The transfer function for output {i} is incorrect.")
-            print("Student's result: ", student)
-            print("Expected result: ", master)
-        else:
-            passed_tests += 1
-    print("Second test series passed")
-
-    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
-    B3 = np.array([[1, 0, 2], [0, 1, 0], [0, 0, 1]], dtype=int)
-    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
-    D3 = np.array([[0, 0, 0], [0, 0, 0], [0, 0, 0]], dtype=int)
-    num_outputs = 3
-    for i in range(num_outputs):
-        try:
-            student = student_sol(A3, B3, C3, D3, i)
-        except Exception as e:
-            print(f"Error: {e}")
-            return False
-        master = master_sol(A3, B3, C3, D3, i)
-        if (compare_tuples(student, master) == False):
-            print("Test failed: The transfer function is incorrect.")
-            print("Student's result: ", student)
-            print("Expected result: ", master)
-        else:
-            passed_tests += 1
-    print("Third test series passed")
-
-    print("Passed tests:", passed_tests, " out of 6")
-    return passed_tests == 6
-
-
-def compare_tuples(t1: Tuple[np.ndarray, np.ndarray, Optional[float]],
-                   t2: Tuple[np.ndarray, np.ndarray, Optional[float]]) -> bool:
-    return np.array_equal(t1[0], t2[0]) and np.array_equal(t1[1], t2[1])
-
-
-def sol_get_tf(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray) -> Tuple[
-    np.ndarray, signal.TransferFunction, signal.TransferFunction, signal.TransferFunction, signal.TransferFunction]:
-    """
-    Find the individual transfer functions in the transfer function matrix.
-
-    Parameters:
-    - ``A`` (np.ndarray): The A matrix of the system.
-    - ``B`` (np.ndarray): The B matrix of the system.
-    - ``C`` (np.ndarray): The C matrix of the system.
-    - ``D`` (np.ndarray): The D matrix of the system.
-
-    Returns:
-    - Tuple[np.ndarray, TransferFunction, TransferFunction, TransferFunction, TransferFunction]: The individual transfer functions
-    """
-    # Check dimensions of A, B, C, D
-    assert A.shape[0] == A.shape[1], "A must be a square matrix"
-    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
-    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
-    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
-
-    tf_output1 = sol_calc_tf_ctrl(A, B, C, D, 0)
-    tf_output2 = sol_calc_tf_ctrl(A, B, C, D, 1)
-
-    den = tf_output1[1]
-
-    tf_11 = signal.TransferFunction(tf_output1[0][0], den)
-    tf_12 = signal.TransferFunction(tf_output2[0][0], den)
-    tf_21 = signal.TransferFunction(tf_output1[0][1], den)
-    tf_22 = signal.TransferFunction(tf_output2[0][1], den)
-
-    return den, tf_11, tf_12, tf_21, tf_22
+from typing import Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import sympy as sp
+    import matplotlib.pyplot as plt
+    import control as ct
+    import signal
+    from scipy import signal as signal
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+
+def sol_sys_matrices():
+    """
+    Produce the system matrices for the CS2Bot system.
+  
+    Parameters:
+    - None
+
+    Returns:
+    - () -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]: The system matrices A, B, C, and D.
+    """
+    A = np.array([[0, 3], [0, 0]], dtype=int)
+    B = np.array([[0, 0], [0, 1]], dtype=int)
+    C = np.array([[1, 0], [0, 1]], dtype=int)
+    D = np.array([[0, 0], [0, 0]], dtype=int)
+
+    return A, B, C, D
+
+
+def test_sys_matrices(student_sol: callable, master_sol: callable) -> bool:
+    """
+    Check if the student solution is correct for sys_matrices().
+
+    Parameters:
+    - ``student_sol`` (function): A function that returns the student's solution.
+    - ``master_sol`` (function): A function that returns the master solution.
+
+    Returns:
+    - bool: A boolean indicating if the student solution is correct.
+    """
+    try:
+        student = student_sol()
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol()
+    assert np.allclose(student[0], master[0]), "A matrix is incorrect."
+    assert np.allclose(student[1], master[1]), "B matrix is incorrect."
+    assert np.allclose(student[2], master[2]), "C matrix is incorrect."
+    assert np.allclose(student[3], master[3]), "D matrix is incorrect."
+
+    print("Student solution is correct.")
+    return True
+
+
+def sol_poles(A_: np.ndarray, B_: np.ndarray, C_: np.array, D_=np.array) -> np.array:
+    """
+    Determine the poles the system.
+
+    Parameters:
+    - ``A_`` (np.ndarray): The A matrix of the system.
+    - ``B_`` (np.ndarray): The B matrix of the system.
+    - ``C_`` (np.ndarray): The C matrix of the system.
+    - ``D_`` (np.ndarray): The D matrix of the system.
+
+    Returns:
+    - np.array: The poles of the system.
+    """
+    return ct.poles(ct.StateSpace(A_, B_, C_, D_))
+
+
+def test_poles(student_sol: callable, master_sol: callable) -> bool:
+    """
+    Unit tests for checking the implementation of sol_poles. This function should calculate the poles of the system.
+    """
+
+    passed_tests = 0
+    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
+    B1 = np.array([[1, 2], [5, 6], [3, 4]])
+    C1 = np.array([[1, -2, 1]])
+    D1 = np.array([[1, 3]])
+    try:
+        student = student_sol(A1, B1, C1, D1)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A1, B1, C1, D1)
+    if not np.array_equal(student, master, equal_nan=True):
+        print("Test failed: The poles are incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    A2 = np.array([[0, 3], [0, 0]], dtype=int)
+    B2 = np.array([[0, 0], [0, 1]], dtype=int)
+    C2 = np.array([[1, 0], [0, 1]], dtype=int)
+    D2 = np.array([[0, 0], [0, 0]], dtype=int)
+    try:
+        student = student_sol(A2, B2, C2, D2)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A2, B2, C2, D2)
+    if not np.array_equal(student, master, equal_nan=True):
+        print("Test failed: The poles are incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
+    B3 = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
+    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
+    D3 = np.array([[0, 0], [0, 0], [0, 0]], dtype=int)
+    try:
+        student = student_sol(A3, B3, C3, D3)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A3, B3, C3, D3)
+    if not np.array_equal(student, master, equal_nan=True):
+        print("Test failed: The poles are incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    print("Passed tests:", passed_tests, " out of 3")
+    return passed_tests == 3
+
+
+def sol_num_inputs(B_: np.ndarray) -> int:
+    """
+    Determine the number of inputs for the system.
+
+    Parameters:
+    - ``B_`` (np.ndarray): The B matrix of the system.
+
+    Returns:
+    - int: The number of inputs for the system.
+    """
+    return B_.shape[1]
+
+
+def sol_num_outputs(C_: np.ndarray) -> int:
+    """
+    Determine the number of outputs for the system.
+
+    Parameters:
+    - ``C_`` (np.ndarray): The C matrix of the system.
+
+    Returns:
+    - int: The number of outputs for the system.
+    """
+    return C_.shape[0]
+
+
+def test_num_inputs_outputs(student_num_inputs: callable, student_num_outputs: callable, master_num_inputs: callable,
+                            master_num_outputs: callable) -> bool:
+    """
+    Check if the student solution is correct for num_inputs() and num_outputs().
+
+    Parameters:
+    - ``student_num_inputs`` (function): A function that returns the student's solution for num_inputs().
+    - ``student_num_outputs`` (function): A function that returns the student's solution for num_outputs().
+    - ``master_num_inputs`` (function): A function that returns the master solution for num_inputs().
+    - ``master_num_outputs`` (function): A function that returns the master solution for num_outputs().
+
+    Returns:
+    - bool: A boolean indicating if the student solution is correct.
+    """
+    B_ = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
+    C_ = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
+
+    try:
+        student_inputs = student_num_inputs(B_)
+        student_outputs = student_num_outputs(C_)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+
+    master_inputs = master_num_inputs(B_)
+    master_outputs = master_num_outputs(C_)
+    assert student_inputs == master_inputs, "The number of inputs is incorrect: {student_inputs} != {master_inputs}"
+    assert student_outputs == master_outputs, "The number of outputs is incorrect: {student_outputs} != {master_outputs}"
+
+    print("Student solution is correct.")
+    return True
+
+
+def sol_calc_tf_symb(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray) -> sp.Matrix:
+    """
+    Calculate the transfer function of the system using symbolic mathematics.
+
+    Parameters:
+    - ``A`` (np.ndarray): The A matrix of the system.
+    - ``B`` (np.ndarray): The B matrix of the system.
+    - ``C`` (np.ndarray): The C matrix of the system.
+    - ``D`` (np.ndarray): The D matrix of the system.
+
+    Returns:
+    - sp.Matrix: The transfer function of the system.
+    """
+    # Check dimensions of A, B, C, D
+    assert A.shape[0] == A.shape[1], "A must be a square matrix"
+    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
+    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
+    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
+
+    # define identity matrix of appropriate size
+    s = sp.symbols('s')
+    I = np.eye(A.shape[0])
+
+    # calculate the inverse of (s*I - A)
+    term = sp.Matrix(s * I - A)
+    inv_term = term.inv()
+
+    # calculate P_s
+    transferfunction = np.dot(C, np.dot(inv_term, B)) + D
+
+    # simplify the answer so that there are no double fractions
+    transferfunction = sp.simplify(transferfunction)
+
+    return transferfunction
+
+
+def test_calc_tf_symb(student_sol: callable, master_sol: callable) -> bool:
+    """
+    Unit tests for checking the implementation of calc_symb_sol(). This function should symbolically calculate the MIMO transfer function given A, B, C, and D matrices.
+    """
+
+    passed_tests = 0
+    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
+    B1 = np.array([[1, 2], [5, 6], [3, 4]])
+    C1 = np.array([[1, -2, 1]])
+    D1 = np.array([[1, 3]])
+    try:
+        student = student_sol(A1, B1, C1, D1)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A1, B1, C1, D1)
+    if (student != master):
+        print("Test failed: The transfer function is incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    A2 = np.array([[0, 3], [0, 0]], dtype=int)
+    B2 = np.array([[0, 0], [0, 1]], dtype=int)
+    C2 = np.array([[1, 0], [0, 1]], dtype=int)
+    D2 = np.array([[0, 0], [0, 0]], dtype=int)
+    try:
+        student = student_sol(A2, B2, C2, D2)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A2, B2, C2, D2)
+    if (student != master):
+        print("Test failed: The transfer function is incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
+    B3 = np.array([[1, 0], [0, 1], [0, 0]], dtype=int)
+    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
+    D3 = np.array([[0, 0], [0, 0], [0, 0]], dtype=int)
+    try:
+        student = student_sol(A3, B3, C3, D3)
+    except Exception as e:
+        print(f"Error: {e}")
+        return False
+    master = master_sol(A3, B3, C3, D3)
+    if (student != master):
+        print("Test failed: The transfer function is incorrect.")
+        print("Student's result: ", student)
+        print("Expected result: ", master)
+    else:
+        passed_tests += 1
+
+    print("Passed tests:", passed_tests, " out of 3")
+    return passed_tests == 3
+
+
+def sol_calc_tf_ctrl(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, outputnumber: int = 0) -> Tuple[
+    np.ndarray, np.ndarray, Optional[float]]:
+    """
+    Calculate the transfer function of the system using signal library.
+
+    Parameters:
+    - ``A`` (np.ndarray): The A matrix of the system.
+    - ``B`` (np.ndarray): The B matrix of the system.
+    - ``C`` (np.ndarray): The C matrix of the system.
+    - ``D`` (np.ndarray): The D matrix of the system.
+
+    Returns:
+    - Tuple[np.ndarray, np.ndarray, Optional[float]]: The transfer function of the system.
+    """
+    # Check dimensions of A, B, C, D
+    assert A.shape[0] == A.shape[1], "A must be a square matrix"
+    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
+    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
+    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
+
+    transferfunction = signal.ss2tf(A, B, C, D, outputnumber)
+
+    return transferfunction
+
+
+def test_calc_tf_ctrl(student_sol: callable, master_sol: callable) -> bool:
+    """
+    Unit tests for checking the implementation of calc_tf_ctrl(). This function should calculate the MIMO transfer function given A, B, C, and D matrices.
+    """
+
+    passed_tests = 0
+    A1 = np.array([[5, 6, 6], [0, 0, 1], [-5, -5, -6]])
+    B1 = np.array([[1, 2], [5, 6], [3, 4]])
+    C1 = np.array([[1, -2, 1]])
+    D1 = np.array([[1, 3]])
+    num_outputs = 1
+    for i in range(num_outputs):
+        try:
+            student = student_sol(A1, B1, C1, D1, i)
+        except Exception as e:
+            print(f"Error: {e}")
+            return False
+        master = master_sol(A1, B1, C1, D1, i)
+        if (compare_tuples(student, master) == False):
+            print("Test failed: The transfer function for output {i} is incorrect.")
+            print("Student's result: ", student)
+            print("Expected result: ", master)
+        else:
+            passed_tests += 1
+    print("First test series passed")
+
+    A2 = np.array([[0, 3], [0, 0]], dtype=int)
+    B2 = np.array([[0, 0], [0, 1]], dtype=int)
+    C2 = np.array([[1, 0], [0, 1]], dtype=int)
+    D2 = np.array([[0, 0], [0, 0]], dtype=int)
+    num_outputs = 2
+    for i in range(num_outputs):
+        try:
+            student = student_sol(A2, B2, C2, D2, i)
+        except Exception as e:
+            print(f"Error: {e}")
+            return False
+        master = master_sol(A2, B2, C2, D2, i)
+        if (compare_tuples(student, master) == False):
+            print("Test failed: The transfer function for output {i} is incorrect.")
+            print("Student's result: ", student)
+            print("Expected result: ", master)
+        else:
+            passed_tests += 1
+    print("Second test series passed")
+
+    A3 = np.array([[0, 1, 0], [1, 0, 0], [0, 0, 1]], dtype=int)
+    B3 = np.array([[1, 0, 2], [0, 1, 0], [0, 0, 1]], dtype=int)
+    C3 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 1]], dtype=int)
+    D3 = np.array([[0, 0, 0], [0, 0, 0], [0, 0, 0]], dtype=int)
+    num_outputs = 3
+    for i in range(num_outputs):
+        try:
+            student = student_sol(A3, B3, C3, D3, i)
+        except Exception as e:
+            print(f"Error: {e}")
+            return False
+        master = master_sol(A3, B3, C3, D3, i)
+        if (compare_tuples(student, master) == False):
+            print("Test failed: The transfer function is incorrect.")
+            print("Student's result: ", student)
+            print("Expected result: ", master)
+        else:
+            passed_tests += 1
+    print("Third test series passed")
+
+    print("Passed tests:", passed_tests, " out of 6")
+    return passed_tests == 6
+
+
+def compare_tuples(t1: Tuple[np.ndarray, np.ndarray, Optional[float]],
+                   t2: Tuple[np.ndarray, np.ndarray, Optional[float]]) -> bool:
+    return np.array_equal(t1[0], t2[0]) and np.array_equal(t1[1], t2[1])
+
+
+def sol_get_tf(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray) -> Tuple[
+    np.ndarray, signal.TransferFunction, signal.TransferFunction, signal.TransferFunction, signal.TransferFunction]:
+    """
+    Find the individual transfer functions in the transfer function matrix.
+
+    Parameters:
+    - ``A`` (np.ndarray): The A matrix of the system.
+    - ``B`` (np.ndarray): The B matrix of the system.
+    - ``C`` (np.ndarray): The C matrix of the system.
+    - ``D`` (np.ndarray): The D matrix of the system.
+
+    Returns:
+    - Tuple[np.ndarray, TransferFunction, TransferFunction, TransferFunction, TransferFunction]: The individual transfer functions
+    """
+    # Check dimensions of A, B, C, D
+    assert A.shape[0] == A.shape[1], "A must be a square matrix"
+    assert A.shape[0] == B.shape[0], "The number of rows in A and B must be the same"
+    assert A.shape[1] == C.shape[1], "The number of columns in A and C must be the same"
+    assert B.shape[1] == D.shape[1] and C.shape[0] == D.shape[0], "D must be of dimensions (C.shape[0], B.shape[1])"
+
+    tf_output1 = sol_calc_tf_ctrl(A, B, C, D, 0)
+    tf_output2 = sol_calc_tf_ctrl(A, B, C, D, 1)
+
+    den = tf_output1[1]
+
+    tf_11 = signal.TransferFunction(tf_output1[0][0], den)
+    tf_12 = signal.TransferFunction(tf_output2[0][0], den)
+    tf_21 = signal.TransferFunction(tf_output1[0][1], den)
+    tf_22 = signal.TransferFunction(tf_output2[0][1], den)
+
+    return den, tf_11, tf_12, tf_21, tf_22
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/lqg.py` & `cs2solutions-0.8.0/src/cs2solutions/lqg.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-
-def sol_kalman_filter(A: np.ndarray, B: np.ndarray, C: np.ndarray, U: Optional[np.ndarray] = None) -> np.ndarray:
-    """
-    Calculate the L observer gain matrix according to the Kalman Filter definition.
-
-    Parameters:
-    - ``A`` (np.ndarray): State matrix of the system.
-    - ``B`` (np.ndarray): Input matrix of the system.
-    - ``C`` (np.ndarray): Output matrix of the system.
-    - ``U`` (np.ndarray): Noisy input (optional).
-
-    Returns:
-    - ``L`` (np.ndarray): Kalman estimator gain matrix.
-    """
-    # Assert that A, B, C are numpy arrays
-    assert isinstance(A, np.ndarray), "A should be a numpy array"
-    assert isinstance(B, np.ndarray), "B should be a numpy array"
-    assert isinstance(C, np.ndarray), "C should be a numpy array"
-
-    # Assert that A, B, C have correct dimensions
-    assert A.shape[0] == A.shape[1], "A should be a square matrix"
-    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
-    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
-
-    #Process and sensor noise covariance matrices
-    QN = np.cov(U, rowvar=True)[1, 1]
-    RN = QN*10
-
-    # If non gaussian-noise
-    if QN == 0:
-        QN = 1
-        RN = 10
-
-    # Kalman estimator gain
-    L, P, E = ct.lqe(A, B, C, QN, RN)
-    return L
-
-def test_kalman_filter(student_sol: callable, master_sol: callable, U: np.ndarray, shouldprint: bool = True) -> bool:
-    """
-    Test the student's Kalman Filter implementation.
-
-    Parameters:
-    - ``student`` (callable): The student's Kalman Filter function.
-    - ``master`` (callable): The master's Kalman Filter function.
-    - ``U`` (np.ndarray): Noisy input.
-    - ``shouldprint`` (bool): Whether to print the test results.
-
-    Returns:
-    - ``bool``: The test result.
-    """
-    # Define the system matrices
-    A1 = np.array([[0, 1], [-1, -1]])
-    B1 = np.array([[0], [1]])
-    C1 = np.array([[1, 0]])
-
-    passed_tests = 0
-    if student_sol(A1, B1, C1, U) is None:
-        print("Student solution is not implemented yet")
-        return False
-
-    if shouldprint: print("Student 1: " + str(student_sol(A1, B1, C1, U)))
-    if shouldprint: print("Master 1: " + str(master_sol(A1, B1, C1, U)))
-    if np.allclose(student_sol(A1, B1, C1, U), master_sol(A1, B1, C1, U)): passed_tests += 1
-
-    A2 = np.array([[0, 1], [-1, -1]])
-    B2 = np.array([[0], [1]])
-    C2 = np.array([[0, 1]])
-
-    if shouldprint: print("Student 2: " + str(student_sol(A2, B2, C2, U)))
-    if shouldprint: print("Master 2: " + str(master_sol(A2, B2, C2, U)))
-    if np.allclose(student_sol(A2, B2, C2, U), master_sol(A2, B2, C2, U)): passed_tests += 1
-
-    A3 = np.array([[0, 0.1], [0, 0]])
-    B3 = np.array([[0], [1]])
-    C3 = np.array([[1, 0]])
-
-    if shouldprint: print("Student 3: " + str(student_sol(A3, B3, C3, U)))
-    if shouldprint: print("Master 3: " + str(master_sol(A3, B3, C3, U)))
-    if np.allclose(student_sol(A3, B3, C3, U), master_sol(A3, B3, C3, U)): passed_tests += 1
-
-    print("Passed tests:", passed_tests, " out of 3")
-    return passed_tests == 3
-
-
-def kalman_perf_written_ans() -> None:
-    """
-    The Kalman filter performs well with gaussian noise. Process and sensor noise covariance are difficult to estimate in reality. If the mean and the standard deviation of the noise are known, the estimator behaves better.
-    """
-    return None
-
-
-def sol_LQR_K(A: np.ndarray, B: np.ndarray, C: np.ndarray, Q: np.ndarray, R: np.ndarray) -> np.ndarray:
-    """
-    Calculate the LQR controller gain matrix.
-
-    Parameters:
-    - ``A`` (np.ndarray): State matrix of the system.
-    - ``B`` (np.ndarray): Input matrix of the system.
-    - ``C`` (np.ndarray): Output matrix of the system.
-    - ``Q`` (np.ndarray): State cost matrix.
-    - ``R`` (np.ndarray): Input cost matrix.
-
-    Returns:
-    - ``K`` (np.ndarray): LQR controller gain matrix.
-    """
-    # Assert that A, B, C, Q, R are numpy arrays
-    assert isinstance(A, np.ndarray), "A should be a numpy array"
-    assert isinstance(B, np.ndarray), "B should be a numpy array"
-    assert isinstance(C, np.ndarray), "C should be a numpy array"
-    assert isinstance(Q, np.ndarray), "Q should be a numpy array"
-    assert isinstance(R, np.ndarray), "R should be a numpy array"
-
-    # Assert that A, B, C, Q, R have correct dimensions
-    assert A.shape[0] == A.shape[1], "A should be a square matrix"
-    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
-    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
-    assert Q.shape[0] == Q.shape[1] == A.shape[0], "Q should be a square matrix with the same dimensions as A"
-    assert R.shape[0] == B.shape[1], "R should be a square matrix with the same number of rows as the number of columns in B"
-
-    sys = ct.ss(A, B, C, 0)
-    K, S, E = ct.lqr(sys, Q, R)
-    return K
-
-
-def test_LQR_K(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Test the student's LQR controller gain implementation.
-
-    Parameters:
-    - ``student`` (callable): The student's LQR controller gain function.
-    - ``master`` (callable): The master's LQR controller gain function.
-    - ``shouldprint`` (bool): Whether to print the test results.
-
-    Returns:
-    - ``bool``: The test result.
-    """
-    # Define the system matrices
-    A1 = np.array([[0, 1], [-1, -1]])
-    B1 = np.array([[0], [1]])
-    C1 = np.array([[1, 0]])
-    # Straight path
-    Q = 1 * np.eye(2,dtype=int)
-    R = np.array([10])
-    # Easy/Hard path
-    #Q = np.array([[1000,0],[0,10]])
-    #R = np.array([1])
-
-    passed_tests = 0
-    if student_sol(A1, B1, C1, Q, R) is None:
-        print("Student solution is not implemented yet")
-        return False
-
-    if shouldprint: print("Student 1: " + str(student_sol(A1, B1, C1, Q, R)))
-    if shouldprint: print("Master 1: " + str(master_sol(A1, B1, C1, Q, R)))
-    if np.allclose(student_sol(A1, B1, C1, Q, R), master_sol(A1, B1, C1, Q, R)): passed_tests += 1
-
-    A2 = np.array([[0, 1], [-1, -1]])
-    B2 = np.array([[0], [1]])
-    C2 = np.array([[0, 1]])
-
-    if shouldprint: print("Student 2: " + str(student_sol(A2, B2, C2, Q, R)))
-    if shouldprint: print("Master 2: " + str(master_sol(A2, B2, C2, Q, R)))
-    if np.allclose(student_sol(A2, B2, C2, Q, R), master_sol(A2, B2, C2, Q, R)): passed_tests += 1
-
-    A3 = np.array([[0, 0.1], [0, 0]])
-    B3 = np.array([[0], [1]])
-    C3 = np.array([[1, 0]])
-
-    if shouldprint: print("Student 3: " + str(student_sol(A3, B3, C3, Q, R)))
-    if shouldprint: print("Master 3: " + str(master_sol(A3, B3, C3, Q, R)))
-    if np.allclose(student_sol(A3, B3, C3, Q, R), master_sol(A3, B3, C3, Q, R)): passed_tests += 1
-
-    print("Passed tests:", passed_tests, " out of 3")
-    return passed_tests == 3
-    
-
-def sol_stability_analysis(A: np.ndarray, B: np.ndarray, C: np.ndarray, K: np.ndarray, L: np.ndarray, shouldprint: bool = False) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Calculate the eigenvalues of the controlled and observed systems.
-
-    Parameters:
-    - ``A`` (np.ndarray): State matrix of the system.
-    - ``B`` (np.ndarray): Input matrix of the system.
-    - ``C`` (np.ndarray): Output matrix of the system.
-    - ``K`` (np.ndarray): LQR controller gain matrix.
-    - ``L`` (np.ndarray): Kalman estimator gain matrix.
-    - ``shouldprint`` (bool): Whether to print the eigenvalues.
-
-    Returns:
-    - ``con_eig`` (np.ndarray): Controller eigenvalues.
-    - ``obs_eig`` (np.ndarray): Observer eigenvalues.
-    """
-    # Assert that A, B, C, K, L are numpy arrays
-    assert isinstance(A, np.ndarray), "A should be a numpy array"
-    assert isinstance(B, np.ndarray), "B should be a numpy array"
-    assert isinstance(C, np.ndarray), "C should be a numpy array"
-    assert isinstance(K, np.ndarray), "K should be a numpy array"
-    assert isinstance(L, np.ndarray), "L should be a numpy array"
-
-    # Assert that A, B, C, K, L have correct dimensions
-    assert A.shape[0] == A.shape[1], "A should be a square matrix"
-    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
-    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
-    assert K.shape[0] == B.shape[1], "The number of rows in K should be equal to the number of columns in B"
-    assert L.shape[1] == C.shape[0], "The number of columns in L should be equal to the number of rows in C"
-
-
-    con_eig = np.linalg.eigvals(A - B @ K)
-    obs_eig = np.linalg.eigvals(A - L @ C)
-
-    if shouldprint: print("Controller eigenvalues:", con_eig, "Observer eigenvalues:", obs_eig)
-    return con_eig, obs_eig
-
-
-def sol_close_loop(A: np.ndarray, B: np.ndarray, C: np.ndarray, Q: np.ndarray, R: np.ndarray, U: np.ndarray) -> ct.StateSpace:
-    """
-    Calculate the state-space representation of the closed-loop system.
-
-    Parameters:
-    - ``A`` (np.ndarray): State matrix of the system.
-    - ``B`` (np.ndarray): Input matrix of the system.
-    - ``C`` (np.ndarray): Output matrix of the system.
-    - ``Q`` (np.ndarray): State cost matrix.
-    - ``R`` (np.ndarray): Input cost matrix.
-    - ``U`` (np.ndarray): Noisy input.
-
-    Returns:
-    - ``sys_cl`` (StateSpace): Closed-loop system.
-    """
-    # Assert that A, B, C, Q, R are numpy arrays
-    assert isinstance(A, np.ndarray), "A should be a numpy array"
-    assert isinstance(B, np.ndarray), "B should be a numpy array"
-    assert isinstance(C, np.ndarray), "C should be a numpy array"
-    assert isinstance(Q, np.ndarray), "Q should be a numpy array"
-    assert isinstance(R, np.ndarray), "R should be a numpy array"
-
-    # Assert that A, B, C, Q, R have correct dimensions
-    assert A.shape[0] == A.shape[1], "A should be a square matrix"
-    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
-    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
-    assert Q.shape[0] == Q.shape[1] == A.shape[0], "Q should be a square matrix with the same dimensions as A"
-    assert R.shape[0] == B.shape[1], "R should be a square matrix with the same number of rows as the number of columns in B"
-
-    # Calculate K and L using LQR and Kalman Filter respectively
-    K = sol_LQR_K(A, B, C, Q, R)
-    L = sol_kalman_filter(A, B, C, U)
-
-    LC = L @ C
-    BK = B @ K
-    KS = -np.linalg.inv(C @ np.linalg.inv(A-BK) @ B)
-
-    # Create the SISO closed-loop system
-    A_s = np.concatenate((A-BK, BK), axis=1)
-    A_i = np.concatenate((np.zeros_like(LC), A-LC), axis=1)
-    A_cl = np.concatenate((A_s, A_i), axis=0)
-    B_cl = np.block([[B @ KS], [np.zeros_like(B)]])
-    C_cl = np.block([[C, np.zeros_like(C)]])
-    D_cl = 0
-
-    closed_loop_sys_sol = ct.ss(A_cl, B_cl, C_cl, D_cl)
-    return closed_loop_sys_sol
-
-
-def test_close_loop(student_sol: callable, master_sol: callable, U: np.ndarray, shouldprint: bool = True) -> bool:
-    """
-    Test the student's closed-loop system implementation.
-
-    Parameters:
-    - ``student`` (callable): The student's closed-loop system function.
-    - ``master`` (callable): The master's closed-loop system function.
-    - ``U`` (np.ndarray): Noisy input.
-    - ``shouldprint`` (bool): Whether to print the test results.
-
-    Returns:
-    - ``bool``: The test result.
-    """
-    # Define the system matrices
-    A = np.array([[0, 1], [-1, -1]])
-    B = np.array([[0], [1]])
-    C = np.array([[1, 0]])
-    # Straight path
-    Q = 1 * np.eye(2,dtype=int)
-    R = np.array([10])
-
-    passed_tests = 0
-    if student_sol(A, B, C, Q, R, U) is None:
-        print("Student solution is not implemented yet")
-        return False
-    
-    student_solution = student_sol(A, B, C, Q, R, U)
-    master_solution = master_sol(A, B, C, Q, R, U)
-
-    if shouldprint: print("Student A_cl: " + str(student_solution.A))
-    if shouldprint: print("Master A_cl: " + str(master_solution.A))
-    if np.allclose(student_solution.A, master_solution.A): passed_tests += 1
-
-    if shouldprint: print("Student B_cl: " + str(student_solution.B))
-    if shouldprint: print("Master B_cl: " + str(master_solution.B))
-    if np.allclose(student_solution.B, master_solution.B): passed_tests += 1
-
-    if shouldprint: print("Student C_cl: " + str(student_solution.C))
-    if shouldprint: print("Master C_cl: " + str(master_solution.C))
-    if np.allclose(student_solution.C, master_solution.C): passed_tests += 1
-
-    if shouldprint: print("Student D_cl: " + str(student_solution.D))
-    if shouldprint: print("Master D_cl: " + str(master_solution.D))
-    if np.allclose(student_solution.D, master_solution.D): passed_tests += 1
-
-    print("Passed tests:", passed_tests, " out of 4")
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+
+def sol_kalman_filter(A: np.ndarray, B: np.ndarray, C: np.ndarray, U: Optional[np.ndarray] = None) -> np.ndarray:
+    """
+    Calculate the L observer gain matrix according to the Kalman Filter definition.
+
+    Parameters:
+    - ``A`` (np.ndarray): State matrix of the system.
+    - ``B`` (np.ndarray): Input matrix of the system.
+    - ``C`` (np.ndarray): Output matrix of the system.
+    - ``U`` (np.ndarray): Noisy input (optional).
+
+    Returns:
+    - ``L`` (np.ndarray): Kalman estimator gain matrix.
+    """
+    # Assert that A, B, C are numpy arrays
+    assert isinstance(A, np.ndarray), "A should be a numpy array"
+    assert isinstance(B, np.ndarray), "B should be a numpy array"
+    assert isinstance(C, np.ndarray), "C should be a numpy array"
+
+    # Assert that A, B, C have correct dimensions
+    assert A.shape[0] == A.shape[1], "A should be a square matrix"
+    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
+    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
+
+    #Process and sensor noise covariance matrices
+    QN = np.cov(U, rowvar=True)[1, 1]
+    RN = QN*10
+
+    # If non gaussian-noise
+    if QN == 0:
+        QN = 1
+        RN = 10
+
+    # Kalman estimator gain
+    L, P, E = ct.lqe(A, B, C, QN, RN)
+    return L
+
+def test_kalman_filter(student_sol: callable, master_sol: callable, U: np.ndarray, shouldprint: bool = True) -> bool:
+    """
+    Test the student's Kalman Filter implementation.
+
+    Parameters:
+    - ``student`` (callable): The student's Kalman Filter function.
+    - ``master`` (callable): The master's Kalman Filter function.
+    - ``U`` (np.ndarray): Noisy input.
+    - ``shouldprint`` (bool): Whether to print the test results.
+
+    Returns:
+    - ``bool``: The test result.
+    """
+    # Define the system matrices
+    A1 = np.array([[0, 1], [-1, -1]])
+    B1 = np.array([[0], [1]])
+    C1 = np.array([[1, 0]])
+
+    passed_tests = 0
+    if student_sol(A1, B1, C1, U) is None:
+        print("Student solution is not implemented yet")
+        return False
+
+    if shouldprint: print("Student 1: " + str(student_sol(A1, B1, C1, U)))
+    if shouldprint: print("Master 1: " + str(master_sol(A1, B1, C1, U)))
+    if np.allclose(student_sol(A1, B1, C1, U), master_sol(A1, B1, C1, U)): passed_tests += 1
+
+    A2 = np.array([[0, 1], [-1, -1]])
+    B2 = np.array([[0], [1]])
+    C2 = np.array([[0, 1]])
+
+    if shouldprint: print("Student 2: " + str(student_sol(A2, B2, C2, U)))
+    if shouldprint: print("Master 2: " + str(master_sol(A2, B2, C2, U)))
+    if np.allclose(student_sol(A2, B2, C2, U), master_sol(A2, B2, C2, U)): passed_tests += 1
+
+    A3 = np.array([[0, 0.1], [0, 0]])
+    B3 = np.array([[0], [1]])
+    C3 = np.array([[1, 0]])
+
+    if shouldprint: print("Student 3: " + str(student_sol(A3, B3, C3, U)))
+    if shouldprint: print("Master 3: " + str(master_sol(A3, B3, C3, U)))
+    if np.allclose(student_sol(A3, B3, C3, U), master_sol(A3, B3, C3, U)): passed_tests += 1
+
+    print("Passed tests:", passed_tests, " out of 3")
+    return passed_tests == 3
+
+
+def kalman_perf_written_ans() -> None:
+    """
+    The Kalman filter performs well with gaussian noise. Process and sensor noise covariance are difficult to estimate in reality. If the mean and the standard deviation of the noise are known, the estimator behaves better.
+    """
+    return None
+
+
+def sol_LQR_K(A: np.ndarray, B: np.ndarray, C: np.ndarray, Q: np.ndarray, R: np.ndarray) -> np.ndarray:
+    """
+    Calculate the LQR controller gain matrix.
+
+    Parameters:
+    - ``A`` (np.ndarray): State matrix of the system.
+    - ``B`` (np.ndarray): Input matrix of the system.
+    - ``C`` (np.ndarray): Output matrix of the system.
+    - ``Q`` (np.ndarray): State cost matrix.
+    - ``R`` (np.ndarray): Input cost matrix.
+
+    Returns:
+    - ``K`` (np.ndarray): LQR controller gain matrix.
+    """
+    # Assert that A, B, C, Q, R are numpy arrays
+    assert isinstance(A, np.ndarray), "A should be a numpy array"
+    assert isinstance(B, np.ndarray), "B should be a numpy array"
+    assert isinstance(C, np.ndarray), "C should be a numpy array"
+    assert isinstance(Q, np.ndarray), "Q should be a numpy array"
+    assert isinstance(R, np.ndarray), "R should be a numpy array"
+
+    # Assert that A, B, C, Q, R have correct dimensions
+    assert A.shape[0] == A.shape[1], "A should be a square matrix"
+    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
+    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
+    assert Q.shape[0] == Q.shape[1] == A.shape[0], "Q should be a square matrix with the same dimensions as A"
+    assert R.shape[0] == B.shape[1], "R should be a square matrix with the same number of rows as the number of columns in B"
+
+    sys = ct.ss(A, B, C, 0)
+    K, S, E = ct.lqr(sys, Q, R)
+    return K
+
+
+def test_LQR_K(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Test the student's LQR controller gain implementation.
+
+    Parameters:
+    - ``student`` (callable): The student's LQR controller gain function.
+    - ``master`` (callable): The master's LQR controller gain function.
+    - ``shouldprint`` (bool): Whether to print the test results.
+
+    Returns:
+    - ``bool``: The test result.
+    """
+    # Define the system matrices
+    A1 = np.array([[0, 1], [-1, -1]])
+    B1 = np.array([[0], [1]])
+    C1 = np.array([[1, 0]])
+    # Straight path
+    Q = 1 * np.eye(2,dtype=int)
+    R = np.array([10])
+    # Easy/Hard path
+    #Q = np.array([[1000,0],[0,10]])
+    #R = np.array([1])
+
+    passed_tests = 0
+    if student_sol(A1, B1, C1, Q, R) is None:
+        print("Student solution is not implemented yet")
+        return False
+
+    if shouldprint: print("Student 1: " + str(student_sol(A1, B1, C1, Q, R)))
+    if shouldprint: print("Master 1: " + str(master_sol(A1, B1, C1, Q, R)))
+    if np.allclose(student_sol(A1, B1, C1, Q, R), master_sol(A1, B1, C1, Q, R)): passed_tests += 1
+
+    A2 = np.array([[0, 1], [-1, -1]])
+    B2 = np.array([[0], [1]])
+    C2 = np.array([[0, 1]])
+
+    if shouldprint: print("Student 2: " + str(student_sol(A2, B2, C2, Q, R)))
+    if shouldprint: print("Master 2: " + str(master_sol(A2, B2, C2, Q, R)))
+    if np.allclose(student_sol(A2, B2, C2, Q, R), master_sol(A2, B2, C2, Q, R)): passed_tests += 1
+
+    A3 = np.array([[0, 0.1], [0, 0]])
+    B3 = np.array([[0], [1]])
+    C3 = np.array([[1, 0]])
+
+    if shouldprint: print("Student 3: " + str(student_sol(A3, B3, C3, Q, R)))
+    if shouldprint: print("Master 3: " + str(master_sol(A3, B3, C3, Q, R)))
+    if np.allclose(student_sol(A3, B3, C3, Q, R), master_sol(A3, B3, C3, Q, R)): passed_tests += 1
+
+    print("Passed tests:", passed_tests, " out of 3")
+    return passed_tests == 3
+    
+
+def sol_stability_analysis(A: np.ndarray, B: np.ndarray, C: np.ndarray, K: np.ndarray, L: np.ndarray, shouldprint: bool = False) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Calculate the eigenvalues of the controlled and observed systems.
+
+    Parameters:
+    - ``A`` (np.ndarray): State matrix of the system.
+    - ``B`` (np.ndarray): Input matrix of the system.
+    - ``C`` (np.ndarray): Output matrix of the system.
+    - ``K`` (np.ndarray): LQR controller gain matrix.
+    - ``L`` (np.ndarray): Kalman estimator gain matrix.
+    - ``shouldprint`` (bool): Whether to print the eigenvalues.
+
+    Returns:
+    - ``con_eig`` (np.ndarray): Controller eigenvalues.
+    - ``obs_eig`` (np.ndarray): Observer eigenvalues.
+    """
+    # Assert that A, B, C, K, L are numpy arrays
+    assert isinstance(A, np.ndarray), "A should be a numpy array"
+    assert isinstance(B, np.ndarray), "B should be a numpy array"
+    assert isinstance(C, np.ndarray), "C should be a numpy array"
+    assert isinstance(K, np.ndarray), "K should be a numpy array"
+    assert isinstance(L, np.ndarray), "L should be a numpy array"
+
+    # Assert that A, B, C, K, L have correct dimensions
+    assert A.shape[0] == A.shape[1], "A should be a square matrix"
+    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
+    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
+    assert K.shape[0] == B.shape[1], "The number of rows in K should be equal to the number of columns in B"
+    assert L.shape[1] == C.shape[0], "The number of columns in L should be equal to the number of rows in C"
+
+
+    con_eig = np.linalg.eigvals(A - B @ K)
+    obs_eig = np.linalg.eigvals(A - L @ C)
+
+    if shouldprint: print("Controller eigenvalues:", con_eig, "Observer eigenvalues:", obs_eig)
+    return con_eig, obs_eig
+
+
+def sol_close_loop(A: np.ndarray, B: np.ndarray, C: np.ndarray, Q: np.ndarray, R: np.ndarray, U: np.ndarray) -> ct.StateSpace:
+    """
+    Calculate the state-space representation of the closed-loop system.
+
+    Parameters:
+    - ``A`` (np.ndarray): State matrix of the system.
+    - ``B`` (np.ndarray): Input matrix of the system.
+    - ``C`` (np.ndarray): Output matrix of the system.
+    - ``Q`` (np.ndarray): State cost matrix.
+    - ``R`` (np.ndarray): Input cost matrix.
+    - ``U`` (np.ndarray): Noisy input.
+
+    Returns:
+    - ``sys_cl`` (StateSpace): Closed-loop system.
+    """
+    # Assert that A, B, C, Q, R are numpy arrays
+    assert isinstance(A, np.ndarray), "A should be a numpy array"
+    assert isinstance(B, np.ndarray), "B should be a numpy array"
+    assert isinstance(C, np.ndarray), "C should be a numpy array"
+    assert isinstance(Q, np.ndarray), "Q should be a numpy array"
+    assert isinstance(R, np.ndarray), "R should be a numpy array"
+
+    # Assert that A, B, C, Q, R have correct dimensions
+    assert A.shape[0] == A.shape[1], "A should be a square matrix"
+    assert B.shape[0] == A.shape[0], "The number of rows in B should be equal to the number of rows in A"
+    assert C.shape[1] == A.shape[0], "The number of columns in C should be equal to the number of rows in A"
+    assert Q.shape[0] == Q.shape[1] == A.shape[0], "Q should be a square matrix with the same dimensions as A"
+    assert R.shape[0] == B.shape[1], "R should be a square matrix with the same number of rows as the number of columns in B"
+
+    # Calculate K and L using LQR and Kalman Filter respectively
+    K = sol_LQR_K(A, B, C, Q, R)
+    L = sol_kalman_filter(A, B, C, U)
+
+    LC = L @ C
+    BK = B @ K
+    KS = -np.linalg.inv(C @ np.linalg.inv(A-BK) @ B)
+
+    # Create the SISO closed-loop system
+    A_s = np.concatenate((A-BK, BK), axis=1)
+    A_i = np.concatenate((np.zeros_like(LC), A-LC), axis=1)
+    A_cl = np.concatenate((A_s, A_i), axis=0)
+    B_cl = np.block([[B @ KS], [np.zeros_like(B)]])
+    C_cl = np.block([[C, np.zeros_like(C)]])
+    D_cl = 0
+
+    closed_loop_sys_sol = ct.ss(A_cl, B_cl, C_cl, D_cl)
+    return closed_loop_sys_sol
+
+
+def test_close_loop(student_sol: callable, master_sol: callable, U: np.ndarray, shouldprint: bool = True) -> bool:
+    """
+    Test the student's closed-loop system implementation.
+
+    Parameters:
+    - ``student`` (callable): The student's closed-loop system function.
+    - ``master`` (callable): The master's closed-loop system function.
+    - ``U`` (np.ndarray): Noisy input.
+    - ``shouldprint`` (bool): Whether to print the test results.
+
+    Returns:
+    - ``bool``: The test result.
+    """
+    # Define the system matrices
+    A = np.array([[0, 1], [-1, -1]])
+    B = np.array([[0], [1]])
+    C = np.array([[1, 0]])
+    # Straight path
+    Q = 1 * np.eye(2,dtype=int)
+    R = np.array([10])
+
+    passed_tests = 0
+    if student_sol(A, B, C, Q, R, U) is None:
+        print("Student solution is not implemented yet")
+        return False
+    
+    student_solution = student_sol(A, B, C, Q, R, U)
+    master_solution = master_sol(A, B, C, Q, R, U)
+
+    if shouldprint: print("Student A_cl: " + str(student_solution.A))
+    if shouldprint: print("Master A_cl: " + str(master_solution.A))
+    if np.allclose(student_solution.A, master_solution.A): passed_tests += 1
+
+    if shouldprint: print("Student B_cl: " + str(student_solution.B))
+    if shouldprint: print("Master B_cl: " + str(master_solution.B))
+    if np.allclose(student_solution.B, master_solution.B): passed_tests += 1
+
+    if shouldprint: print("Student C_cl: " + str(student_solution.C))
+    if shouldprint: print("Master C_cl: " + str(master_solution.C))
+    if np.allclose(student_solution.C, master_solution.C): passed_tests += 1
+
+    if shouldprint: print("Student D_cl: " + str(student_solution.D))
+    if shouldprint: print("Master D_cl: " + str(master_solution.D))
+    if np.allclose(student_solution.D, master_solution.D): passed_tests += 1
+
+    print("Passed tests:", passed_tests, " out of 4")
     return passed_tests == 4
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/morse.py` & `cs2solutions-0.8.0/src/cs2solutions/morse.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,399 +1,399 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-
-# Visualize the Noise signal in Morse-Transmission
-def plot_noise_signal(t_cont: np.array, rand_noise: np.array,
-            t_cont_start: int, t_cont_end: int) -> None:
-  """
-  Plot the continuous noise signal.
-  
-  Parameters:
-   - ``t_cont`` (np.array): Array of time values for the continuous signal.
-   - ``rand_noise`` (np.array): Array of amplitude values for the continuous noise signal.
-   - ``t_cont_start`` (int): Start time for the x-axis.
-   - ``t_cont_end`` (int): End time for the x-axis.
-
-  Returns:
-   - None
-  """
-  
-  plt.figure(figsize=(5, 3))
-  plt.title("(Continuous) Noise")
-  plt.axhline(y=0, color='g', linestyle='-')
-  plt.plot(t_cont, rand_noise)
-  plt.xticks(np.arange(t_cont_start, t_cont_end))
-  plt.xlabel('Time (s)')
-  plt.ylabel('Amplitude')
-  plt.show()
-    
-  return None
-
-
-# Define the morse code dictionary.
-MORSE_CODE_DICT = { 'A':'.-', 'B':'-...',
-                    'C':'-.-.', 'D':'-..', 'E':'.',
-                    'F':'..-.', 'G':'--.', 'H':'....',
-                    'I':'..', 'J':'.---', 'K':'-.-',
-                    'L':'.-..', 'M':'--', 'N':'-.',
-                    'O':'---', 'P':'.--.', 'Q':'--.-',
-                    'R':'.-.', 'S':'...', 'T':'-',
-                    'U':'..-', 'V':'...-', 'W':'.--',
-                    'X':'-..-', 'Y':'-.--', 'Z':'--..',
-                    '1':'.----', '2':'..---', '3':'...--',
-                    '4':'....-', '5':'.....', '6':'-....',
-                    '7':'--...', '8':'---..', '9':'----.',
-                    '0':'-----', ', ':'--..--', '.':'.-.-.-',
-                    '?':'..--..', '/':'-..-.', '-':'-....-',
-                    '(':'-.--.', ')':'-.--.-','':''}
-
-# Function to encrypt the string according to the Morse code chart.
-def encrypt(message: str) -> str:
-    """
-    Encrypts a given message using Morse code.
-
-    Parameters:
-    - ``message`` (str): The message to be encrypted.
-
-    Returns:
-    - ``cipher`` (str): The encrypted message in Morse code.
-    """
-    cipher = ''
-    for letter in message:
-        if letter != ' ':
-            cipher += MORSE_CODE_DICT[letter] + ' '
-        else:
-            cipher += ' '
-
-    return cipher
-
-# Function to decrypt the string from Morse to English.
-def decrypt(message: str) -> str:
-    """
-    Decrypts a message encoded in Morse code.
-    
-    Parameters:
-     - ``message`` (str): The Morse code message to be decrypted.
-        
-    Returns:
-     - ``decipher`` (str): The decrypted message in English.
-    """
-    
-    # Extra space added at the end to access the last morse code.
-    message += ' '
-    
-    # Variables to keep track of the Morse code and the English translation.
-    decipher = ''
-    citext = ''
-    for letter in message:
- 
-        # Checks for space.
-        if (letter != ' '):
-            # Counter to keep track of space.
-            i = 0
- 
-            # Storing Morse code of a single character.
-            citext += letter
- 
-        # In the case of space.
-        else:
-            # If i = 1 that indicates a new character.
-            i += 1
- 
-            # If i = 2 that indicates a new word.
-            if i == 2 :
-                 # Adding space to separate words.
-                decipher += ' '
-            else:
-                try:
-                    # Accessing the keys using their values (reverse of encryption).
-                    decipher += list(MORSE_CODE_DICT.keys())[list(MORSE_CODE_DICT.values()).index(citext)]
-                    citext = ''
-                except:
-                    pass
- 
-    return decipher
-
-
-def code_to_signal(t_cont: np.array,                
-                   morse_code: str,
-                   morse_com_freq: float) -> np.array:
-  """
-  Standardized signal to represent the Morse Signal:
-
-  ".": 1 ON & 1 OFF
-  "-": 2 ON & 1 OFF
-  " ": 2 OFF
-
-  This Function that turns these into ON and OFF signals.
-
-  Parameters: 
-  - ``t_cont`` (np.array): Array of time values for the continuous signal.
-  - ``morse_code`` (str): The Morse code message to be transmitted.
-  - ``morse_com_freq`` (float): The frequency of the Morse code signal.
-      
-  Output: 
-  - ``morse_signal`` (np.array): The Morse code signal.
-  """
-  
-  # A calculation turns the frequency to the period in [s].
-  # The period defines how long a "." is (represented in signal as on).
-  period = 1/morse_com_freq
-  
-  # Generate an empty array matching the size of the continuous time array for signal data storage.
-  morse_signal = np.zeros(t_cont.size)
-
-  e = 0
-  i = 0
-
-  # Check if counter within both array.
-  while ((e < len(morse_code)) and (i < t_cont.size - 1)):
-    # If yes, read the current character in Morse code and determine what to write on the signal data storage.
-    
-    """
-    ".": 1 ON & 1 OFF
-    "-": 2 ON & 1 OFF
-    " ": 2 OFF
-    """
-    
-    if morse_code[e] == '.':
-
-      on_end = t_cont[i] + period
-      off_end = t_cont[i] + 2*period
-
-    if morse_code[e] == "-":
-      on_end = t_cont[i] + 2*period
-      off_end = t_cont[i] + 3*period
-
-    if morse_code[e] == " ":
-      on_end = t_cont[i]
-      off_end = t_cont[i] + 2*period
-
-    # After determining how long and what to write, write the signal on the data array.
-    while ((t_cont[i] < on_end) and (i < t_cont.size - 1)):
-      # Write the ON state.
-      morse_signal[i] = 1
-      i = i + 1
-
-    while ((t_cont[i] <= off_end) and (i < t_cont.size - 1)):
-      # Write the OFF state.
-      morse_signal[i] = 0
-      i = i + 1
-
-    e = e + 1
-    
-  return morse_signal
-
-
-def signal_to_code(t_dis: np.array,
-                   dis_morse_signal: np.array,
-                   morse_com_freq: float) -> str:
-  """
-  This function decodes signals back to Morse Code.
-
-  Parameters:
-  - ``t_dis`` (np.array): Discrete-Time Time Array.
-  - ``dis_morse_signal`` (np.array): Discrete-Time Signal Value Array. Signal must be normalized to 1 and 0.
-  - ``morse_com_freq`` (float): Morse Communication Frequency.
-
-  Returns:
-  - ``morse_code`` (str): Morse Code consisting of ".", "-", and " ".
-  """
-
-  # A calculation turns the frequency to the period in [s].
-  # The period defines how long a "." is (represented in signal as on).
-  period = 1/morse_com_freq
-  
-  i = 0
-  p = 0
-  state = 0
-  hold_time = 0
-  code = ""
-  
-  while i < len(t_dis)-1:
-    
-    while state == 0:
-      # Check if the element index is still in the range of the data array.
-      # Check if the state remains unchanged, hence signal is smaller than 0.8.
-      # Check if the OFF is being held for too long, might mean that the message has ended.
-      while i < len(t_dis)-1 and dis_morse_signal[i] < 0.8 and hold_time < 20*period:
-        # Move to the next element.
-        i += 1
-        hold_time = t_dis[i] - t_dis[p]
-        
-      if i >= len(t_dis)-1:
-        # This condition indicates wether the index is over the total elements, in which case the function should be terminated.
-        return code
-      
-      if hold_time >= 10*period:
-        # This condition indicates the message ends.
-        code += "  "
-        return code
-      
-      # Otherwise it indicates a state change from OFF to ON, and the message continues.
-      if hold_time >= 0.6*period:
-        if hold_time >= 2.5*period:
-          if hold_time >= 4.2*period:
-            code += "  "
-          else:
-            code += " "
-      # Otherwise it was just a break to start another character.
-      
-      # Change the state to ON.
-      state = 1
-      # Refresh the timer.
-      p = i
-      
-    while state == 1:
-      # Check if the element index is still in the range of the data array.
-      # Check if the state remains unchanged, hence signal is higher than 0.8.
-      # Check if the ON is being held for too long, might mean that the message has an error.
-      while i < len(t_dis)-1 and dis_morse_signal[i] >= 0.8 and hold_time < 20*period:
-        # Move to the next element.
-        i += 1
-        hold_time = t_dis[i] - t_dis[p]
-      
-      if i >= len(t_dis)-1:
-        # This condition indicates the index is over the total elements, in which case the function should be terminated.
-        return code
-      
-      if hold_time >= 20*period:
-        # This condition indicates the message ends.
-        code += "  "
-        return code
-      
-      # Otherwise it indicates a state change from ON to OFF, and the message continues.
-      if hold_time >= 0.6*period:
-        # If ON time is longer than 1.8, it's a "-".
-        if hold_time >= 1.6*period:
-          code += "-"
-        else:
-          code += "."
-      
-      # Change the state to OFF.
-      state = 0
-      # Refresh the timer.
-      p = i
-    
-  return code
-
-
-def butter_lowpass_filter(data: np.array,
-                          cutoff_frequency: float,
-                          sampling_frequency: float,
-                          order: int) -> np.array:
-    """
-    Apply a low-pass Butterworth filter to the input signal data.
-    
-    Parameters:
-    - ``data`` (np.array): 1D array of signal values.
-    - ``cutoff_frequency`` (float): Cutoff frequency of the filter.
-    - ``sampling_frequency`` (float): Sampling frequency of the data.
-    - ``order`` (int): Order of the low-pass transfer function.
-    
-    Returns:
-    - ``filtered_data`` (np.array): 1D array of filtered signal values.
-    """
-    nyquist = 0.5 * sampling_frequency
-    normal_cutoff = cutoff_frequency / nyquist
-    b, a = butter(order, normal_cutoff, btype='low', analog=False)
-    # Apply the filter to the signal.
-    filtered_data = lfilter(b, a, data)
-    return filtered_data
-
-
-def analog_digital_converter(t_cont: np.array,
-                             cont_signal: np.array,
-                             freq: float,
-                             t_or_s: str) -> np.array:
-    """
-    This function selectively picks the data points from the continuous data array to simulate signal sampling.
-    
-    Parameters:
-    - ``t_cont`` (np.array): Continues-Time Time Array.
-    - ``cont_signal`` (np.array): Continues-Time Signal Value Array.
-    - ``freq`` (float): ADC Sampling Frequency.
-    - ``t_or_s`` (str): Array generator selector. 't' to generate a Discrete-Time Time Array, 's' to generate a Discrete-Time Signal Value Array.
-    
-    Returns:
-    - ``t_dis`` OR ``dis_signal`` (np.array): Discrete-Time Time Array or Discrete-Time Signal Value Array, depending on the value of t_or_s.
-    """
-    
-    # Converting the Sampling frequency to the sampling period.
-    period = 1/freq
- 
-    # Initialize an empty array to store the time data for discrete time.
-    t_dis = np.zeros(t_cont.size)
-    dis_signal = np.zeros(t_cont.size)
- 
-    i = 0
-    p = 0
-    e = 0
- 
-    # Check if the element index is still in the range of the time array.
-    while i < len(t_cont)-1:
-        
-        # Collect data from continuous time and write it to the sensor data array.
-        t_dis[e] = t_cont[i]
-        dis_signal[e] = cont_signal[i]
-        
-        # Move to the next element in the sensor data.
-        e += 1
-        
-        # Keep skipping the time till the next time to be sampled by the sensor.
-        # While checking if the element is still in range.
-        while (t_cont[i] < t_cont[p] + period) and (i < len(t_cont)-1):
-            i += 1
-        # We skipped a period in continuous time, now it is time to collect data.
-        p = i
-    
-    # If dis_time wanted, return dis_time array.
-    if t_or_s == "t":
-        return t_dis   
-    
-    # If dis_signal wanted, return dis_signal array
-    if t_or_s == "s":
-        return dis_signal
- 
-    return None
-    
-
-def data_normalization_sol(data_raw: np.array,
-                           min: float,
-                           normalization: float,
-                           idle: float) -> np.array:
-    """
-    Normalize the input data array to discrete values of 1 or 0.
-    If the signal value is higher than or equal to the minimum threshold, it is normalized to the normalization value.
-    If the signal value is lower than the minimum threshold, it is normalized to the idle value.
-    
-    Parameters:
-    - ``data_raw`` (np.array): 1D array of raw data points.
-    - ``min`` (float): Minimum threshold for normalization.
-    - ``normalization`` (float): Value to normalize to when the signal value is higher than or equal to the minimum threshold.
-    - ``idle`` (float): Value to normalize to when the signal value is lower than the minimum threshold.
-    
-    Returns:
-    - ``data_norm`` (np.array): 1D array of filtered data points with the same size as the raw data array.
-    """
-    # Create an array to save the filtered data with the same size as the raw data array.
-    data_norm = np.zeros(data_raw.size)
-    
-    # Check each value and normalize or set it to the idle value in the filtered data array.
-    for i in range(data_raw.size):
-        if min <= data_raw[i]:
-            data_norm[i] = normalization
-        else:
-            data_norm[i] = idle
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+
+# Visualize the Noise signal in Morse-Transmission
+def plot_noise_signal(t_cont: np.array, rand_noise: np.array,
+            t_cont_start: int, t_cont_end: int) -> None:
+  """
+  Plot the continuous noise signal.
+  
+  Parameters:
+   - ``t_cont`` (np.array): Array of time values for the continuous signal.
+   - ``rand_noise`` (np.array): Array of amplitude values for the continuous noise signal.
+   - ``t_cont_start`` (int): Start time for the x-axis.
+   - ``t_cont_end`` (int): End time for the x-axis.
+
+  Returns:
+   - None
+  """
+  
+  plt.figure(figsize=(5, 3))
+  plt.title("(Continuous) Noise")
+  plt.axhline(y=0, color='g', linestyle='-')
+  plt.plot(t_cont, rand_noise)
+  plt.xticks(np.arange(t_cont_start, t_cont_end))
+  plt.xlabel('Time (s)')
+  plt.ylabel('Amplitude')
+  plt.show()
+    
+  return None
+
+
+# Define the morse code dictionary.
+MORSE_CODE_DICT = { 'A':'.-', 'B':'-...',
+                    'C':'-.-.', 'D':'-..', 'E':'.',
+                    'F':'..-.', 'G':'--.', 'H':'....',
+                    'I':'..', 'J':'.---', 'K':'-.-',
+                    'L':'.-..', 'M':'--', 'N':'-.',
+                    'O':'---', 'P':'.--.', 'Q':'--.-',
+                    'R':'.-.', 'S':'...', 'T':'-',
+                    'U':'..-', 'V':'...-', 'W':'.--',
+                    'X':'-..-', 'Y':'-.--', 'Z':'--..',
+                    '1':'.----', '2':'..---', '3':'...--',
+                    '4':'....-', '5':'.....', '6':'-....',
+                    '7':'--...', '8':'---..', '9':'----.',
+                    '0':'-----', ', ':'--..--', '.':'.-.-.-',
+                    '?':'..--..', '/':'-..-.', '-':'-....-',
+                    '(':'-.--.', ')':'-.--.-','':''}
+
+# Function to encrypt the string according to the Morse code chart.
+def encrypt(message: str) -> str:
+    """
+    Encrypts a given message using Morse code.
+
+    Parameters:
+    - ``message`` (str): The message to be encrypted.
+
+    Returns:
+    - ``cipher`` (str): The encrypted message in Morse code.
+    """
+    cipher = ''
+    for letter in message:
+        if letter != ' ':
+            cipher += MORSE_CODE_DICT[letter] + ' '
+        else:
+            cipher += ' '
+
+    return cipher
+
+# Function to decrypt the string from Morse to English.
+def decrypt(message: str) -> str:
+    """
+    Decrypts a message encoded in Morse code.
+    
+    Parameters:
+     - ``message`` (str): The Morse code message to be decrypted.
+        
+    Returns:
+     - ``decipher`` (str): The decrypted message in English.
+    """
+    
+    # Extra space added at the end to access the last morse code.
+    message += ' '
+    
+    # Variables to keep track of the Morse code and the English translation.
+    decipher = ''
+    citext = ''
+    for letter in message:
+ 
+        # Checks for space.
+        if (letter != ' '):
+            # Counter to keep track of space.
+            i = 0
+ 
+            # Storing Morse code of a single character.
+            citext += letter
+ 
+        # In the case of space.
+        else:
+            # If i = 1 that indicates a new character.
+            i += 1
+ 
+            # If i = 2 that indicates a new word.
+            if i == 2 :
+                 # Adding space to separate words.
+                decipher += ' '
+            else:
+                try:
+                    # Accessing the keys using their values (reverse of encryption).
+                    decipher += list(MORSE_CODE_DICT.keys())[list(MORSE_CODE_DICT.values()).index(citext)]
+                    citext = ''
+                except:
+                    pass
+ 
+    return decipher
+
+
+def code_to_signal(t_cont: np.array,                
+                   morse_code: str,
+                   morse_com_freq: float) -> np.array:
+  """
+  Standardized signal to represent the Morse Signal:
+
+  ".": 1 ON & 1 OFF
+  "-": 2 ON & 1 OFF
+  " ": 2 OFF
+
+  This Function that turns these into ON and OFF signals.
+
+  Parameters: 
+  - ``t_cont`` (np.array): Array of time values for the continuous signal.
+  - ``morse_code`` (str): The Morse code message to be transmitted.
+  - ``morse_com_freq`` (float): The frequency of the Morse code signal.
+      
+  Output: 
+  - ``morse_signal`` (np.array): The Morse code signal.
+  """
+  
+  # A calculation turns the frequency to the period in [s].
+  # The period defines how long a "." is (represented in signal as on).
+  period = 1/morse_com_freq
+  
+  # Generate an empty array matching the size of the continuous time array for signal data storage.
+  morse_signal = np.zeros(t_cont.size)
+
+  e = 0
+  i = 0
+
+  # Check if counter within both array.
+  while ((e < len(morse_code)) and (i < t_cont.size - 1)):
+    # If yes, read the current character in Morse code and determine what to write on the signal data storage.
+    
+    """
+    ".": 1 ON & 1 OFF
+    "-": 2 ON & 1 OFF
+    " ": 2 OFF
+    """
+    
+    if morse_code[e] == '.':
+
+      on_end = t_cont[i] + period
+      off_end = t_cont[i] + 2*period
+
+    if morse_code[e] == "-":
+      on_end = t_cont[i] + 2*period
+      off_end = t_cont[i] + 3*period
+
+    if morse_code[e] == " ":
+      on_end = t_cont[i]
+      off_end = t_cont[i] + 2*period
+
+    # After determining how long and what to write, write the signal on the data array.
+    while ((t_cont[i] < on_end) and (i < t_cont.size - 1)):
+      # Write the ON state.
+      morse_signal[i] = 1
+      i = i + 1
+
+    while ((t_cont[i] <= off_end) and (i < t_cont.size - 1)):
+      # Write the OFF state.
+      morse_signal[i] = 0
+      i = i + 1
+
+    e = e + 1
+    
+  return morse_signal
+
+
+def signal_to_code(t_dis: np.array,
+                   dis_morse_signal: np.array,
+                   morse_com_freq: float) -> str:
+  """
+  This function decodes signals back to Morse Code.
+
+  Parameters:
+  - ``t_dis`` (np.array): Discrete-Time Time Array.
+  - ``dis_morse_signal`` (np.array): Discrete-Time Signal Value Array. Signal must be normalized to 1 and 0.
+  - ``morse_com_freq`` (float): Morse Communication Frequency.
+
+  Returns:
+  - ``morse_code`` (str): Morse Code consisting of ".", "-", and " ".
+  """
+
+  # A calculation turns the frequency to the period in [s].
+  # The period defines how long a "." is (represented in signal as on).
+  period = 1/morse_com_freq
+  
+  i = 0
+  p = 0
+  state = 0
+  hold_time = 0
+  code = ""
+  
+  while i < len(t_dis)-1:
+    
+    while state == 0:
+      # Check if the element index is still in the range of the data array.
+      # Check if the state remains unchanged, hence signal is smaller than 0.8.
+      # Check if the OFF is being held for too long, might mean that the message has ended.
+      while i < len(t_dis)-1 and dis_morse_signal[i] < 0.8 and hold_time < 20*period:
+        # Move to the next element.
+        i += 1
+        hold_time = t_dis[i] - t_dis[p]
+        
+      if i >= len(t_dis)-1:
+        # This condition indicates wether the index is over the total elements, in which case the function should be terminated.
+        return code
+      
+      if hold_time >= 10*period:
+        # This condition indicates the message ends.
+        code += "  "
+        return code
+      
+      # Otherwise it indicates a state change from OFF to ON, and the message continues.
+      if hold_time >= 0.6*period:
+        if hold_time >= 2.5*period:
+          if hold_time >= 4.2*period:
+            code += "  "
+          else:
+            code += " "
+      # Otherwise it was just a break to start another character.
+      
+      # Change the state to ON.
+      state = 1
+      # Refresh the timer.
+      p = i
+      
+    while state == 1:
+      # Check if the element index is still in the range of the data array.
+      # Check if the state remains unchanged, hence signal is higher than 0.8.
+      # Check if the ON is being held for too long, might mean that the message has an error.
+      while i < len(t_dis)-1 and dis_morse_signal[i] >= 0.8 and hold_time < 20*period:
+        # Move to the next element.
+        i += 1
+        hold_time = t_dis[i] - t_dis[p]
+      
+      if i >= len(t_dis)-1:
+        # This condition indicates the index is over the total elements, in which case the function should be terminated.
+        return code
+      
+      if hold_time >= 20*period:
+        # This condition indicates the message ends.
+        code += "  "
+        return code
+      
+      # Otherwise it indicates a state change from ON to OFF, and the message continues.
+      if hold_time >= 0.6*period:
+        # If ON time is longer than 1.8, it's a "-".
+        if hold_time >= 1.6*period:
+          code += "-"
+        else:
+          code += "."
+      
+      # Change the state to OFF.
+      state = 0
+      # Refresh the timer.
+      p = i
+    
+  return code
+
+
+def butter_lowpass_filter(data: np.array,
+                          cutoff_frequency: float,
+                          sampling_frequency: float,
+                          order: int) -> np.array:
+    """
+    Apply a low-pass Butterworth filter to the input signal data.
+    
+    Parameters:
+    - ``data`` (np.array): 1D array of signal values.
+    - ``cutoff_frequency`` (float): Cutoff frequency of the filter.
+    - ``sampling_frequency`` (float): Sampling frequency of the data.
+    - ``order`` (int): Order of the low-pass transfer function.
+    
+    Returns:
+    - ``filtered_data`` (np.array): 1D array of filtered signal values.
+    """
+    nyquist = 0.5 * sampling_frequency
+    normal_cutoff = cutoff_frequency / nyquist
+    b, a = butter(order, normal_cutoff, btype='low', analog=False)
+    # Apply the filter to the signal.
+    filtered_data = lfilter(b, a, data)
+    return filtered_data
+
+
+def analog_digital_converter(t_cont: np.array,
+                             cont_signal: np.array,
+                             freq: float,
+                             t_or_s: str) -> np.array:
+    """
+    This function selectively picks the data points from the continuous data array to simulate signal sampling.
+    
+    Parameters:
+    - ``t_cont`` (np.array): Continues-Time Time Array.
+    - ``cont_signal`` (np.array): Continues-Time Signal Value Array.
+    - ``freq`` (float): ADC Sampling Frequency.
+    - ``t_or_s`` (str): Array generator selector. 't' to generate a Discrete-Time Time Array, 's' to generate a Discrete-Time Signal Value Array.
+    
+    Returns:
+    - ``t_dis`` OR ``dis_signal`` (np.array): Discrete-Time Time Array or Discrete-Time Signal Value Array, depending on the value of t_or_s.
+    """
+    
+    # Converting the Sampling frequency to the sampling period.
+    period = 1/freq
+ 
+    # Initialize an empty array to store the time data for discrete time.
+    t_dis = np.zeros(t_cont.size)
+    dis_signal = np.zeros(t_cont.size)
+ 
+    i = 0
+    p = 0
+    e = 0
+ 
+    # Check if the element index is still in the range of the time array.
+    while i < len(t_cont)-1:
+        
+        # Collect data from continuous time and write it to the sensor data array.
+        t_dis[e] = t_cont[i]
+        dis_signal[e] = cont_signal[i]
+        
+        # Move to the next element in the sensor data.
+        e += 1
+        
+        # Keep skipping the time till the next time to be sampled by the sensor.
+        # While checking if the element is still in range.
+        while (t_cont[i] < t_cont[p] + period) and (i < len(t_cont)-1):
+            i += 1
+        # We skipped a period in continuous time, now it is time to collect data.
+        p = i
+    
+    # If dis_time wanted, return dis_time array.
+    if t_or_s == "t":
+        return t_dis   
+    
+    # If dis_signal wanted, return dis_signal array
+    if t_or_s == "s":
+        return dis_signal
+ 
+    return None
+    
+
+def data_normalization_sol(data_raw: np.array,
+                           min: float,
+                           normalization: float,
+                           idle: float) -> np.array:
+    """
+    Normalize the input data array to discrete values of 1 or 0.
+    If the signal value is higher than or equal to the minimum threshold, it is normalized to the normalization value.
+    If the signal value is lower than the minimum threshold, it is normalized to the idle value.
+    
+    Parameters:
+    - ``data_raw`` (np.array): 1D array of raw data points.
+    - ``min`` (float): Minimum threshold for normalization.
+    - ``normalization`` (float): Value to normalize to when the signal value is higher than or equal to the minimum threshold.
+    - ``idle`` (float): Value to normalize to when the signal value is lower than the minimum threshold.
+    
+    Returns:
+    - ``data_norm`` (np.array): 1D array of filtered data points with the same size as the raw data array.
+    """
+    # Create an array to save the filtered data with the same size as the raw data array.
+    data_norm = np.zeros(data_raw.size)
+    
+    # Check each value and normalize or set it to the idle value in the filtered data array.
+    for i in range(data_raw.size):
+        if min <= data_raw[i]:
+            data_norm[i] = normalization
+        else:
+            data_norm[i] = idle
     return data_norm
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions/norms.py` & `cs2solutions-0.8.0/src/cs2solutions/norms.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,476 +1,476 @@
-from typing import List, Tuple
-
-try:
-    from typing import Optional, List, Tuple
-    import numpy as np
-    import matplotlib.pyplot as plt
-    import control as ct
-    from scipy import signal as sig
-    from scipy.signal import butter, lfilter
-    import unittest as unit
-except ImportError as e:
-    print(f"Error: {e}")
-    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
-
-def sol_vector2norm(vector: np.ndarray) -> float:
-    """
-    Calculate the 2-norm (Euclidean norm) of a NumPy array.
-
-    Parameters:
-    vector (np.ndarray): Input array for which 2-norm is to be calculated.
-
-    Returns:
-    float: The 2-norm of the input array.
-    """
-    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
-        raise ValueError("Input vector is invalid")
-    
-    squared_sum = 0.0
-    for elem in vector:
-        squared_sum += elem**2
-    norm = np.sqrt(squared_sum)
-
-    return norm
-
-def sol_vectorInfnorm(vector: np.ndarray) -> float:
-    """
-    Calculate the infinity-norm (maximum absolute value) of a NumPy array.
-
-    Parameters:
-    vector (np.ndarray): Input array for which infinity-norm is to be calculated.
-
-    Returns:
-    float: The infinity-norm of the input array.
-    """
-    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
-        raise ValueError("Input vector is invalid")
-    
-    max_elem = 0.0
-    for elem in vector:
-        if abs(elem) > max_elem:
-            max_elem = abs(elem)
-
-    return max_elem
-
-def sol_vectorPnorm(vector: np.ndarray, p: float) -> float:
-    """
-    Calculate the p-norm (maximum absolute value) of a NumPy array.
-
-    Parameters:
-    vector (np.ndarray): Input array for which p-norm is to be calculated.
-
-    Returns:
-    float: The p-norm of the input array.
-    """
-    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
-        raise ValueError("Input vector is invalid")
-
-    if p is None:
-        return sol_vector2norm(vector)
-
-    p = float(p)
-    if not isinstance(p, float) or p <= 0.0:
-        raise ValueError("p must be a positive integer")
-
-    norm_sum = 0.0
-    for elem in vector:
-        norm_sum += abs(elem)**p
-    
-    return norm_sum**(1/p)
-
-def test_vector_norm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Unit test function to see if the student solution for 'vector2norm' or 'vectorInfnorm' is correct.
-
-    Parameters:
-    - ``student_sol`` (callable): The student's solution function.
-    - ``master_sol`` (callable): The master solution function.
-    - ``shouldprint`` (bool): Flag to print the test results.
-
-    Returns:
-    bool: The test result.
-    """
-
-    vectors = [
-        np.array([1, 2, 3, 4, 5]),
-        np.array([0, 0, 0, 0, 0]),
-        np.array([1, 1, 1, 1, 1]),
-        np.array([1, 0, 1, 0, 1]),
-        np.array([0, 1, 0, 1, 0]),
-        np.array([2, 4, 3.5, 2, 1.5]),
-        np.array([-1, -2, -3, -4, -5]),
-        np.array([1, -2, 3, -4, 5]),
-        np.array([1.5, 2.5, 3.5, 4.5, 5.5]),
-        np.array([1, 1, 1, 1, 100])
-    ]
-
-    passed_tests = 0
-
-    for i, v in enumerate(vectors):
-        try: 
-            student_result = student_sol(v)
-        except Exception as e:
-            print(f"An error occurred: {e}")
-            continue
-
-        master_result = master_sol(v)
-        correct_answer = master_result == student_result
-
-        if shouldprint and not correct_answer: 
-            print("Error in vector ", i, ": ", v)
-            print("Student's result: ", student_result)
-            print("Expected result: ", master_result)
-
-        passed_tests += 1 if correct_answer else 0
-
-    print("Passed tests: ", passed_tests, " out of 10")
-    return passed_tests == 10
-
-
-def test_vectorPnorm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Unit test function to see if the student solution for 'vectorPnorm' is correct.
-
-    Parameters:
-    - ``student_sol`` (callable): The student's solution function.
-    - ``master_sol`` (callable): The master solution function.
-    - ``shouldprint`` (bool): Flag to print the test results.
-
-    Returns:
-    bool: The test result.
-    """
-
-    vectors = [
-        np.array([1, 2, 3, 4, 5]),
-        np.array([0, 0, 0, 0, 0]),
-        np.array([1, 1, 1, 1, 1]),
-        np.array([1, 0, 1, 0, 1]),
-        np.array([0, 1, 0, 1, 0]),
-        np.array([2, 4, 3.5, 2, 1.5]),
-        np.array([-1, -2, -3, -4, -5]),
-        np.array([1, -2, 3, -4, 5]),
-        np.array([1.5, 2.5, 3.5, 4.5, 5.5]),
-        np.array([1, 1, 1, 1, 100])
-    ]
-    p_values = [1, 2, 3, 4, 5]
-    passed_tests = 0
-    one_incorrect = False
-    for i, v in enumerate(vectors):
-        for p in p_values:
-            try: 
-                student_result = student_sol(v, p)
-            except Exception as e:
-                print(f"An error occurred: {e}")
-                continue
-
-            master_result = master_sol(v, p)
-            correct_answer = master_result == student_result
-
-            if shouldprint and not correct_answer and not one_incorrect: 
-                print("Error in vector ", i, ": ", v, " with p = ", p)
-                print("Student's result: ", student_result)
-                print("Expected result: ", master_result)
-                one_incorrect = True
-
-            passed_tests += 1 if correct_answer else 0
-
-    print("Passed tests: ", passed_tests, " out of 50")
-    return passed_tests == 50
-
-def sol_matrix2norm(matrix: np.ndarray) -> float:
-    """
-    Calculate the 2-norm of a matrix manually.
-
-    Parameters:
-    matrix (numpy.ndarray): Input matrix for which the 2-norm is to be calculated.
-
-    Returns:
-    float: The 2-norm of the input matrix.
-    """
-    if matrix is None or not isinstance(matrix, np.ndarray):
-        raise ValueError("Input matrix is invalid")
-
-    product_matrix = np.dot(matrix.T, matrix)
-    eigenvalues, _ = np.linalg.eig(product_matrix)
-    max_eigenvalue = np.max(eigenvalues)
-    norm = np.sqrt(max_eigenvalue)
-    return norm
-
-def sol_calculate_matrix_singular_values(matrix: np.ndarray) -> np.ndarray:
-    """
-    Calculate the singular values of a matrix manually.
-
-    Parameters:
-    matrix (numpy.ndarray): Input matrix for which the singular values are to be calculated.
-
-    Returns:
-    numpy.ndarray: The singular values of the input matrix.
-    """
-    if matrix is None or not isinstance(matrix, np.ndarray):
-        raise ValueError("Input matrix is invalid")
-
-    product_matrix = np.dot(matrix.T, matrix) if matrix.shape[0] > matrix.shape[1] else np.dot(matrix, matrix.T)
-    eigenvalues, _ = np.linalg.eig(product_matrix)
-    singular_values = np.sqrt(np.abs(eigenvalues))
-    return singular_values
-
-def sol_matrixPnorm(matrix: np.ndarray, p: float) -> float:
-    """
-    Calculate the p-norm of a matrix manually.
-
-    Parameters:
-    matrix (numpy.ndarray): Input matrix for which the p-norm is to be calculated.
-
-    Returns:
-    float: The p-norm of the input matrix.
-    """
-    if matrix is None or not isinstance(matrix, np.ndarray):
-        raise ValueError("Input matrix is invalid")
-    if p is None:
-        return sol_matrix2norm(matrix)
-    p = float(p)
-    if not isinstance(p, float) or p <= 0.0:
-        raise ValueError("p must be a positive integer")
-
-    singular_values = sol_calculate_matrix_singular_values(matrix)
-    norm = np.sum(np.abs(singular_values)**p)**(1.0/p)
-    return norm
-
-def sol_matrixInfnorm(matrix: np.ndarray) -> float:
-    """
-    Calculate the infinity-norm of a matrix manually.
-
-    Parameters:
-    matrix (numpy.ndarray): Input matrix for which the infinity-norm is to be calculated.
-
-    Returns:
-    float: The infinity-norm of the input matrix.
-    """
-    if matrix is None or not isinstance(matrix, np.ndarray):
-        raise ValueError("Input matrix is invalid")
-
-    row_sums = np.sum(np.abs(matrix), axis=1)  # Calculate absolute row sums
-    norm = np.max(row_sums)  # Take the maximum of the absolute row sums
-    return norm
-
-def test_matrix_norm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Unit test function to see if the student solution for 'matrix2norm' or 'matrixInfnorm' is correct.
-
-    Parameters:
-    - ``student_sol`` (callable): The student's solution function.
-    - ``master_sol`` (callable): The master solution function.
-    - ``shouldprint`` (bool): Flag to print the test results.
-
-    Returns:
-    bool: The test result.
-    """
-
-    matrices = [
-        np.array([[1, 2], [3, 4]]),
-        np.array([[0, 0], [0, 0]]),
-        np.array([[1, 1], [1, 1]]),
-        np.array([[1, 0], [0, 1]]),
-        np.array([[0, 1], [1, 0]]),
-        np.array([[2, 4], [3.5, 2]]),
-        np.array([[-1, -2], [-3, -4]]),
-        np.array([[1, -2], [3, -4]]),
-        np.array([[1.5, 2.5], [3.5, 4.5]]),
-        np.array([[1, 1], [1, 100]])
-    ]
-
-    passed_tests = 0
-
-    for i, m in enumerate(matrices):
-        try: 
-            student_result = student_sol(m)
-        except Exception as e:
-            print(f"An error occurred: {e}")
-            continue
-
-        master_result = master_sol(m)
-        correct_answer = master_result == student_result
-
-        if shouldprint and not correct_answer: 
-            print("Error in matrix ", i, ": ", m)
-            print("Student's result: ", student_result)
-            print("Expected result: ", master_result)
-
-        passed_tests += 1 if correct_answer else 0
-
-    print("Passed tests: ", passed_tests, " out of 10")
-    return passed_tests == 10
-
-def test_matrixPnorm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
-    """
-    Unit test function to see if the student solution for 'matrixPnorm' is correct.
-
-    Parameters:
-    - ``student_sol`` (callable): The student's solution function.
-    - ``master_sol`` (callable): The master solution function.
-    - ``shouldprint`` (bool): Flag to print the test results.
-
-    Returns:
-    bool: The test result.
-    """
-
-    matrices = [
-        np.array([[1, 2], [3, 4]]),
-        np.array([[0, 0], [0, 0]]),
-        np.array([[1, 1], [1, 1]]),
-        np.array([[1, 0], [0, 1]]),
-        np.array([[0, 1], [1, 0]]),
-        np.array([[2, 4], [3.5, 2]]),
-        np.array([[-1, -2], [-3, -4]]),
-        np.array([[1, -2], [3, -4]]),
-        np.array([[1.5, 2.5], [3.5, 4.5]]),
-        np.array([[1, 1], [1, 100]])
-    ]
-    p_values = [1, 2, 3, 4, 5]
-    passed_tests = 0
-    one_incorrect = False
-    for i, m in enumerate(matrices):
-        for p in p_values:
-            try: 
-                student_result = student_sol(m, p)
-            except Exception as e:
-                print(f"An error occurred: {e}")
-                continue
-
-            master_result = master_sol(m, p)
-            correct_answer = master_result == student_result
-
-            if shouldprint and not correct_answer and not one_incorrect: 
-                print("Error in matrix ", i, ": ", m, " with p = ", p)
-                print("Student's result: ", student_result)
-                print("Expected result: ", master_result)
-                one_incorrect = True
-
-            passed_tests += 1 if correct_answer else 0
-
-    print("Passed tests: ", passed_tests, " out of 50")
-    return passed_tests == 50
-
-def sol_signalInfnorm(x: np.ndarray) -> float:
-    return np.max(np.abs(x))
-
-def sol_signal1norm(x: np.ndarray) -> float:
-    return np.sum(np.abs(x))
-
-def sol_signal2norm(x: np.ndarray) -> float:
-    return np.sqrt(np.sum(np.abs(x)**2))
-
-def sol_bauerfike(L: np.ndarray, delL: np.ndarray) -> float:
-    """
-    Calculate $min(||L||_1 ||L^{-1}||_1 \cdot ||\Delta L||_1, ||L||_{\infty} ||L^{-1}||_{\infty} \cdot ||\Delta L||_{\infty})$ 
-
-    Parameters:
-    - L (np.ndarray): The original matrix.
-    - delL (np.ndarray): The perturbation matrix.
-
-    Returns:
-    -> float: The deviation value.
-    """
-
-    if L is None or delL is None or not isinstance(L, np.ndarray) or not isinstance(delL, np.ndarray):
-        raise ValueError("Input matrices are invalid")
-    if L.shape != delL.shape:
-        raise ValueError("Input matrices must be of the same shape")
-
-    norm1 = sol_matrixPnorm(L, 1) * sol_matrixPnorm(np.linalg.inv(L), 1) * sol_matrixPnorm(delL, 1)
-    normInf = sol_matrixInfnorm(L) * sol_matrixInfnorm(np.linalg.inv(L)) * sol_matrixInfnorm(delL)
-    return min(norm1, normInf)
-
-def sol_maxinputdir(A: np.ndarray) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """
-    Find the input and output direction corresponding to the largest singular value.
-
-    Parameters:
-    - A (np.ndarray): The input matrix.
-
-    Returns:
-    -> Tuple[np.ndarray, float, np.ndarray]: The input direction, the largest singular value, and the output direction.
-    """
-
-    U, S, Vt = np.linalg.svd(A)
-    max_index = np.argmax(S)
-    
-    input_dir = Vt[max_index]
-    max_singular_value = S[max_index]
-    output_dir = U[max_index]
-
-    return input_dir, max_singular_value, output_dir
-
-def subplot_svd(A: np.ndarray, i: np.ndarray, j: np.ndarray, k: np.ndarray, v1: np.ndarray, v2: np.ndarray, v3: np.ndarray, dir: np.ndarray = None) -> None:
-    fig1 = plt.figure(figsize=(3, 3))
-    ax1 = fig1.add_subplot(111, projection='3d')
-    ax1.quiver(0, 0, 0, v1[0], v1[1], v1[2], color='k', label='i (1,0,0)')
-    ax1.quiver(0, 0, 0, v2[0], v2[1], v2[2], color='k', label='j (0,1,0)')
-    ax1.quiver(0, 0, 0, v3[0], v3[1], v3[2], color='k', label='k (0,0,1)')
-    if dir is not None:
-        ax1.quiver(0, 0, 0, dir[0], dir[1], dir[2], color='r', label='Input direction')
-
-    # Generate points on the unit sphere
-    u = np.linspace(0, 2 * np.pi, 100)
-    v = np.linspace(0, np.pi, 50)
-    x = np.outer(np.cos(u), np.sin(v))
-    y = np.outer(np.sin(u), np.sin(v))
-    z = np.outer(np.ones_like(u), np.cos(v))
-
-    # Rotate and translate points to align with the given vectors
-    transform_matrix = np.vstack((i, j, k))
-    points = np.vstack((x.flatten(), y.flatten(), z.flatten())).T
-    transformed_points = np.dot(points, transform_matrix)
-
-    ax1.plot_surface(transformed_points[:, 0].reshape(x.shape),
-                    transformed_points[:, 1].reshape(y.shape),
-                    transformed_points[:, 2].reshape(z.shape),
-                    alpha=0.5)
-
-    # Set the aspect ratio of the axes to be equal
-    ax1.set_box_aspect([np.ptp(transformed_points[:, 0]), np.ptp(transformed_points[:, 1]), np.ptp(transformed_points[:, 2])])
-
-    ax1.set_xlabel('X')
-    ax1.set_ylabel('Y')
-    ax1.set_zlabel('Z')
-    plt.show()
-
-def plot_svd3x3(A: np.ndarray) -> None:
-    """
-    Plot the singular values of a matrix.
-
-    Parameters:
-    - A (np.ndarray): The input matrix.
-    """
-    if not isinstance(A, np.ndarray) or len(A.shape) != 2:
-        raise ValueError("Input must be a 2D numpy array")
-    
-    U, S, Vt = np.linalg.svd(A)
-    S = np.diag(S)
-    input_dir, max_singular_value, output_dir = sol_maxinputdir(A)
-
-    i1 = np.array([1, 0, 0])
-    j1 = np.array([0, 1, 0])
-    k1 = np.array([0, 0, 1])
-    subplot_svd(A, i1, j1, k1, i1, j1, k1, input_dir)
-
-    i2 = Vt@i1
-    j2 = Vt@j1
-    k2 = Vt@k1
-    subplot_svd(A, i2, j2, k2, i2, j2, k2, Vt@input_dir)
-
-    i3 = S[0] * i1
-    j3 = S[1] * j1
-    k3 = S[2] * k1
-    v1 = S@Vt@i1
-    v2 = S@Vt@j1
-    v3 = S@Vt@k1
-    subplot_svd(A, i3, j3, k3, v1, v2, v3, S@Vt@input_dir)
-
-    i4 = U@i3
-    j4 = U@j3
-    k4 = U@k3
-    output_dir = U@S@Vt@input_dir
-    subplot_svd(A, i4, j4, k4, U@v1, U@v2, U@v3, output_dir)
-
+from typing import List, Tuple
+
+try:
+    from typing import Optional, List, Tuple
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import control as ct
+    from scipy import signal as sig
+    from scipy.signal import butter, lfilter
+    import unittest as unit
+except ImportError as e:
+    print(f"Error: {e}")
+    print(f"Please install the required packages using the command '!pip install control numpy matplotlib scipy'")
+
+def sol_vector2norm(vector: np.ndarray) -> float:
+    """
+    Calculate the 2-norm (Euclidean norm) of a NumPy array.
+
+    Parameters:
+    vector (np.ndarray): Input array for which 2-norm is to be calculated.
+
+    Returns:
+    float: The 2-norm of the input array.
+    """
+    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
+        raise ValueError("Input vector is invalid")
+    
+    squared_sum = 0.0
+    for elem in vector:
+        squared_sum += elem**2
+    norm = np.sqrt(squared_sum)
+
+    return norm
+
+def sol_vectorInfnorm(vector: np.ndarray) -> float:
+    """
+    Calculate the infinity-norm (maximum absolute value) of a NumPy array.
+
+    Parameters:
+    vector (np.ndarray): Input array for which infinity-norm is to be calculated.
+
+    Returns:
+    float: The infinity-norm of the input array.
+    """
+    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
+        raise ValueError("Input vector is invalid")
+    
+    max_elem = 0.0
+    for elem in vector:
+        if abs(elem) > max_elem:
+            max_elem = abs(elem)
+
+    return max_elem
+
+def sol_vectorPnorm(vector: np.ndarray, p: float) -> float:
+    """
+    Calculate the p-norm (maximum absolute value) of a NumPy array.
+
+    Parameters:
+    vector (np.ndarray): Input array for which p-norm is to be calculated.
+
+    Returns:
+    float: The p-norm of the input array.
+    """
+    if len(vector) == 0 or vector is None or not isinstance(vector, np.ndarray):
+        raise ValueError("Input vector is invalid")
+
+    if p is None:
+        return sol_vector2norm(vector)
+
+    p = float(p)
+    if not isinstance(p, float) or p <= 0.0:
+        raise ValueError("p must be a positive integer")
+
+    norm_sum = 0.0
+    for elem in vector:
+        norm_sum += abs(elem)**p
+    
+    return norm_sum**(1/p)
+
+def test_vector_norm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Unit test function to see if the student solution for 'vector2norm' or 'vectorInfnorm' is correct.
+
+    Parameters:
+    - ``student_sol`` (callable): The student's solution function.
+    - ``master_sol`` (callable): The master solution function.
+    - ``shouldprint`` (bool): Flag to print the test results.
+
+    Returns:
+    bool: The test result.
+    """
+
+    vectors = [
+        np.array([1, 2, 3, 4, 5]),
+        np.array([0, 0, 0, 0, 0]),
+        np.array([1, 1, 1, 1, 1]),
+        np.array([1, 0, 1, 0, 1]),
+        np.array([0, 1, 0, 1, 0]),
+        np.array([2, 4, 3.5, 2, 1.5]),
+        np.array([-1, -2, -3, -4, -5]),
+        np.array([1, -2, 3, -4, 5]),
+        np.array([1.5, 2.5, 3.5, 4.5, 5.5]),
+        np.array([1, 1, 1, 1, 100])
+    ]
+
+    passed_tests = 0
+
+    for i, v in enumerate(vectors):
+        try: 
+            student_result = student_sol(v)
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            continue
+
+        master_result = master_sol(v)
+        correct_answer = master_result == student_result
+
+        if shouldprint and not correct_answer: 
+            print("Error in vector ", i, ": ", v)
+            print("Student's result: ", student_result)
+            print("Expected result: ", master_result)
+
+        passed_tests += 1 if correct_answer else 0
+
+    print("Passed tests: ", passed_tests, " out of 10")
+    return passed_tests == 10
+
+
+def test_vectorPnorm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Unit test function to see if the student solution for 'vectorPnorm' is correct.
+
+    Parameters:
+    - ``student_sol`` (callable): The student's solution function.
+    - ``master_sol`` (callable): The master solution function.
+    - ``shouldprint`` (bool): Flag to print the test results.
+
+    Returns:
+    bool: The test result.
+    """
+
+    vectors = [
+        np.array([1, 2, 3, 4, 5]),
+        np.array([0, 0, 0, 0, 0]),
+        np.array([1, 1, 1, 1, 1]),
+        np.array([1, 0, 1, 0, 1]),
+        np.array([0, 1, 0, 1, 0]),
+        np.array([2, 4, 3.5, 2, 1.5]),
+        np.array([-1, -2, -3, -4, -5]),
+        np.array([1, -2, 3, -4, 5]),
+        np.array([1.5, 2.5, 3.5, 4.5, 5.5]),
+        np.array([1, 1, 1, 1, 100])
+    ]
+    p_values = [1, 2, 3, 4, 5]
+    passed_tests = 0
+    one_incorrect = False
+    for i, v in enumerate(vectors):
+        for p in p_values:
+            try: 
+                student_result = student_sol(v, p)
+            except Exception as e:
+                print(f"An error occurred: {e}")
+                continue
+
+            master_result = master_sol(v, p)
+            correct_answer = master_result == student_result
+
+            if shouldprint and not correct_answer and not one_incorrect: 
+                print("Error in vector ", i, ": ", v, " with p = ", p)
+                print("Student's result: ", student_result)
+                print("Expected result: ", master_result)
+                one_incorrect = True
+
+            passed_tests += 1 if correct_answer else 0
+
+    print("Passed tests: ", passed_tests, " out of 50")
+    return passed_tests == 50
+
+def sol_matrix2norm(matrix: np.ndarray) -> float:
+    """
+    Calculate the 2-norm of a matrix manually.
+
+    Parameters:
+    matrix (numpy.ndarray): Input matrix for which the 2-norm is to be calculated.
+
+    Returns:
+    float: The 2-norm of the input matrix.
+    """
+    if matrix is None or not isinstance(matrix, np.ndarray):
+        raise ValueError("Input matrix is invalid")
+
+    product_matrix = np.dot(matrix.T, matrix)
+    eigenvalues, _ = np.linalg.eig(product_matrix)
+    max_eigenvalue = np.max(eigenvalues)
+    norm = np.sqrt(max_eigenvalue)
+    return norm
+
+def sol_calculate_matrix_singular_values(matrix: np.ndarray) -> np.ndarray:
+    """
+    Calculate the singular values of a matrix manually.
+
+    Parameters:
+    matrix (numpy.ndarray): Input matrix for which the singular values are to be calculated.
+
+    Returns:
+    numpy.ndarray: The singular values of the input matrix.
+    """
+    if matrix is None or not isinstance(matrix, np.ndarray):
+        raise ValueError("Input matrix is invalid")
+
+    product_matrix = np.dot(matrix.T, matrix) if matrix.shape[0] > matrix.shape[1] else np.dot(matrix, matrix.T)
+    eigenvalues, _ = np.linalg.eig(product_matrix)
+    singular_values = np.sqrt(np.abs(eigenvalues))
+    return singular_values
+
+def sol_matrixPnorm(matrix: np.ndarray, p: float) -> float:
+    """
+    Calculate the p-norm of a matrix manually.
+
+    Parameters:
+    matrix (numpy.ndarray): Input matrix for which the p-norm is to be calculated.
+
+    Returns:
+    float: The p-norm of the input matrix.
+    """
+    if matrix is None or not isinstance(matrix, np.ndarray):
+        raise ValueError("Input matrix is invalid")
+    if p is None:
+        return sol_matrix2norm(matrix)
+    p = float(p)
+    if not isinstance(p, float) or p <= 0.0:
+        raise ValueError("p must be a positive integer")
+
+    singular_values = sol_calculate_matrix_singular_values(matrix)
+    norm = np.sum(np.abs(singular_values)**p)**(1.0/p)
+    return norm
+
+def sol_matrixInfnorm(matrix: np.ndarray) -> float:
+    """
+    Calculate the infinity-norm of a matrix manually.
+
+    Parameters:
+    matrix (numpy.ndarray): Input matrix for which the infinity-norm is to be calculated.
+
+    Returns:
+    float: The infinity-norm of the input matrix.
+    """
+    if matrix is None or not isinstance(matrix, np.ndarray):
+        raise ValueError("Input matrix is invalid")
+
+    row_sums = np.sum(np.abs(matrix), axis=1)  # Calculate absolute row sums
+    norm = np.max(row_sums)  # Take the maximum of the absolute row sums
+    return norm
+
+def test_matrix_norm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Unit test function to see if the student solution for 'matrix2norm' or 'matrixInfnorm' is correct.
+
+    Parameters:
+    - ``student_sol`` (callable): The student's solution function.
+    - ``master_sol`` (callable): The master solution function.
+    - ``shouldprint`` (bool): Flag to print the test results.
+
+    Returns:
+    bool: The test result.
+    """
+
+    matrices = [
+        np.array([[1, 2], [3, 4]]),
+        np.array([[0, 0], [0, 0]]),
+        np.array([[1, 1], [1, 1]]),
+        np.array([[1, 0], [0, 1]]),
+        np.array([[0, 1], [1, 0]]),
+        np.array([[2, 4], [3.5, 2]]),
+        np.array([[-1, -2], [-3, -4]]),
+        np.array([[1, -2], [3, -4]]),
+        np.array([[1.5, 2.5], [3.5, 4.5]]),
+        np.array([[1, 1], [1, 100]])
+    ]
+
+    passed_tests = 0
+
+    for i, m in enumerate(matrices):
+        try: 
+            student_result = student_sol(m)
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            continue
+
+        master_result = master_sol(m)
+        correct_answer = master_result == student_result
+
+        if shouldprint and not correct_answer: 
+            print("Error in matrix ", i, ": ", m)
+            print("Student's result: ", student_result)
+            print("Expected result: ", master_result)
+
+        passed_tests += 1 if correct_answer else 0
+
+    print("Passed tests: ", passed_tests, " out of 10")
+    return passed_tests == 10
+
+def test_matrixPnorm(student_sol: callable, master_sol: callable, shouldprint: bool = True) -> bool:
+    """
+    Unit test function to see if the student solution for 'matrixPnorm' is correct.
+
+    Parameters:
+    - ``student_sol`` (callable): The student's solution function.
+    - ``master_sol`` (callable): The master solution function.
+    - ``shouldprint`` (bool): Flag to print the test results.
+
+    Returns:
+    bool: The test result.
+    """
+
+    matrices = [
+        np.array([[1, 2], [3, 4]]),
+        np.array([[0, 0], [0, 0]]),
+        np.array([[1, 1], [1, 1]]),
+        np.array([[1, 0], [0, 1]]),
+        np.array([[0, 1], [1, 0]]),
+        np.array([[2, 4], [3.5, 2]]),
+        np.array([[-1, -2], [-3, -4]]),
+        np.array([[1, -2], [3, -4]]),
+        np.array([[1.5, 2.5], [3.5, 4.5]]),
+        np.array([[1, 1], [1, 100]])
+    ]
+    p_values = [1, 2, 3, 4, 5]
+    passed_tests = 0
+    one_incorrect = False
+    for i, m in enumerate(matrices):
+        for p in p_values:
+            try: 
+                student_result = student_sol(m, p)
+            except Exception as e:
+                print(f"An error occurred: {e}")
+                continue
+
+            master_result = master_sol(m, p)
+            correct_answer = master_result == student_result
+
+            if shouldprint and not correct_answer and not one_incorrect: 
+                print("Error in matrix ", i, ": ", m, " with p = ", p)
+                print("Student's result: ", student_result)
+                print("Expected result: ", master_result)
+                one_incorrect = True
+
+            passed_tests += 1 if correct_answer else 0
+
+    print("Passed tests: ", passed_tests, " out of 50")
+    return passed_tests == 50
+
+def sol_signalInfnorm(x: np.ndarray) -> float:
+    return np.max(np.abs(x))
+
+def sol_signal1norm(x: np.ndarray) -> float:
+    return np.sum(np.abs(x))
+
+def sol_signal2norm(x: np.ndarray) -> float:
+    return np.sqrt(np.sum(np.abs(x)**2))
+
+def sol_bauerfike(L: np.ndarray, delL: np.ndarray) -> float:
+    """
+    Calculate $min(||L||_1 ||L^{-1}||_1 \cdot ||\Delta L||_1, ||L||_{\infty} ||L^{-1}||_{\infty} \cdot ||\Delta L||_{\infty})$ 
+
+    Parameters:
+    - L (np.ndarray): The original matrix.
+    - delL (np.ndarray): The perturbation matrix.
+
+    Returns:
+    -> float: The deviation value.
+    """
+
+    if L is None or delL is None or not isinstance(L, np.ndarray) or not isinstance(delL, np.ndarray):
+        raise ValueError("Input matrices are invalid")
+    if L.shape != delL.shape:
+        raise ValueError("Input matrices must be of the same shape")
+
+    norm1 = sol_matrixPnorm(L, 1) * sol_matrixPnorm(np.linalg.inv(L), 1) * sol_matrixPnorm(delL, 1)
+    normInf = sol_matrixInfnorm(L) * sol_matrixInfnorm(np.linalg.inv(L)) * sol_matrixInfnorm(delL)
+    return min(norm1, normInf)
+
+def sol_maxinputdir(A: np.ndarray) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """
+    Find the input and output direction corresponding to the largest singular value.
+
+    Parameters:
+    - A (np.ndarray): The input matrix.
+
+    Returns:
+    -> Tuple[np.ndarray, float, np.ndarray]: The input direction, the largest singular value, and the output direction.
+    """
+
+    U, S, Vt = np.linalg.svd(A)
+    max_index = np.argmax(S)
+    
+    input_dir = Vt[max_index]
+    max_singular_value = S[max_index]
+    output_dir = U[max_index]
+
+    return input_dir, max_singular_value, output_dir
+
+def subplot_svd(A: np.ndarray, i: np.ndarray, j: np.ndarray, k: np.ndarray, v1: np.ndarray, v2: np.ndarray, v3: np.ndarray, dir: np.ndarray = None) -> None:
+    fig1 = plt.figure(figsize=(3, 3))
+    ax1 = fig1.add_subplot(111, projection='3d')
+    ax1.quiver(0, 0, 0, v1[0], v1[1], v1[2], color='k', label='i (1,0,0)')
+    ax1.quiver(0, 0, 0, v2[0], v2[1], v2[2], color='k', label='j (0,1,0)')
+    ax1.quiver(0, 0, 0, v3[0], v3[1], v3[2], color='k', label='k (0,0,1)')
+    if dir is not None:
+        ax1.quiver(0, 0, 0, dir[0], dir[1], dir[2], color='r', label='Input direction')
+
+    # Generate points on the unit sphere
+    u = np.linspace(0, 2 * np.pi, 100)
+    v = np.linspace(0, np.pi, 50)
+    x = np.outer(np.cos(u), np.sin(v))
+    y = np.outer(np.sin(u), np.sin(v))
+    z = np.outer(np.ones_like(u), np.cos(v))
+
+    # Rotate and translate points to align with the given vectors
+    transform_matrix = np.vstack((i, j, k))
+    points = np.vstack((x.flatten(), y.flatten(), z.flatten())).T
+    transformed_points = np.dot(points, transform_matrix)
+
+    ax1.plot_surface(transformed_points[:, 0].reshape(x.shape),
+                    transformed_points[:, 1].reshape(y.shape),
+                    transformed_points[:, 2].reshape(z.shape),
+                    alpha=0.5)
+
+    # Set the aspect ratio of the axes to be equal
+    ax1.set_box_aspect([np.ptp(transformed_points[:, 0]), np.ptp(transformed_points[:, 1]), np.ptp(transformed_points[:, 2])])
+
+    ax1.set_xlabel('X')
+    ax1.set_ylabel('Y')
+    ax1.set_zlabel('Z')
+    plt.show()
+
+def plot_svd3x3(A: np.ndarray) -> None:
+    """
+    Plot the singular values of a matrix.
+
+    Parameters:
+    - A (np.ndarray): The input matrix.
+    """
+    if not isinstance(A, np.ndarray) or len(A.shape) != 2:
+        raise ValueError("Input must be a 2D numpy array")
+    
+    U, S, Vt = np.linalg.svd(A)
+    S = np.diag(S)
+    input_dir, max_singular_value, output_dir = sol_maxinputdir(A)
+
+    i1 = np.array([1, 0, 0])
+    j1 = np.array([0, 1, 0])
+    k1 = np.array([0, 0, 1])
+    subplot_svd(A, i1, j1, k1, i1, j1, k1, input_dir)
+
+    i2 = Vt@i1
+    j2 = Vt@j1
+    k2 = Vt@k1
+    subplot_svd(A, i2, j2, k2, i2, j2, k2, Vt@input_dir)
+
+    i3 = S[0] * i1
+    j3 = S[1] * j1
+    k3 = S[2] * k1
+    v1 = S@Vt@i1
+    v2 = S@Vt@j1
+    v3 = S@Vt@k1
+    subplot_svd(A, i3, j3, k3, v1, v2, v3, S@Vt@input_dir)
+
+    i4 = U@i3
+    j4 = U@j3
+    k4 = U@k3
+    output_dir = U@S@Vt@input_dir
+    subplot_svd(A, i4, j4, k4, U@v1, U@v2, U@v3, output_dir)
+
     subplot_svd(A, A@i1, A@j1, A@k1, A@i1, A@j1, A@k1, A@input_dir)
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions.egg-info/PKG-INFO` & `cs2solutions-0.8.0/src/cs2solutions.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,720 +1,720 @@
-Metadata-Version: 2.1
-Name: cs2solutions
-Version: 0.7.5
-Summary: A package containing solutions for the CS2 lecture at ETH Zürich
-Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
-Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://idsc.ethz.ch/education/lectures/control-systems-ii.html
-Project-URL: Repository, https://github.com/idsc-frazzoli/cs2solutions
-Project-URL: Notebooks, https://github.com/idsc-frazzoli/CS2-2024-notebooks
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: control
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: sympy
-Requires-Dist: pandas
-
-# [cs2solutions]
-
-Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
-Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
-
-## pip Installation
-The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
-
-```bash
-pip install cs2solutions
-```
-
-Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
-
-## Features
-Contains:
-- Utility functions for control systems, such as plotting and generic formulas
-- Solutions for all notebooks
-- Unit tests to check student implementations of code
-
-
+Metadata-Version: 2.1
+Name: cs2solutions
+Version: 0.8.0
+Summary: A package containing solutions for the CS2 lecture at ETH Zürich
+Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
+Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+        
+Project-URL: Homepage, https://idsc.ethz.ch/education/lectures/control-systems-ii.html
+Project-URL: Repository, https://github.com/idsc-frazzoli/cs2solutions
+Project-URL: Notebooks, https://github.com/idsc-frazzoli/CS2-2024-notebooks
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: control
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: sympy
+Requires-Dist: pandas
+
+# [cs2solutions]
+
+Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
+Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
+
+## pip Installation
+The cs2solutions package can be installed directly using '%pip install cs2solutions' in the Jupyter notebook or 'pip install cs2solutions' in the terminal.
+
+```bash
+pip install cs2solutions
+```
+
+Manual installation guide, such as for code contributions, can be found in the [update guide](UPDATE.md).
+
+## Features
+Contains:
+- Utility functions for control systems, such as plotting and generic formulas
+- Solutions for all notebooks
+- Unit tests to check student implementations of code
+
+
```

### Comparing `cs2solutions-0.7.5/src/cs2solutions.egg-info/SOURCES.txt` & `cs2solutions-0.8.0/src/cs2solutions.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/cs2solutions/__init__.py
 src/cs2solutions/aircraft.py
 src/cs2solutions/cs.py
 src/cs2solutions/cs2bot.py
 src/cs2solutions/decomp.py
 src/cs2solutions/discretization.py
 src/cs2solutions/duckiebot.py
+src/cs2solutions/inf_pkg.py
 src/cs2solutions/intro.py
 src/cs2solutions/intromimo.py
 src/cs2solutions/lqg.py
 src/cs2solutions/lqrfeedback.py
 src/cs2solutions/morse.py
 src/cs2solutions/norms.py
 src/cs2solutions/plot.py
```

