# Comparing `tmp/pc-perf-1.1.6.tar.gz` & `tmp/pc-perf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc-perf-1.1.6.tar", last modified: Wed May  1 19:13:34 2024, max compression
+gzip compressed data, was "pc-perf-1.2.1.tar", last modified: Sat May  4 05:19:24 2024, max compression
```

## Comparing `pc-perf-1.1.6.tar` & `pc-perf-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:13:34.233986 pc-perf-1.1.6/
--rw-rw-rw-   0        0        0    35823 2024-04-20 15:52:03.000000 pc-perf-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      943 2024-05-01 19:13:34.233986 pc-perf-1.1.6/PKG-INFO
--rwxrwxrwx   0        0        0   377856 2024-01-28 09:39:06.000000 pc-perf-1.1.6/PresentMon.exe
--rw-rw-rw-   0        0        0     1272 2024-05-01 18:58:09.000000 pc-perf-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 19:13:34.218357 pc-perf-1.1.6/core/
--rw-rw-rw-   0        0        0     2584 2024-04-28 13:34:36.000000 pc-perf-1.1.6/core/monitor.py
--rw-rw-rw-   0        0        0    10071 2024-05-01 19:12:46.000000 pc-perf-1.1.6/core/pc_tools.py
--rw-rw-rw-   0        0        0     6709 2024-04-21 07:37:00.000000 pc-perf-1.1.6/dao.py
--rw-rw-rw-   0        0        0      664 2024-04-21 15:03:50.000000 pc-perf-1.1.6/log.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:13:34.233986 pc-perf-1.1.6/pc_perf.egg-info/
--rw-rw-rw-   0        0        0      943 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      240 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-05-01 19:13:34.000000 pc-perf-1.1.6/pc_perf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4035 2024-05-01 19:07:42.000000 pc-perf-1.1.6/pc_perf.py
--rw-rw-rw-   0        0        0       42 2024-05-01 19:13:34.233986 pc-perf-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2591 2024-05-01 19:13:08.000000 pc-perf-1.1.6/setup.py
--rw-rw-rw-   0        0        0     1545 2024-04-20 11:36:25.000000 pc-perf-1.1.6/task_handle.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:13:34.218357 pc-perf-1.1.6/test_result/
--rw-rw-rw-   0        0        0    31424 2024-05-01 18:58:09.000000 pc-perf-1.1.6/test_result/index.html
--rw-rw-rw-   0        0        0     2879 2024-04-21 15:04:24.000000 pc-perf-1.1.6/util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.311389 pc-perf-1.2.1/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2024-04-28 09:32:22.000000 pc-perf-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1393 2024-05-04 05:19:24.311177 pc-perf-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)   377856 2024-04-28 09:32:22.000000 pc-perf-1.2.1/PresentMon.exe
+-rw-r--r--   0 root         (0) staff       (20)     1238 2024-04-30 11:28:59.000000 pc-perf-1.2.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.308593 pc-perf-1.2.1/core/
+-rw-r--r--   0 root         (0) staff       (20)     2509 2024-05-03 17:30:18.000000 pc-perf-1.2.1/core/monitor.py
+-rw-r--r--   0 root         (0) staff       (20)     9861 2024-05-03 17:30:18.000000 pc-perf-1.2.1/core/pc_tools.py
+-rw-r--r--   0 root         (0) staff       (20)     6903 2024-05-02 16:29:09.000000 pc-perf-1.2.1/dao.py
+-rw-r--r--   0 root         (0) staff       (20)      648 2024-04-28 09:32:22.000000 pc-perf-1.2.1/log.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.310896 pc-perf-1.2.1/pc_perf.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1393 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      349 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       41 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)      260 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 05:19:24.000000 pc-perf-1.2.1/pc_perf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     4851 2024-05-04 03:07:45.000000 pc-perf-1.2.1/pc_perf.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-04 05:19:24.311433 pc-perf-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2541 2024-05-04 05:19:19.000000 pc-perf-1.2.1/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1625 2024-05-04 03:16:45.000000 pc-perf-1.2.1/task_handle.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-04 05:19:24.309814 pc-perf-1.2.1/test_result/
+-rw-r--r--   0 root         (0) staff       (20)    30701 2024-05-02 16:25:39.000000 pc-perf-1.2.1/test_result/index.html
+-rw-r--r--   0 root         (0) staff       (20)     3868 2024-05-04 03:09:43.000000 pc-perf-1.2.1/util.py
```

### Comparing `pc-perf-1.1.6/LICENSE` & `pc-perf-1.2.1/LICENSE`

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

### Comparing `pc-perf-1.1.6/PresentMon.exe` & `pc-perf-1.2.1/PresentMon.exe`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.6/README.md` & `pc-perf-1.2.1/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# pc_perf
-pc 进程性能测试平台，支持 windows / mac / linux 平台普通进程、window游戏GUI进程的
-cpu、memory、fps（仅支持windowsOpenGL  DirectX 引擎应用 unity u3d应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
-
-# 启动入口
-    方式0（推荐）：
-    直接下载二进制运行：https://github.com/15525730080/pc_perf/releases
-    
-    方式1：
-    git clone https://github.com/15525730080/pc_perf.git
-    pip install -r requirements.txt
-    #需要使用管理员权限启动才可以获取到windows fps ！！！
-    python pc_perf.py 
-    
-    方式2：
-    #需要使用管理员权限启动才可以获取到windows fps ！！！
-    pip install pc-perf
-    python -m pc_perf  
-
-    
-
-# 创建任务
-![image](https://github.com/15525730080/pc_perf/assets/153100629/91995e83-6fc6-4350-84d1-24704f1bccce)
-
-# 任务列表
-![image](https://github.com/15525730080/pc_perf/assets/153100629/10112d4b-3724-4ada-9cb8-df633af302a0)
-
-# 性能报表
-![image](https://github.com/15525730080/pc_perf/assets/153100629/2e28527a-6e5d-487c-8753-8d3483c0f108)
-
-# 开源
-本项目归属：范博洲  
-使用需要关注开源协议
-禁止申请软著、专利 本人已申请
+# pc_perf
+pc 进程性能测试平台，支持 windows / mac / linux 平台普通进程、window游戏GUI进程的
+cpu、memory、fps（仅支持windowsOpenGL  DirectX 引擎应用 unity u3d应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
+
+# 启动入口
+    方式0（推荐）：
+    直接下载二进制运行：https://github.com/15525730080/pc_perf/releases
+    
+    方式1：
+    git clone https://github.com/15525730080/pc_perf.git
+    pip install -r requirements.txt
+    #需要使用管理员权限启动才可以获取到windows fps ！！！
+    python pc_perf.py 
+    
+    方式2：
+    #需要使用管理员权限启动才可以获取到windows fps ！！！
+    pip install pc-perf
+    python -m pc_perf  
+
+    
+
+# 创建任务
+![image](https://github.com/15525730080/pc_perf/assets/153100629/91995e83-6fc6-4350-84d1-24704f1bccce)
+
+# 任务列表
+![image](https://github.com/15525730080/pc_perf/assets/153100629/10112d4b-3724-4ada-9cb8-df633af302a0)
+
+# 性能报表
+![image](https://github.com/15525730080/pc_perf/assets/153100629/2e28527a-6e5d-487c-8753-8d3483c0f108)
+
+# 开源
+本项目归属：范博洲  
+使用需要关注开源协议
+禁止申请软著、专利 本人已申请
```

### Comparing `pc-perf-1.1.6/core/monitor.py` & `pc-perf-1.2.1/core/monitor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import asyncio
-import csv
-import inspect
-import json
-import time
-import traceback
-from pathlib import Path
-
-from log import log as logger
-
-
-def print_json(data, *args, **kwargs):
-    data_json = json.dumps(data)
-    logger.info(data_json, *args, **kwargs)
-
-
-class MonitorIter(object):
-
-    def __init__(self, stop_event):
-        self.stop_event = stop_event
-
-    def __aiter__(self):
-        return self
-
-    def __anext__(self):
-        if self.stop_event.is_set():
-            future = asyncio.Future()
-            future.set_result(None)
-            return future
-        elif not self.stop_event.is_set():
-            raise StopAsyncIteration()
-
-
-class Monitor(object):
-
-    def __init__(self, func, **kwargs):
-        super(Monitor, self).__init__()
-        self.stop_event = asyncio.Event()
-        self.func = func
-        self.kwargs = kwargs
-        self.stop_event.set()
-        self.key_value = kwargs.get("key_value", [])
-        self.name = self.func.__name__
-        self.save_dir = kwargs.get("save_dir")
-        self.is_out = self.kwargs.get("is_out", True)
-        if self.is_out:
-            dir_instance = Path(self.save_dir)
-            if not dir_instance.exists():
-                dir_instance.mkdir()
-            csv_instance = dir_instance.joinpath(self.name + ".csv")
-            self.csv_path = csv_instance.resolve()
-            with open(self.csv_path, "w", encoding="utf-8", newline="") as f:
-                csv_writer = csv.writer(f)
-                csv_writer.writerow(self.key_value)
-            self.key_value = [key.split("(")[0] for key in self.key_value]
-
-    async def run(self):
-        async for _ in MonitorIter(self.stop_event):
-            before_func = time.time()
-            param_names = inspect.signature(self.func).parameters.keys()
-            params = {name: self.kwargs.get(name) for name in param_names}
-            try:
-                res = await self.func(**params)
-                if self.is_out and res:
-                    with open(self.csv_path, "a+", encoding="utf-8", newline="") as f:
-                        csv_writer = csv.writer(f)
-                        csv_writer.writerow([res.get(key, "") for key in self.key_value])
-            except:
-                logger.error(traceback.print_exc())
-            finally:
-                end_func = time.time()
-                if interval_time := (int(end_func) - int(before_func)) <= 1:
-                    await asyncio.sleep(interval_time)
-
-    def stop(self):
-        self.stop_event.clear()
+import asyncio
+import csv
+import inspect
+import json
+import time
+import traceback
+from pathlib import Path
+
+from log import log as logger
+
+
+def print_json(data, *args, **kwargs):
+    data_json = json.dumps(data)
+    logger.info(data_json, *args, **kwargs)
+
+
+class MonitorIter(object):
+
+    def __init__(self, stop_event):
+        self.stop_event = stop_event
+
+    def __aiter__(self):
+        return self
+
+    def __anext__(self):
+        if self.stop_event.is_set():
+            future = asyncio.Future()
+            future.set_result(None)
+            return future
+        elif not self.stop_event.is_set():
+            raise StopAsyncIteration()
+
+
+class Monitor(object):
+
+    def __init__(self, func, **kwargs):
+        super(Monitor, self).__init__()
+        self.stop_event = asyncio.Event()
+        self.func = func
+        self.kwargs = kwargs
+        self.stop_event.set()
+        self.key_value = kwargs.get("key_value", [])
+        self.name = self.func.__name__
+        self.save_dir = kwargs.get("save_dir")
+        self.is_out = self.kwargs.get("is_out", True)
+        if self.is_out:
+            dir_instance = Path(self.save_dir)
+            if not dir_instance.exists():
+                dir_instance.mkdir()
+            csv_instance = dir_instance.joinpath(self.name + ".csv")
+            self.csv_path = csv_instance.resolve()
+            with open(self.csv_path, "w", encoding="utf-8", newline="") as f:
+                csv_writer = csv.writer(f)
+                csv_writer.writerow(self.key_value)
+            self.key_value = [key.split("(")[0] for key in self.key_value]
+
+    async def run(self):
+        async for _ in MonitorIter(self.stop_event):
+            before_func = time.time()
+            param_names = inspect.signature(self.func).parameters.keys()
+            params = {name: self.kwargs.get(name) for name in param_names}
+            try:
+                res = await self.func(**params)
+                if self.is_out and res:
+                    with open(self.csv_path, "a+", encoding="utf-8", newline="") as f:
+                        csv_writer = csv.writer(f)
+                        csv_writer.writerow([res.get(key, "") for key in self.key_value])
+            except:
+                logger.error(traceback.format_exc())
+            finally:
+                end_func = time.time()
+                if interval_time := (int(end_func) - int(before_func)) <= 1:
+                    await asyncio.sleep(interval_time)
+
+    def stop(self):
+        self.stop_event.clear()
```

### Comparing `pc-perf-1.1.6/core/pc_tools.py` & `pc-perf-1.2.1/core/pc_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,276 +1,277 @@
-import asyncio
-import json
-import platform
-import subprocess
-import threading
-import time
-import traceback
-from io import BytesIO
-import psutil
-import pynvml
-from pathlib import Path
-from log import log
-from core.monitor import Monitor
-
-SUPPORT_GPU = True
-try:
-    pynvml.nvmlInit()
-except:
-    traceback.print_exc()
-    log.info("本设备gpu获取不适配")
-    SUPPORT_GPU = False
-from PIL import ImageGrab
-
-
-def print_json(msg):
-    log.info(json.dumps(msg))
-
-
-class WinFps(object):
-    frame_que = list()
-    single_instance = None
-    fps_process = None
-
-    def __init__(self, pid):
-        self.pid = pid
-
-    def __new__(cls, *args, **kwargs):
-        if not cls.single_instance:
-            cls.single_instance = super().__new__(cls)
-        return cls.single_instance
-
-    def fps(self):
-        if not WinFps.fps_process:
-            threading.Thread(target=self.start_fps_collect, args=(self.pid,)).start()
-        if self.check_queue_head_frames_complete():
-            return self.pop_complete_fps()
-
-    @staticmethod
-    def check_queue_head_frames_complete():
-        if not WinFps.frame_que:
-            return False
-        head_time = int(WinFps.frame_que[0])
-        end_time = int(WinFps.frame_que[-1])
-        if head_time == end_time:
-            return False
-        return True
-
-    @staticmethod
-    def pop_complete_fps():
-        head_time = int(WinFps.frame_que[0])
-        complete_fps = []
-        while int(WinFps.frame_que[0]) == head_time:
-            complete_fps.append(WinFps.frame_que.pop(0))
-        return complete_fps
-
-    def start_fps_collect(self, pid):
-        start_fps_collect_time = int(time.time())
-        PresentMon = Path(__file__).parent.parent.joinpath("PresentMon.exe")
-        res_terminate = subprocess.Popen(
-            [PresentMon, "-process_id", str(pid), "-output_stdout", "-stop_existing_session"],
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        WinFps.fps_process = res_terminate
-        res_terminate.stdout.readline()
-        while not res_terminate.poll():
-            line = res_terminate.stdout.readline()
-            if not line:
-                try:
-                    res_terminate.kill()
-                except:
-                    traceback.print_exc()
-                break
-            try:
-                line = line.decode(encoding="utf-8")
-                line_list = line.split(",")
-                print("line ", line_list)
-                WinFps.frame_que.append(start_fps_collect_time + round(float(line_list[7]), 7))
-            except:
-                time.sleep(1)
-                traceback.print_exc()
-
-
-async def sys_info():
-    def real_func():
-        current_platform = platform.system()
-        computer_name = platform.node()
-        res = {"platform": current_platform, "computer_name": computer_name, "time": time.time(),
-               "cpu_cores": psutil.cpu_count(), "ram": "{0}G".format(int(psutil.virtual_memory().total / 1024 ** 3)),
-               "rom": "{0}G".format(int(psutil.disk_usage('/').total / 1024 ** 3))}
-        print_json(res)
-        return res
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func), timeout=10)
-
-
-async def pids():
-    def real_func():
-        process_list = []
-        for proc in psutil.process_iter(attrs=['name', 'pid', 'cmdline', 'username']):
-            try:
-                process_list.append(
-                    {"name": proc.info['name'], "pid": proc.info['pid'], "cmd": proc.info['cmdline'],
-                     "username": proc.username()})
-            except Exception as e:
-                log.error(e)
-        process_list.sort(key=lambda x: x['name'])
-        print_json(process_list)
-        return process_list
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func), timeout=10)
-
-
-async def screenshot(pid, save_dir):
-    def real_func(pid, save_dir):
-        start_time = int(time.time())
-        if pid:
-            window = None
-            if platform.system() == "Windows":
-                import ctypes
-                import pygetwindow as gw
-                def get_pid(hwnd):
-                    pid = ctypes.wintypes.DWORD()
-                    ctypes.windll.user32.GetWindowThreadProcessId(hwnd, ctypes.byref(pid))
-                    return pid.value
-
-                def get_window_by_pid(pid):
-                    for window in gw.getAllWindows():
-                        if get_pid(window._hWnd) == pid:
-                            return window
-                    return None
-
-                window = get_window_by_pid(int(pid))
-            if window:
-                screenshot = ImageGrab.grab(
-                    bbox=(window.left, window.top, window.left + window.width, window.top + window.height),
-                    all_screens=True)
-            else:
-                screenshot = ImageGrab.grab(all_screens=True)
-            if save_dir:
-                dir_instance = Path(save_dir)
-                screenshot_dir = dir_instance.joinpath("screenshot")
-                screenshot_dir.mkdir(exist_ok=True)
-                screenshot.save(screenshot_dir.joinpath(str(start_time) + ".png"), format="PNG")
-            else:
-                output_buffer = BytesIO()
-                screenshot.save(output_buffer, format='PNG')
-                output_buffer.seek(0)  # 重置缓冲区指针
-                image_data = output_buffer.getvalue()
-                return image_data
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func, pid, save_dir), timeout=10)
-
-
-async def cpu(pid):
-    def real_func(pid):
-        start_time = int(time.time())
-        proc = psutil.Process(pid=int(pid))
-        cpu_usage = proc.cpu_percent(interval=1)
-        cpu_count = psutil.cpu_count()
-        res = {"cpu_usage": cpu_usage / cpu_count, "cpu_usage_all": cpu_usage,
-               "cpu_core_num": cpu_count, "time": start_time}
-        print_json(res)
-        return res
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
-
-
-async def memory(pid):
-    def real_func(pid):
-        start_time = int(time.time())
-        process = psutil.Process(int(pid))
-        process_memory_info = process.memory_info()
-        process_memory_usage = process_memory_info.rss / (1024 ** 2)  # In MB
-        memory_info = {"process_memory_usage": process_memory_usage, "time": start_time}
-        print_json(memory_info)
-        return memory_info
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
-
-
-async def fps(pid):
-    if platform.system() != "Windows":
-        return {"type": "fps", "time": int(time.time())}
-    frames = WinFps(pid).fps()
-    if not frames:
-        return frames
-    res = {"type": "fps", "fps": len(frames), "frames": frames, "time": int(frames[0]) if frames else int(time.time())}
-    print_json(res)
-    return res
-
-
-async def gpu(pid):
-    def real_func(pid):
-        pid = int(pid)
-        start_time = int(time.time())
-        if SUPPORT_GPU:
-            device_count = pynvml.nvmlDeviceGetCount()
-            res = None
-            for i in range(device_count):
-                handle = pynvml.nvmlDeviceGetHandleByIndex(i)
-                processes = pynvml.nvmlDeviceGetComputeRunningProcesses(handle)
-                for process in processes:
-                    print(process)
-                    if process.pid == pid:
-                        gpu_Utilization = pynvml.nvmlDeviceGetUtilizationRates(handle)
-                        gpu_utilization_percentage = gpu_Utilization.gpu  # GPU的计算使用率
-                        res = {"gpu": gpu_utilization_percentage, "time": start_time}
-                        print_json(res)
-                        return res
-            return res
-        else:
-            return {"time": start_time}
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
-
-
-async def process_info(pid):
-    def real_func(pid):
-        start_time = int(time.time())
-        process = psutil.Process(int(pid))
-        num_handles = None
-        num_threads = None
-        try:
-            num_handles = process.num_handles()
-        except:
-            log.error(traceback.print_exc())
-        try:
-            num_threads = process.num_threads()
-        except:
-            log.error(traceback.print_exc())
-        res = {"time": start_time}
-        if num_handles: res["num_handles"] = num_handles
-        if num_threads: res["num_threads"] = num_threads
-        print_json(res)
-        return res
-
-    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
-
-
-async def perf(pid, save_dir):
-    monitors = {
-        "cpu": Monitor(cpu,
-                       pid=pid,
-                       key_value=["time", "cpu_usage(%)", "cpu_usage_all(%)", "cpu_core_num(个)"],
-                       save_dir=save_dir),
-        "memory": Monitor(memory,
-                          pid=pid,
-                          key_value=["time", "process_memory_usage(M)"],
-                          save_dir=save_dir),
-        "process_info": Monitor(process_info,
-                                pid=pid,
-                                key_value=["time", "num_threads(个)", "num_handles(个)"],
-                                save_dir=save_dir),
-        "fps": Monitor(fps,
-                       pid=pid,
-                       key_value=["time", "fps(帧)", "frames"],
-                       save_dir=save_dir),
-        "gpu": Monitor(gpu,
-                       pid=pid,
-                       key_value=["time", "gpu(%)"],
-                       save_dir=save_dir),
-        "screenshot": Monitor(screenshot,
-                              pid=pid,
-                              save_dir=save_dir, is_out=False)
-    }
-    run_monitors = [monitor.run() for name, monitor in monitors.items()]
-    await asyncio.gather(*run_monitors)
+import asyncio
+import json
+import platform
+import subprocess
+import threading
+import time
+import traceback
+from io import BytesIO
+import psutil
+import pynvml
+from pathlib import Path
+from log import log
+from core.monitor import Monitor
+
+SUPPORT_GPU = True
+try:
+    pynvml.nvmlInit()
+except:
+    traceback.print_exc()
+    log.info("本设备gpu获取不适配")
+    SUPPORT_GPU = False
+from PIL import ImageGrab
+
+
+def print_json(msg):
+    log.info(json.dumps(msg))
+
+
+class WinFps(object):
+    frame_que = list()
+    single_instance = None
+    fps_process = None
+
+    def __init__(self, pid):
+        self.pid = pid
+
+    def __new__(cls, *args, **kwargs):
+        if not cls.single_instance:
+            cls.single_instance = super().__new__(cls)
+        return cls.single_instance
+
+    def fps(self):
+        if not WinFps.fps_process:
+            threading.Thread(target=self.start_fps_collect, args=(self.pid,)).start()
+        if self.check_queue_head_frames_complete():
+            return self.pop_complete_fps()
+
+    @staticmethod
+    def check_queue_head_frames_complete():
+        if not WinFps.frame_que:
+            return False
+        head_time = int(WinFps.frame_que[0])
+        end_time = int(WinFps.frame_que[-1])
+        if head_time == end_time:
+            return False
+        return True
+
+    @staticmethod
+    def pop_complete_fps():
+        head_time = int(WinFps.frame_que[0])
+        complete_fps = []
+        while int(WinFps.frame_que[0]) == head_time:
+            complete_fps.append(WinFps.frame_que.pop(0))
+        return complete_fps
+
+    def start_fps_collect(self, pid):
+        start_fps_collect_time = int(time.time())
+        PresentMon = Path(__file__).parent.parent.joinpath("PresentMon.exe")
+        res_terminate = subprocess.Popen(
+            [PresentMon, "-process_id", str(pid), "-output_stdout", "-stop_existing_session"],
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        WinFps.fps_process = res_terminate
+        res_terminate.stdout.readline()
+        while not res_terminate.poll():
+            line = res_terminate.stdout.readline()
+            if not line:
+                try:
+                    res_terminate.kill()
+                except:
+                    traceback.print_exc()
+                break
+            try:
+                line = line.decode(encoding="utf-8")
+                line_list = line.split(",")
+                print("line ", line_list)
+                WinFps.frame_que.append(start_fps_collect_time + round(float(line_list[7]), 7))
+            except:
+                time.sleep(1)
+                log.error(traceback.format_exc())
+
+
+async def sys_info():
+    def real_func():
+        current_platform = platform.system()
+        computer_name = platform.node()
+        res = {"platform": current_platform, "computer_name": computer_name, "time": time.time(),
+               "cpu_cores": psutil.cpu_count(), "ram": "{0}G".format(int(psutil.virtual_memory().total / 1024 ** 3)),
+               "rom": "{0}G".format(int(psutil.disk_usage('/').total / 1024 ** 3))}
+        print_json(res)
+        return res
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func), timeout=10)
+
+
+async def pids():
+    def real_func():
+        process_list = []
+        for proc in psutil.process_iter(attrs=['name', 'pid', 'cmdline', 'username']):
+            try:
+                if proc.is_running():
+                    process_list.append(
+                        {"name": proc.info['name'], "pid": proc.info['pid'], "cmd": proc.info['cmdline'],
+                         "username": proc.username()})
+            except Exception as e:
+                log.error(e)
+        process_list.sort(key=lambda x: x['name'])
+        # print_json(process_list)
+        return process_list
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func), timeout=10)
+
+
+async def screenshot(pid, save_dir):
+    def real_func(pid, save_dir):
+        start_time = int(time.time())
+        if pid:
+            window = None
+            if platform.system() == "Windows":
+                import ctypes
+                import pygetwindow as gw
+                def get_pid(hwnd):
+                    pid = ctypes.wintypes.DWORD()
+                    ctypes.windll.user32.GetWindowThreadProcessId(hwnd, ctypes.byref(pid))
+                    return pid.value
+
+                def get_window_by_pid(pid):
+                    for window in gw.getAllWindows():
+                        if get_pid(window._hWnd) == pid:
+                            return window
+                    return None
+
+                window = get_window_by_pid(int(pid))
+            if window:
+                screenshot = ImageGrab.grab(
+                    bbox=(window.left, window.top, window.left + window.width, window.top + window.height),
+                    all_screens=True)
+            else:
+                screenshot = ImageGrab.grab(all_screens=True)
+            if save_dir:
+                dir_instance = Path(save_dir)
+                screenshot_dir = dir_instance.joinpath("screenshot")
+                screenshot_dir.mkdir(exist_ok=True)
+                screenshot.save(screenshot_dir.joinpath(str(start_time) + ".png"), format="PNG")
+            else:
+                output_buffer = BytesIO()
+                screenshot.save(output_buffer, format='PNG')
+                output_buffer.seek(0)  # 重置缓冲区指针
+                image_data = output_buffer.getvalue()
+                return image_data
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func, pid, save_dir), timeout=10)
+
+
+async def cpu(pid):
+    def real_func(pid):
+        start_time = int(time.time())
+        proc = psutil.Process(pid=int(pid))
+        cpu_usage = proc.cpu_percent(interval=1)
+        cpu_count = psutil.cpu_count()
+        res = {"cpu_usage": cpu_usage / cpu_count, "cpu_usage_all": cpu_usage,
+               "cpu_core_num": cpu_count, "time": start_time}
+        print_json(res)
+        return res
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
+
+
+async def memory(pid):
+    def real_func(pid):
+        start_time = int(time.time())
+        process = psutil.Process(int(pid))
+        process_memory_info = process.memory_info()
+        process_memory_usage = process_memory_info.rss / (1024 ** 2)  # In MB
+        memory_info = {"process_memory_usage": process_memory_usage, "time": start_time}
+        print_json(memory_info)
+        return memory_info
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
+
+
+async def fps(pid):
+    if platform.system() != "Windows":
+        return {"type": "fps", "time": int(time.time())}
+    frames = WinFps(pid).fps()
+    if not frames:
+        return frames
+    res = {"type": "fps", "fps": len(frames), "frames": frames, "time": int(frames[0]) if frames else int(time.time())}
+    print_json(res)
+    return res
+
+
+async def gpu(pid):
+    def real_func(pid):
+        pid = int(pid)
+        start_time = int(time.time())
+        if SUPPORT_GPU:
+            device_count = pynvml.nvmlDeviceGetCount()
+            res = None
+            for i in range(device_count):
+                handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+                processes = pynvml.nvmlDeviceGetComputeRunningProcesses(handle)
+                for process in processes:
+                    print(process)
+                    if process.pid == pid:
+                        gpu_Utilization = pynvml.nvmlDeviceGetUtilizationRates(handle)
+                        gpu_utilization_percentage = gpu_Utilization.gpu  # GPU的计算使用率
+                        res = {"gpu": gpu_utilization_percentage, "time": start_time}
+                        print_json(res)
+                        return res
+            return res
+        else:
+            return {"time": start_time}
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
+
+
+async def process_info(pid):
+    def real_func(pid):
+        start_time = int(time.time())
+        process = psutil.Process(int(pid))
+        num_handles = None
+        num_threads = None
+        try:
+            num_handles = process.num_handles()
+        except:
+            log.error(traceback.format_exc())
+        try:
+            num_threads = process.num_threads()
+        except:
+            log.error(traceback.format_exc())
+        res = {"time": start_time}
+        if num_handles: res["num_handles"] = num_handles
+        if num_threads: res["num_threads"] = num_threads
+        print_json(res)
+        return res
+
+    return await asyncio.wait_for(asyncio.to_thread(real_func, pid), timeout=10)
+
+
+async def perf(pid, save_dir):
+    monitors = {
+        "cpu": Monitor(cpu,
+                       pid=pid,
+                       key_value=["time", "cpu_usage(%)", "cpu_usage_all(%)", "cpu_core_num(个)"],
+                       save_dir=save_dir),
+        "memory": Monitor(memory,
+                          pid=pid,
+                          key_value=["time", "process_memory_usage(M)"],
+                          save_dir=save_dir),
+        "process_info": Monitor(process_info,
+                                pid=pid,
+                                key_value=["time", "num_threads(个)", "num_handles(个)"],
+                                save_dir=save_dir),
+        "fps": Monitor(fps,
+                       pid=pid,
+                       key_value=["time", "fps(帧)", "frames"],
+                       save_dir=save_dir),
+        "gpu": Monitor(gpu,
+                       pid=pid,
+                       key_value=["time", "gpu(%)"],
+                       save_dir=save_dir),
+        "screenshot": Monitor(screenshot,
+                              pid=pid,
+                              save_dir=save_dir, is_out=False)
+    }
+    run_monitors = [monitor.run() for name, monitor in monitors.items()]
+    await asyncio.gather(*run_monitors)
```

### Comparing `pc-perf-1.1.6/dao.py` & `pc-perf-1.2.1/dao.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,159 +1,167 @@
-import asyncio
-import datetime
-import os
-import platform
-from sqlalchemy import Column, String, Integer, DateTime, select, or_
-from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
-from sqlalchemy.orm import sessionmaker
-from contextlib import asynccontextmanager
-from sqlalchemy_serializer import SerializerMixin
-from sqlalchemy.orm import declarative_base
-from log import log as logger
-
-logger.info("工作空间{0}".format(os.getcwd()))
-db_path = os.path.join(os.getcwd(), "task.sqlite")
-logger.info("db path {0}".format(db_path))
-async_engine = create_async_engine('sqlite+aiosqlite:///{0}'.format(db_path), echo=False)
-logger.info("current path {0}".format(os.getcwd()))
-AsyncSessionLocal = sessionmaker(bind=async_engine, class_=AsyncSession, expire_on_commit=False)
-Base = declarative_base()
-
-
-@asynccontextmanager
-async def async_connect():
-    session = AsyncSessionLocal()
-    try:
-        logger.info("sql begin")
-        yield session
-        await session.commit()
-        logger.info("sql success")
-    except Exception as e:
-        await session.rollback()
-        raise e
-    finally:
-        logger.info("sql end")
-        await session.close()
-
-
-async def update_table_structure():
-    async with async_engine.begin() as conn:
-        # 反射现有的数据库结构
-        await conn.run_sync(Base.metadata.create_all)
-
-
-class Task(Base, SerializerMixin):
-    __tablename__ = 'tasks'
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    start_time = Column(DateTime, default=None)
-    end_time = Column(DateTime, default=None)
-    serialno = Column(String(255), default=None)
-    status = Column(Integer)  # 0未开始, 1 执行中 , 2 执行完成 3.暂停
-    file_dir = Column(String(255), default=None)  # 存储csv文件的路径
-    target_pid = Column(Integer)  # 被测进程pid
-    target_pid_name = Column(String(255), default=None)  # 被测进程pid 名称
-    monitor_pid = Column(Integer, default=None)  # 当前任务运行的进程pid，任务执行的进程，里面有各个性能指标的线程
-    platform = Column(String(50), default="win")  # win | mac | linux 任务
-    name = Column(String(255), default=None)  # 任务名称
-
-
-class TaskLabel(Base, SerializerMixin):
-    __tablename__ = 'task_label'
-    id = Column(Integer, primary_key=True, autoincrement=True)
-    start_time = Column(DateTime, default=None)  # 标签开始
-    end_time = Column(DateTime, default=None)  # 标签结束
-    label_name = Column(String(255), default=None)  # 标签名称
-
-
-class TaskCollection(object):
-
-    @classmethod
-    async def set_task_running(cls, task_id, monitor_pid):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task).filter(Task.id == task_id))
-                task = result.scalars().first()
-                assert task, "NOT FIND TASK"
-                assert task.status == 0, "TASK RUNNING FAIL, TASK STATUS IS {0}".format(task.status)
-                task.status = 1
-                task.monitor_pid = monitor_pid
-                return task.to_dict()
-
-    @classmethod
-    async def get_all_task(cls):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task))
-                task = result.scalars().fetchall()
-                result_list = [t.to_dict() for t in task]
-                result_list.sort(key=lambda x: x.get("start_time"), reverse=True)
-                return result_list
-
-    @classmethod
-    async def get_item_task(cls, task_id):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task).filter(Task.id == task_id))
-                task = result.scalars().first()
-                assert task, "NOT FIND TASK"
-                return task.to_dict()
-
-    @classmethod
-    async def create_task(cls, pid, pid_name, file_dir, name):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(
-                    select(Task).filter(Task.target_pid == pid).filter(or_(
-                        Task.status == 0,
-                        Task.status == 1,
-                    )))
-                task = result.scalars().first()
-                assert not task, "MONITOR PID {0} TASK {1} IS RUN".format(pid, task.name)
-                new_task = Task(start_time=datetime.datetime.now(), serialno=platform.node(), status=0,
-                                target_pid=pid, platform=platform.system(), name=name, target_pid_name=pid_name)
-                session.add(new_task)
-                await session.flush()
-                file_dir = os.path.join(file_dir, str(new_task.id))
-                new_task.file_dir = file_dir
-                await session.flush()
-                return new_task.id, file_dir
-
-    @classmethod
-    async def stop_task(cls, task_id):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task).filter(Task.id == task_id))
-                task = result.scalars().first()
-                assert task, "NOT FIND TASK"
-                assert task.status != 0, "TASK NOT RUNNING, TASK STATUS IS {0}".format(task.status)
-                task.status = 2
-                task.end_time = datetime.datetime.now()
-                return task.to_dict()
-
-    @classmethod
-    async def delete_task(cls, task_id):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task).filter(Task.id == task_id))
-                task = result.scalars().first()
-                assert task, "NOT FIND TASK"
-                assert task.status != 1, "TASK RUNNING NOT DELETE, TASK STATUS IS {0}".format(task.status)
-                res = task.to_dict()
-                await session.delete(task)
-                return res
-
-    @classmethod
-    async def change_task_name(cls, task_id, new_name):
-        async with async_connect() as session:
-            async with session.begin():
-                result = await session.execute(select(Task).filter(Task.id == task_id))
-                task = result.scalars().first()
-                assert task, "NOT FIND TASK"
-                task.name = new_name
-                return task.to_dict()
-
-
-async def create_table():
-    await update_table_structure()
-
-
-asyncio.run(create_table())
+import asyncio
+import datetime
+import os
+import platform
+from sqlalchemy import Column, String, Integer, DateTime, select, or_
+from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
+from sqlalchemy.orm import sessionmaker
+from contextlib import asynccontextmanager
+from sqlalchemy_serializer import SerializerMixin
+from sqlalchemy.orm import declarative_base
+from log import log as logger
+
+logger.info("工作空间{0}".format(os.getcwd()))
+db_path = os.path.join(os.getcwd(), "task.sqlite")
+logger.info("db path {0}".format(db_path))
+async_engine = create_async_engine('sqlite+aiosqlite:///{0}'.format(db_path), echo=False)
+logger.info("current path {0}".format(os.getcwd()))
+AsyncSessionLocal = sessionmaker(bind=async_engine, class_=AsyncSession, expire_on_commit=False)
+Base = declarative_base()
+
+
+@asynccontextmanager
+async def async_connect():
+    session = AsyncSessionLocal()
+    try:
+        logger.info("sql begin")
+        yield session
+        await session.commit()
+        logger.info("sql success")
+    except Exception as e:
+        await session.rollback()
+        raise e
+    finally:
+        logger.info("sql end")
+        await session.close()
+
+
+async def update_table_structure():
+    async with async_engine.begin() as conn:
+        # 反射现有的数据库结构
+        await conn.run_sync(Base.metadata.create_all)
+
+
+class Task(Base, SerializerMixin):
+    __tablename__ = 'tasks'
+    id = Column(Integer, primary_key=True, autoincrement=True)
+    start_time = Column(DateTime, default=None)
+    end_time = Column(DateTime, default=None)
+    serialno = Column(String(255), default=None)
+    status = Column(Integer)  # 0未开始, 1 执行中 , 2 执行完成 3.暂停
+    file_dir = Column(String(255), default=None)  # 存储csv文件的路径
+    target_pid = Column(Integer)  # 被测进程pid
+    target_pid_name = Column(String(255), default=None)  # 被测进程pid 名称
+    monitor_pid = Column(Integer, default=None)  # 当前任务运行的进程pid，任务执行的进程，里面有各个性能指标的线程
+    platform = Column(String(50), default="win")  # win | mac | linux 任务
+    name = Column(String(255), default=None)  # 任务名称
+
+
+class TaskLabel(Base, SerializerMixin):
+    __tablename__ = 'task_label'
+    id = Column(Integer, primary_key=True, autoincrement=True)
+    start_time = Column(DateTime, default=None)  # 标签开始
+    end_time = Column(DateTime, default=None)  # 标签结束
+    label_name = Column(String(255), default=None)  # 标签名称
+
+
+class TaskCollection(object):
+
+    @classmethod
+    async def set_task_running(cls, task_id, monitor_pid):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.id == task_id))
+                task = result.scalars().first()
+                assert task, "NOT FIND TASK"
+                assert task.status == 0, "TASK RUNNING FAIL, TASK STATUS IS {0}".format(task.status)
+                task.status = 1
+                task.monitor_pid = monitor_pid
+                return task.to_dict()
+
+    @classmethod
+    async def get_all_task(cls):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task))
+                task = result.scalars().fetchall()
+                result_list = [t.to_dict() for t in task]
+                result_list.sort(key=lambda x: x.get("start_time"), reverse=True)
+                return result_list
+
+    @classmethod
+    async def get_item_task(cls, task_id):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.id == task_id))
+                task = result.scalars().first()
+                assert task, "NOT FIND TASK"
+                return task.to_dict()
+
+    @classmethod
+    async def get_all_stop_task_monitor_pid(cls):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.status == 2))
+                tasks = result.scalars().fetchall()
+                return [task.monitor_pid for task in tasks]
+
+    @classmethod
+    async def create_task(cls, pid, pid_name, file_dir, name):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(
+                    select(Task).filter(Task.target_pid == pid).filter(or_(
+                        Task.status == 0,
+                        Task.status == 1,
+                    )))
+                task = result.scalars().first()
+                assert not task, "MONITOR PID {0} TASK {1} IS RUN".format(pid, task.name)
+                new_task = Task(start_time=datetime.datetime.now(), serialno=platform.node(), status=0,
+                                target_pid=pid, platform=platform.system(), name=name, target_pid_name=pid_name)
+                session.add(new_task)
+                await session.flush()
+                file_dir = os.path.join(file_dir, str(new_task.id))
+                new_task.file_dir = file_dir
+                await session.flush()
+                return new_task.id, file_dir
+
+    @classmethod
+    async def stop_task(cls, task_id):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.id == task_id))
+                task = result.scalars().first()
+                assert task, "NOT FIND TASK"
+                assert task.status != 0, "TASK NOT RUNNING, TASK STATUS IS {0}".format(task.status)
+                task.status = 2
+                task.end_time = datetime.datetime.now()
+                return task.to_dict()
+
+    @classmethod
+    async def delete_task(cls, task_id):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.id == task_id))
+                task = result.scalars().first()
+                assert task, "NOT FIND TASK"
+                assert task.status != 1, "TASK RUNNING NOT DELETE, TASK STATUS IS {0}".format(task.status)
+                res = task.to_dict()
+                await session.delete(task)
+                return res
+
+    @classmethod
+    async def change_task_name(cls, task_id, new_name):
+        async with async_connect() as session:
+            async with session.begin():
+                result = await session.execute(select(Task).filter(Task.id == task_id))
+                task = result.scalars().first()
+                assert task, "NOT FIND TASK"
+                task.name = new_name
+                return task.to_dict()
+
+
+async def create_table():
+    await update_table_structure()
+
+
+asyncio.run(create_table())
```

### Comparing `pc-perf-1.1.6/log.py` & `pc-perf-1.2.1/log.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from logging import getLogger, INFO, StreamHandler, Formatter
-from concurrent_log_handler import ConcurrentRotatingFileHandler
-import os
-
-log = getLogger(__name__)
-# Use an absolute path to prevent file rotation trouble.
-logfile = os.path.abspath("log.log")
-# Rotate log after reaching 512K, keep 5 old copies.
-rotateHandler = ConcurrentRotatingFileHandler(logfile, "a", 512 * 1024 * 1024, 1)
-log.addHandler(rotateHandler)
-log.setLevel(INFO)
-streamHandler = StreamHandler()
-streamHandler.setLevel(INFO)
-streamHandler.setFormatter(Formatter(
-    '%(asctime)s - %(name)s - %(levelname)s - %(message)s'  # 日志格式
-))
+from logging import getLogger, INFO, StreamHandler, Formatter
+from concurrent_log_handler import ConcurrentRotatingFileHandler
+import os
+
+log = getLogger(__name__)
+# Use an absolute path to prevent file rotation trouble.
+logfile = os.path.abspath("log.log")
+# Rotate log after reaching 512K, keep 5 old copies.
+rotateHandler = ConcurrentRotatingFileHandler(logfile, "a", 512 * 1024 * 1024, 1)
+log.addHandler(rotateHandler)
+log.setLevel(INFO)
+streamHandler = StreamHandler()
+streamHandler.setLevel(INFO)
+streamHandler.setFormatter(Formatter(
+    '%(asctime)s - %(name)s - %(levelname)s - %(message)s'  # 日志格式
+))
 log.addHandler(streamHandler)
```

### Comparing `pc-perf-1.1.6/setup.py` & `pc-perf-1.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,82 @@
-# coding=utf-8
-from setuptools import setup, find_packages
-
-setup(
-    # 包的名称，通常与包的目录名称相同
-    name='pc-perf',
-
-    # 版本号，遵循语义化版本控制规则
-    version='1.1.6',
-
-    # 项目简短描述
-    description='pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示',
-
-    # 项目的URL，通常是项目主页或源代码仓库
-    url='https://github.com/15525730080/pc_perf',
-
-    # 作者
-    author='范博洲',
-
-    # 作者的电子邮件地址
-    author_email='15525730080@163.com',
-
-    # 包的许可证
-    license='MIT',
-
-    # 包的关键词
-    keywords='pc fps cpu memory gpu monitor',
-
-    # 定义项目所需的依赖
-    install_requires=[
-        "concurrent_log_handler==0.9.25",
-        "fastapi==0.110.2",
-        "numpy==1.23.5",
-        "pandas==2.2.2",
-        "Pillow==10.3.0",
-        "psutil==5.9.8",
-        "PyGetWindow==0.0.9",
-        "pynvml==11.5.0",
-        "SQLAlchemy==2.0.29",
-        "SQLAlchemy_serializer==1.4.12",
-        "starlette==0.37.2",
-        "uvicorn==0.29.0",
-        "aiosqlite==0.20.0"
-    ],
-
-    # 从包中自动寻找所有的子包和子模块
-    py_modules=['dao', 'log', 'task_handle', 'util', 'pc_perf', 'core'],
-    packages=['core'],
-    
-    # 包含数据文件，比如配置文件
-    include_package_data=True,
-
-    # 定义包中非.py文件的内容
-    package_data={
-        # 如果你的包中有数据文件，可以在这里指定
-        '': ['../*.exe', '../test_result/*.html'],
-    },
-
-    # 指定Python版本要求
-    python_requires='>=3.9',
-
-    # # 指定包的入口点，用于命令行工具
-    entry_points={
-        'console_scripts': [
-            'pc_perf=pc_perf:main',  # 这里的web-command是你为命令行工具定义的命令
-        ],
-    },
-
-    # 指定分发文件的类别，例如："Programming Language :: Python :: 3"
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.12',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries',
-    ],
-)
+# coding=utf-8
+from setuptools import setup, find_packages
+
+setup(
+    # 包的名称，通常与包的目录名称相同
+    name='pc-perf',
+
+    # 版本号，遵循语义化版本控制规则
+    version='1.2.1',
+
+    # 项目简短描述
+    description='pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示',
+
+    # 项目的URL，通常是项目主页或源代码仓库
+    url='https://github.com/15525730080/pc_perf',
+
+    # 作者
+    author='范博洲',
+
+    # 作者的电子邮件地址
+    author_email='15525730080@163.com',
+
+    # 包的许可证
+    license='MIT',
+
+    # 包的关键词
+    keywords='pc fps cpu memory gpu monitor',
+
+    # 定义项目所需的依赖
+    install_requires=[
+        "concurrent_log_handler==0.9.25",
+        "fastapi==0.110.2",
+        "numpy==1.23.5",
+        "pandas==2.2.2",
+        "Pillow==10.3.0",
+        "psutil==5.9.8",
+        "PyGetWindow==0.0.9",
+        "pynvml==11.5.0",
+        "SQLAlchemy==2.0.29",
+        "SQLAlchemy_serializer==1.4.12",
+        "starlette==0.37.2",
+        "uvicorn==0.29.0",
+        "aiosqlite==0.20.0",
+        "APScheduler==3.10.4"
+    ],
+
+    # 从包中自动寻找所有的子包和子模块
+    py_modules=['dao', 'log', 'task_handle', 'util', 'pc_perf', 'core'],
+    packages=['core'],
+    
+    # 包含数据文件，比如配置文件
+    include_package_data=True,
+
+    # 定义包中非.py文件的内容
+    package_data={
+        # 如果你的包中有数据文件，可以在这里指定
+        '': ['../*.exe', '../test_result/*.html'],
+    },
+
+    # 指定Python版本要求
+    python_requires='>=3.9',
+
+    # # 指定包的入口点，用于命令行工具
+    entry_points={
+        'console_scripts': [
+            'pc_perf=pc_perf:main',  # 这里的web-command是你为命令行工具定义的命令
+        ],
+    },
+
+    # 指定分发文件的类别，例如："Programming Language :: Python :: 3"
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries',
+    ],
+)
```

### Comparing `pc-perf-1.1.6/task_handle.py` & `pc-perf-1.2.1/task_handle.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-# coding=utf-8
-import asyncio
-import os
-from builtins import *
-from multiprocessing.context import Process
-
-import psutil
-
-from dao import TaskCollection
-from log import log as logger
-from core.pc_tools import perf as pc_perf
-
-
-class TaskHandle(Process):
-
-    def __init__(self, serialno: str, target_pid: int, file_dir: str, task_id: int, platform: str):
-        super(TaskHandle, self).__init__()
-        self.serialno = serialno
-        self.target_pid = target_pid
-        self.file_dir = file_dir
-        if not os.path.exists(self.file_dir):
-            os.makedirs(self.file_dir)
-        self.daemon = True
-        self.task_id = task_id
-        self.platform = platform  # platform.system()
-
-    def start(self):
-        logger.info("join task handle")
-        super().start()
-
-    def run(self):
-        logger.info("join task handle run")
-        asyncio.run(TaskCollection.set_task_running(self.task_id, self.pid))
-        asyncio.run(pc_perf(self.target_pid, self.file_dir))
-
-    @staticmethod
-    def stop_handle(monitor_pid):
-        logger.info("Stopping task handle and subprocesses...")
-        # Terminate the pc_perf subprocess
-        current_process = psutil.Process(monitor_pid)
-        try:
-            for child in current_process.children(recursive=True):
-                child.terminate()
-        except Exception as e:
-            logger.error(e)
-        finally:
-            current_process.terminate()
-
-
-if __name__ == '__main__':
-    TaskHandle.stop_handle(15160)
+# coding=utf-8
+import asyncio
+import os
+import traceback
+from builtins import *
+from multiprocessing.context import Process
+
+import psutil
+
+from dao import TaskCollection
+from log import log as logger
+from core.pc_tools import perf as pc_perf
+
+
+class TaskHandle(Process):
+
+    def __init__(self, serialno: str, target_pid: int, file_dir: str, task_id: int, platform: str):
+        super(TaskHandle, self).__init__()
+        self.serialno = serialno
+        self.target_pid = target_pid
+        self.file_dir = file_dir
+        if not os.path.exists(self.file_dir):
+            os.makedirs(self.file_dir)
+        self.daemon = True
+        self.task_id = task_id
+        self.platform = platform  # platform.system()
+
+    def start(self):
+        logger.info("join task handle")
+        super().start()
+
+    def run(self):
+        logger.info("join task handle run")
+        asyncio.run(TaskCollection.set_task_running(self.task_id, self.pid))
+        asyncio.run(pc_perf(self.target_pid, self.file_dir))
+
+    @staticmethod
+    def stop_handle(monitor_pid):
+        logger.info("Stopping task handle and subprocesses... {0}".format(monitor_pid))
+        # kill the pc_perf subprocess
+        current_process = psutil.Process(monitor_pid)
+        try:
+            for child in current_process.children(recursive=True):
+                child.kill()
+                child.wait(0.2)
+        except Exception as e:
+            logger.error(e)
+        finally:
+            try:
+                current_process.kill()
+                current_process.wait(1)
+            except:
+                logger.error(traceback.format_exc())
+
+
```

### Comparing `pc-perf-1.1.6/test_result/index.html` & `pc-perf-1.2.1/test_result/index.html`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,723 +1,723 @@
-<!DOCTYPE html>
-<html>
-<head>
-    <meta charset="UTF-8">
-    <title>性能测试报告</title>
-    <!-- 引入 Element UI CSS -->
-    <link href="https://unpkg.com/element-ui/lib/theme-chalk/index.css" rel="stylesheet">
-    <!-- 引入 Swiper CSS -->
-    <link href="https://unpkg.com/swiper@latest/swiper-bundle.min.css" rel="stylesheet">
-    <!-- 引入 Vue -->
-    <script src="https://cdn.bootcdn.net/ajax/libs/vue/2.6.14/vue.min.js"></script>
-    <!-- 引入 Element UI -->
-    <script src="https://unpkg.com/element-ui/lib/index.js"></script>
-    <!-- 引入 Axios -->
-    <script src="https://cdn.bootcdn.net/ajax/libs/axios/0.21.1/axios.min.js"></script>
-    <!-- 引入 ECharts -->
-    <script src="https://unpkg.com/echarts/dist/echarts.min.js"></script>
-    <!-- 引入 Swiper -->
-    <script src="https://unpkg.com/swiper@latest/swiper-bundle.min.js"></script>
-    <style>
-        /* 自定义样式 */
-        .el-aside {
-            background-color: #f2f2f2;
-        }
-        .task-button {
-            margin-bottom: 10px;
-        }
-		.headernavbar{
-			background-color: #3b4d6e;
-            color: #fff;
-            margin: 0;
-            padding: 0;
-            display: flex;
-            justify-content: space-between;
-            align-items: center;
-            height: 100%;
-		}
-		.headernavbar h1 {
-            margin: 0;
-            font-size: 18px;
-            color: #fff;
-        }
-        html, body {
-        margin: 0;
-        padding: 0;
-        height: 100%; /* 使 body 占满整个视口高度 */
-        }
-        .el-header{
-            margin:0;
-            padding:0;
-        }
-		.el-aside {
-            background-color: #fff;
-            box-shadow: 2px 0 8px rgba(0, 0, 0, .1);
-            flex: 0 0 200px;
-        }
-
-        .box-card {
-          border: none;
-          box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
-          border-radius: 8px;
-          overflow: hidden;
-        }
-
-        .box-card:hover {
-          box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
-          transition: box-shadow 0.3s ease-in-out;
-        }
-
-        .el-card__header {
-          background-color: #409eff;
-          color: white;
-          padding: 10px 20px;
-          font-size: 18px;
-          font-weight: bold;
-          border-radius: 8px 8px 0 0;
-        }
-
-        .el-card__body {
-          padding: 20px;
-        }
-
-        p {
-          margin: 0;
-          color: #333;
-          line-height: 1.6;
-        }
-
-        p span {
-          color: #409eff;
-          font-weight: bold;
-        }
-
-        @media (max-width: 600px) {
-          .box-card {
-            width: calc(100% - 20px);
-          }
-        }
-        .taskform {
-          margin: 50px auto;
-          padding: 20px;
-          background-color: #fff;
-          border-radius: 8px;
-          box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
-        }
-
-
-
-
-        /* 图表容器的基本样式 */
-.chart-container {
-  width: 50%; /* 占满容器宽度 */
-  max-width: 100%; /* 防止宽度超过容器 */
-  height: 400px; /* 默认高度 */
-  margin-bottom: 20px; /* 图表之间的间距 */
-  background-color: #ffffff; /* 背景颜色 */
-  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* 轻微的阴影效果 */
-  border-radius: 4px; /* 轻微的圆角 */
-  overflow: hidden; /* 隐藏溢出的内容 */
-}
-
-/* 图表标题样式 */
-.chart-title {
-  font-size: 1.1em;
-  font-weight: bold;
-  margin: 0 0 10px; /* 上下边距为0，下边距为10px */
-  padding: 10px;
-  background-color: #f2f2f2; /* 标题背景颜色 */
-  border-radius: 4px 4px 0 0; /* 仅上边缘圆角 */
-}
-
-/* 图表容器内的 ECharts 图表样式 */
-.echarts-chart {
-  width: 100%; /* 占满容器宽度 */
-  height: calc(100% - 30px); /* 减去标题的高度 */
-}
-
-
-    </style>
-</head>
-<body>
-<div id="app" style="margin:0;padding:0; height: 100%;">
-    <el-header style="height: 8%;">
-        <div class="headernavbar">
-            <svg class="icon" style="height: 3em;vertical-align: middle;fill: currentColor;overflow: hidden;"
-                 viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2539">
-                <path d="M467.104627 672.205804L110.431373 840.422902l348.300549 159.422745c24.636235 10.842353 43.670588 16.263529 57.123137 16.263529 13.452549 0 33.209725-5.421176 59.231372-16.263529L913.568627 840.44298l-356.673254-168.217098a105.251137 105.251137 0 0 0-89.790746 0z"
-                      fill="#797979" p-id="2540"></path>
-                <path d="M110.431373 791.752784v55.17553c202.912627 91.597804 319.006118 142.898196 348.300549 153.901176 43.951686 16.484392 58.287686 25.660235 129.244862-4.718431 47.304784-20.259137 155.828706-70.194196 325.591843-149.785098v-54.573177c-200.864627 93.043451-309.388549 142.817882-325.591843 149.303216-24.294902 9.758118-101.677176 18.713098-138.782117 0-24.736627-12.448627-137.657725-62.243137-338.763294-149.303216z"
-                      fill="#282F9A" p-id="2541"></path>
-                <path d="M467.104627 623.535686L110.431373 791.752784l348.300549 159.422745c24.636235 10.842353 43.670588 16.243451 57.123137 16.243451 13.452549 0 33.209725-5.421176 59.231372-16.243451L913.568627 791.752784l-356.673254-168.217098a105.251137 105.251137 0 0 0-89.790746 0z"
-                      fill="#727AFF" p-id="2542"></path>
-                <path d="M634.819765 43.369412l-195.604079 402.713098 160.326275 13.874196-110.933334 332.900392 269.050981-472.485647-132.116079-32.225882z"
-                      fill="#FFCB28" p-id="2543"></path>
-                <path d="M438.633412 458.189804l-101.355922 81.116863L595.425882 81.960157l39.393883-38.590745z"
-                      fill="#FF9D00" p-id="2544"></path>
-                <path d="M338.723137 538.001569h157.776314l112.097882-78.72753-163.84-12.609255z" fill="#CD7E00"
-                      p-id="2545"></path>
-                <path d="M496.499451 538.001569L455.981176 811.971765l32.727844-18.873726 117.559215-333.342117z"
-                      fill="#FF9D00" p-id="2546"></path>
-            </svg>
-            <h1>PC进程性能测试平台
-            </h1>
-        </div>
-    </el-header>
-    <el-container style="height: 90%;">
-        <!-- 侧边栏 -->
-        <el-aside style="width: 150px;">
-            <el-menu :default-active="1" class="el-menu-demo" style="border-right: solid 0px">
-                <el-menu-item index="1" class="task-button" @click="switchView('taskList');">
-                    <h3>任务列表</h3>
-                </el-menu-item>
-                <el-menu-item index="2" class="task-button" @click="switchView('createTask')">
-                    <h3>创建任务</h3>
-                </el-menu-item>
-            </el-menu>
-        </el-aside>
-        <!-- 内容区域 -->
-        <el-container>
-            <el-main>
-                <template v-if="currentView === 'taskList'">
-                    <el-table :data="tasks" style="width: 100%" height="100%">
-                        <el-table-column prop="name" label="任务名称" sortable></el-table-column>
-                        <el-table-column prop="serialno" label="被测设备" sortable></el-table-column>
-                        <el-table-column prop="target_pid" label="被测进程" sortable></el-table-column>
-                        <el-table-column prop="target_pid_name" label="进程名称" sortable></el-table-column>
-                        <el-table-column prop="status" label="任务状态" sortable>
-                            <template slot-scope="scope">
-                                <el-button type="info" size="mini" v-if="scope.row.status==0">待执行</el-button>
-                                <el-button type="primary" size="mini" v-if="scope.row.status==1">执行中</el-button>
-                                <el-button type="danger" size="mini" v-if="scope.row.status==-1">执行失败</el-button>
-                                <el-button type="success" size="mini" v-if="scope.row.status==2">执行完成</el-button>
-                            </template>
-                        </el-table-column>
-                        <el-table-column prop="platform" label="设备平台" sortable></el-table-column>
-                        <el-table-column prop="start_time" label="开始时间" sortable></el-table-column>
-                        <el-table-column prop="end_time" label="结束时间" sortable></el-table-column>
-                        <el-table-column label="操作">
-                            <template slot-scope="scope">
-                                <el-button type="danger" size="mini" v-if="scope.row.status==1"
-                                           @click="stop_task(scope.row.id)">停止任务
-                                </el-button>
-                                <el-button type="danger" size="mini" v-if="scope.row.status!=1"
-                                           @click="delete_task(scope.row.id)">删除任务
-                                </el-button>
-                                <el-button type="primary" size="mini" v-if="scope.row.status!=0||scope.row.status!=-1"
-                                           @click="result(scope.row.id);curtaskid=scope.row.id;">查看结果
-                                </el-button>
-                            </template>
-                        </el-table-column>
-                    </el-table>
-                </template>
-                <template v-if="currentView === 'createTask'">
-                    <el-card class="box-card">
-                        <div slot="header" class="clearfix">
-                            <span>设备信息</span>
-                        </div>
-                        <div>
-                            <p>平台: <span>{{ currentSystemInfo.platform }}</span></p>
-                            <p>计算机名称: <span>{{ currentSystemInfo.computer_name }}</span></p>
-                            <p>CPU 核心数: <span>{{ currentSystemInfo.cpu_cores }}</span></p>
-                            <p>RAM: <span>{{ currentSystemInfo.ram }}</span></p>
-                            <p>ROM: <span>{{ currentSystemInfo.rom }}</span></p>
-                        </div>
-                    </el-card>
-                    <el-form ref="newTask" :model="newTask" label-width="5%" class="taskform">
-                        <el-form-item label="任务名称">
-                            <el-input v-model="newTask.name" placeholder="请输入任务名称" clearable></el-input>
-                        </el-form-item>
-                        <el-form-item label="选择 PID">
-                            <el-select v-model="newTask.pid" filterable placeholder="请选择 PID"
-                                       @visible-change="get_pids"
-                                       @change="getPidCmd">
-                                <el-option
-                                        v-for="pid in pids"
-                                        :key="pid.pid"
-                                        :label="pid.name + '_' + pid.pid"
-                                        :value="pid.pid">
-                                </el-option>
-                            </el-select>
-                        </el-form-item>
-                        <el-form-item v-if="cmd" label="pid cmd">
-                            {{cmd}}
-                        </el-form-item>
-                        <el-form-item v-if="cmd" label="pid 截图">
-                            <el-image
-                                    style="width: 100%; height: 100%"
-                                    :src=pid_img
-                            >
-                                <div slot="error" class="image-slot">
-                                </div>
-                            </el-image>
-                        </el-form-item>
-                        <el-form-item>
-                            <el-button type="primary" @click="createTask">创建任务</el-button>
-                        </el-form-item>
-                    </el-form>
-                </template>
-            </el-main>
-        </el-container>
-    </el-container>
-    <el-dialog
-            :visible.sync="dialogVisible"
-            width="80%"
-            @open="handleDialogVisibleChange"
-            @closed="clearInterval(intervalId);"
-            @destroy-on-close="true"
-    >
-        <div style="display: flex;flex-direction: row;flex-wrap: wrap;">
-
-            <div class="chart-container">
-                <div class="chart-title">{{num2time(clicktime)}}进程截图</div>
-                <div class="demo-image">
-                    <el-image
-                            style="width: 100%; height: 100%"
-                            :src='"/static/" + this.opentaskid + "/screenshot/" + this.clicktime + ".png"'
-                    >
-                        <div slot="error" class="image-slot">
-                        </div>
-                    </el-image>
-
-                </div>
-            </div>
-
-
-            <div class="chart-container">
-                <div class="chart-title">
-                    CPU 使用率
-                </div>
-                <div id="cpuChart" class="echarts-chart"></div>
-
-            </div>
-            <div class="chart-container">
-                <div class="chart-title">内存使用量</div>
-                <div id="memoryChart" class="echarts-chart"></div>
-
-            </div>
-            <div class="chart-container">
-                <div class="chart-title">FPS</div>
-                <div id="fpsChart" class="echarts-chart"></div>
-
-            </div>
-            <div class="chart-container">
-                <div class="chart-title">GPU 使用率</div>
-                <div id="gpuChart" class="echarts-chart"></div>
-
-            </div>
-            <div class="chart-container">
-                <div class="chart-title">线程数与句柄数</div>
-                <div id="processInfoChart" class="echarts-chart"></div>
-
-            </div>
-
-        </div>
-    </el-dialog>
-</div>
-
-<script>
-    new Vue({
-        el: '#app',
-        data: function() {
-            return {
-                dialogVisible: false,
-                currentSystemInfo: null,
-                currentView: 'taskList', // 当前视图，默认为任务列表
-                newTask: { // 新任务对象
-                    name: this.getCurrentTimestamp(),
-                    pid: null
-                },
-                pids: [],
-                tasks: [ // 任务列表数据
-
-                ],
-                cmd: '',
-                pid_name: '',
-                pid_img: '',
-                resultOption: null,
-                cpuChart: null,
-                memoryChart: null,
-                fpsChart: null,
-                gpuChart: null,
-                processInfoChart: null,
-                clicktime: null,
-                opentaskid: null, 
-                curtaskid: null,
-                intervalId: null,
-                isloadres: false,
-            };
-        },
-        methods: {
-            switchView(view) {
-                this.currentView = view;
-                this.getAllTask().then()
-            },
-            getCurrentTimestamp() {
-              const date = new Date();
-              const year = date.getFullYear();
-              const month = (date.getMonth() + 1).toString().padStart(2, '0'); // 月份从0开始，所以加1
-              const day = date.getDate().toString().padStart(2, '0');
-              const hours = date.getHours().toString().padStart(2, '0');
-              const minutes = date.getMinutes().toString().padStart(2, '0');
-              const seconds = date.getSeconds().toString().padStart(2, '0');
-
-              return `${year}-${month}-${day} ${hours}:${minutes}:${seconds}`;
-            },
-            getPidCmd(){
-                for (let i = 0; i < this.pids.length; i++) {
-                  if (this.newTask.pid === this.pids[i].pid) {
-                      this.cmd = this.pids[i].cmd.join(" ");
-                      this.pid_name = this.pids[i].name
-                  }
-                }
-                this.getPidImg()
-
-            },
-            syncDataZoom(chartInstance, otherCharts) {
-                chartInstance.getZr().on('click', (params) => {
-                        const pointInPixel = [params.offsetX, params.offsetY];
-                        if (chartInstance.containPixel("grid", pointInPixel)) {
-                            // 转换像素坐标到数据坐标
-                            // 将像素坐标转换为 x 轴的数据索引
-                            let xIndex = chartInstance.convertFromPixel({seriesIndex: 0}, pointInPixel)[0];
-                            let xAxisData = chartInstance.getOption().xAxis[0].data;
-                            let xAxisValue = xAxisData[xIndex];
-                            this.clicktime = xAxisValue
-                            console.log(this.clicktime)
-                            chartInstance.dispatchAction({
-                                type: "brush",
-                                areas: [
-                                {
-                                    brushType: "lineX",
-                                    coordRange: [
-                                        xIndex,
-                                        xIndex,
-                                    ],
-                                    xAxisIndex: 0,
-                                    transformable: false,
-                                },
-                                ],
-                            });
-                            for(let index in otherCharts){
-                                otherCharts[index].dispatchAction({
-                                    type: "brush",
-                                    areas: [
-                                    {
-                                        brushType: "lineX",
-                                        coordRange: [
-                                            xIndex,
-                                            xIndex,
-                                        ],
-                                        xAxisIndex: 0,
-                                        transformable: false,
-                                    },
-                                    ],
-                                }); 
-                            }
-                        }
-                    
-                    });
-            },
-            async get_pids() {
-                const res = await axios({method: 'get',//提交方法
-                            url: '/get_pids/'
-                 })
-				 console.log(res)
-				 this.pids = res.data.msg
-            },
-            async get_system_info() {
-                const res = await axios({method: 'get',//提交方法
-                            url: '/system_info/'
-                 })
-				 console.log(res)
-
-				 this.currentSystemInfo = res.data.msg
-            },
-            async createTask() {
-                const res = await axios({method: 'get',//提交方法
-                            url: '/run_task/?pid='+this.newTask.pid+'&task_name='+this.newTask.name+'&pid_name='+this.pid_name//提交地址
-                 })
-                 this.print_res(res)
-				 console.log(res)
-            },
-            async getAllTask(){
-                 const res = await axios({method: 'get',//提交方法
-							url: '/get_all_task/'//提交地址
-				 })
-				 console.log(res)
-				 this.tasks = res.data.msg
-            },
-            async getPidImg(){
-                 const res = await axios({method: 'get',//提交方法
-							url: '/pid_img/?pid=' + this.newTask.pid//提交地址
-				 })
-				 console.log(res)
-				 this.pid_img = "data:image/png;base64," + res.data
-            },
-            async delete_task(taskId){
-                    const res = await axios({method: 'get',//提交方法
-                                    url: '/delete_task/?task_id=' + taskId//提交地址
-                         })
-                         this.print_res(res)
-				 console.log(res.data)
-				 await this.getAllTask()
-            },
-            async result(taskId, isnotopenvis){
-		const res = await axios({method: 'get',//提交方法
-							url: '/result/?task_id=' + taskId//提交地址
-				 })
-                this.opentaskid = taskId
-				let tempOption={
-				      legend: {
-                        show: true
-                      },
-				      tooltip: {
-                        trigger: 'axis',
-                        axisPointer: {
-                            type: 'cross',
-                            crossStyle: {
-                                color: '#999'
-                            }
-                        }
-                    },
-                    xAxis: {
-                        type: 'category',
-                        boundaryGap: false,
-                        data: [/* 时间戳数据 */],
-                        axisPointer: {
-                            type: 'shadow'
-                        },
-                        axisLabel: {
-                            formatter: timestamp => {
-                                // 将Unix时间戳转换为JavaScript的Date对象
-                                const date = new Date(timestamp * 1000);
-                                // 使用toLocaleString方法格式化时间戳
-                                return date.toLocaleTimeString();
-                                }
-                        }
-                    },
-                    yAxis: {
-                        type: 'value'
-                    },
-                    series: [
-
-                    ],
-                    toolbox: {
-                     show: false,
-                    },
-                    brush: {
-                        xAxisIndex: "all",
-                        brushLink: "all",
-                        brushStyle: {
-                            borderWidth: 3,
-                            color: 'rgba(255,36,36,0.2)',
-                            borderColor: '#ff2424'
-                        }
-                    },
-                    markArea:{},
-					clickable: true,
-					symbol: 'circle',
-                    lineStyle: {
-							width: 0.5,
-					},
-                    showSymbol: false,//是否默认展示圆点
-                    dataZoom: 
-                        {
-                            type: 'slider', // 滑动条型 dataZoom 组件
-                            start: 0,      // 默认起始位置为 0（即最左端）
-                            end: 100,       // 默认结束位置为 100（即最右端）
-                            height: 15, // 设置高度为10像素
-                        }
-                    
-				}
-				let allRes = {}
-            			if(!isnotopenvis){
-					this.dialogVisible = true
-				}
-                
-				res.data.msg.forEach(x=>{
-				    let tempOption_tmp = JSON.parse(JSON.stringify(tempOption));
-                    tempOption_tmp.xAxis.axisLabel.formatter = tempOption.xAxis.axisLabel.formatter
-				    let timeList = []
-				    let cpuList = []
-				    let fpsList = []
-				    let gpuList = []
-				    let memoryList = []
-				    let numThreadList = []
-				    let numHandlesList = []
-				    x.value.forEach(v=>{
-				        if (x.name == "cpu"){
-				            cpuList.push((v["cpu_usage(%)"]||v["cpu_usage(%)"]===0)?v["cpu_usage(%)"]:"-")
-				            timeList.push(v["time"])
-                           
-                        }else if(x.name == "fps"){
-                            fpsList.push(v["fps(帧)"]||v["fps(帧)"]===0?v["fps(帧)"]:"-")
-				            timeList.push(v["time"]?v["time"]:"-")
-                           
-				        }else if(x.name == "gpu"){
-                            gpuList.push(v["gpu(%)"]||v["gpu(%)"]===0?v["gpu(%)"]:"-")
-				            timeList.push(v["time"]?v["time"]:"-")
-                           
-				        }else if(x.name == "memory"){
-                            memoryList.push(v["process_memory_usage(M)"]||v["process_memory_usage(M)"]===0?v["process_memory_usage(M)"]:"-")
-				            timeList.push(v["time"]?v["time"]:"-")
-                           
-				        }else if(x.name == "process_info"){
-                            numHandlesList.push(v["num_handles(个)"]||v["num_handles(个)"]===0?v["num_handles(个)"]:"-")
-				            numThreadList.push(v["num_threads(个)"]||["num_threads(个)"]===0?v["num_threads(个)"]:"-")
-				            timeList.push(v["time"]?v["time"]:"-")
-                           
-				        }
-                    
-				    })
-
-                    tempOption_tmp.xAxis.data = timeList
-				    allRes[x.name] = tempOption_tmp
-
-				  if (x.name == "cpu"){
-                    tempOption_tmp.series.push(
-                                {
-                                    name: 'cpu_usage(%)',
-                                    type: 'line',
-                                    data: cpuList,
-                                    connectNulls: true,
-                                    areaStyle: {},
-
-                                  }
-                                
-				            )
-
-				        }else if(x.name == "fps"){
-				            tempOption_tmp.series.push(
-                                {
-                                    name: 'fps(帧)',
-                                    type: 'line',
-                                    data: fpsList,
-                                    connectNulls: true
-                                }
-				            )
-
-				        }else if(x.name == "gpu"){
-                            tempOption_tmp.series.push(
-                                {
-                                    name: 'gpu(%)',
-                                    type: 'line',
-                                    data: gpuList,
-                                    connectNulls: true,
-                                    areaStyle: {}
-                                }
-				            )
-
-				        }else if(x.name == "memory"){
-                            tempOption_tmp.series.push(
-                                {
-                                    name: 'process_memory_usage(M)',
-                                    type: 'line',
-                                    data: memoryList,
-                                    connectNulls: true,
-                                    areaStyle: {}
-                                }
-				            )
-
-				        }else if(x.name == "process_info"){
-                            tempOption_tmp.series.push(
-                                {
-                                    name: 'num_handles(个)',
-                                    type: 'line',
-                                    data: numHandlesList,
-                                    connectNulls: true
-                                }
-				            )
-				            tempOption_tmp.series.push(
-                                {
-                                    name: 'num_threads(个)',
-                                    type: 'line',
-                                    data: numThreadList,
-                                    connectNulls: true
-                                }
-				            )
-
-				        }
-				})
-				this.resultOption = allRes
-            },
-            num2time(clicktime){
-                if (!clicktime){
-                    return ""
-                }
-                const date = new Date(clicktime * 1000);
-                                // 使用toLocaleString方法格式化时间戳
-                                return date.toLocaleTimeString();
-            },
-            handleDialogVisibleChange(){
-                console.log(this.resultOption)
-                this.$nextTick(() => {
-                    let allRes = this.resultOption
-                    this.cpuChart = echarts.init(document.getElementById('cpuChart'));
-                    this.memoryChart = echarts.init(document.getElementById('memoryChart'));
-                    this.fpsChart = echarts.init(document.getElementById('fpsChart'));
-                    this.gpuChart = echarts.init(document.getElementById('gpuChart'));
-                    this.processInfoChart = echarts.init(document.getElementById('processInfoChart'));
-                    this.cpuChart.setOption(allRes["cpu"]);
-                    this.memoryChart.setOption(allRes["memory"]);
-                    this.fpsChart.setOption(allRes["fps"]);
-                    this.gpuChart.setOption(allRes["gpu"]);  
-                    this.processInfoChart.setOption(allRes["process_info"]);  
-                    this.syncDataZoom(this.cpuChart, [this.memoryChart, this.fpsChart, this.gpuChart, this.processInfoChart]);
-                    this.syncDataZoom(this.memoryChart, [this.cpuChart, this.fpsChart, this.gpuChart, this.processInfoChart]);
-                    this.syncDataZoom(this.fpsChart, [this.cpuChart, this.memoryChart, this.gpuChart, this.processInfoChart]);
-                    this.syncDataZoom(this.gpuChart, [this.cpuChart, this.memoryChart, this.fpsChart, this.processInfoChart]);
-                    this.syncDataZoom(this.processInfoChart, [this.cpuChart, this.memoryChart, this.fpsChart, this.gpuChart]);
-                    
-                });
-                this.intervalId = setInterval(() => {
-                    // 调用加载数据的函数
-                    if (!this.isloadres){
-                        this.reloadchart();
-                    }
-
-                }, 3000);
-                
-            },
-            async stop_task(taskId){
-                const res = await axios({method: 'get',//提交方法
-							url: '/stop_task/?task_id=' + taskId//提交地址
-				 })
-				 console.log(res.data)
-				 this.print_res(res)
-				await this.getAllTask()
-            },
-            print_res(res){
-                if (res.data.code == 200){
-                    this.$message({
-                      showClose: true,
-                      message: res.data.msg,
-                      type: 'success'
-                    });
-                }else{
-                    this.$message.error(res.data.msg);
-                }
-            },
-            async reloadchart(){
-                this.isloadres = true
-                await this.result(this.curtaskid, true)
-                let allRes = this.resultOption
-                this.cpuChart.setOption(allRes["cpu"]);
-                this.memoryChart.setOption(allRes["memory"]);
-                this.fpsChart.setOption(allRes["fps"]);
-                this.gpuChart.setOption(allRes["gpu"]);  
-                this.processInfoChart.setOption(allRes["process_info"]);  
-                this.isloadres = false
-            }
-
-        },
-        async mounted(){
-            await this.getAllTask();
-            await this.get_system_info()
-        }
-    });
-
-
-</script>
-</body>
-</html>
+<!DOCTYPE html>
+<html>
+<head>
+    <meta charset="UTF-8">
+    <title>性能测试报告</title>
+    <!-- 引入 Element UI CSS -->
+    <link href="https://unpkg.com/element-ui/lib/theme-chalk/index.css" rel="stylesheet">
+    <!-- 引入 Swiper CSS -->
+    <link href="https://unpkg.com/swiper@latest/swiper-bundle.min.css" rel="stylesheet">
+    <!-- 引入 Vue -->
+    <script src="https://cdn.bootcdn.net/ajax/libs/vue/2.6.14/vue.min.js"></script>
+    <!-- 引入 Element UI -->
+    <script src="https://unpkg.com/element-ui/lib/index.js"></script>
+    <!-- 引入 Axios -->
+    <script src="https://cdn.bootcdn.net/ajax/libs/axios/0.21.1/axios.min.js"></script>
+    <!-- 引入 ECharts -->
+    <script src="https://unpkg.com/echarts/dist/echarts.min.js"></script>
+    <!-- 引入 Swiper -->
+    <script src="https://unpkg.com/swiper@latest/swiper-bundle.min.js"></script>
+    <style>
+        /* 自定义样式 */
+        .el-aside {
+            background-color: #f2f2f2;
+        }
+        .task-button {
+            margin-bottom: 10px;
+        }
+		.headernavbar{
+			background-color: #3b4d6e;
+            color: #fff;
+            margin: 0;
+            padding: 0;
+            display: flex;
+            justify-content: space-between;
+            align-items: center;
+            height: 100%;
+		}
+		.headernavbar h1 {
+            margin: 0;
+            font-size: 18px;
+            color: #fff;
+        }
+        html, body {
+        margin: 0;
+        padding: 0;
+        height: 100%; /* 使 body 占满整个视口高度 */
+        }
+        .el-header{
+            margin:0;
+            padding:0;
+        }
+		.el-aside {
+            background-color: #fff;
+            box-shadow: 2px 0 8px rgba(0, 0, 0, .1);
+            flex: 0 0 200px;
+        }
+
+        .box-card {
+          border: none;
+          box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
+          border-radius: 8px;
+          overflow: hidden;
+        }
+
+        .box-card:hover {
+          box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
+          transition: box-shadow 0.3s ease-in-out;
+        }
+
+        .el-card__header {
+          background-color: #409eff;
+          color: white;
+          padding: 10px 20px;
+          font-size: 18px;
+          font-weight: bold;
+          border-radius: 8px 8px 0 0;
+        }
+
+        .el-card__body {
+          padding: 20px;
+        }
+
+        p {
+          margin: 0;
+          color: #333;
+          line-height: 1.6;
+        }
+
+        p span {
+          color: #409eff;
+          font-weight: bold;
+        }
+
+        @media (max-width: 600px) {
+          .box-card {
+            width: calc(100% - 20px);
+          }
+        }
+        .taskform {
+          margin: 50px auto;
+          padding: 20px;
+          background-color: #fff;
+          border-radius: 8px;
+          box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
+        }
+
+
+
+
+        /* 图表容器的基本样式 */
+.chart-container {
+  width: 50%; /* 占满容器宽度 */
+  max-width: 100%; /* 防止宽度超过容器 */
+  height: 400px; /* 默认高度 */
+  margin-bottom: 20px; /* 图表之间的间距 */
+  background-color: #ffffff; /* 背景颜色 */
+  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* 轻微的阴影效果 */
+  border-radius: 4px; /* 轻微的圆角 */
+  overflow: hidden; /* 隐藏溢出的内容 */
+}
+
+/* 图表标题样式 */
+.chart-title {
+  font-size: 1.1em;
+  font-weight: bold;
+  margin: 0 0 10px; /* 上下边距为0，下边距为10px */
+  padding: 10px;
+  background-color: #f2f2f2; /* 标题背景颜色 */
+  border-radius: 4px 4px 0 0; /* 仅上边缘圆角 */
+}
+
+/* 图表容器内的 ECharts 图表样式 */
+.echarts-chart {
+  width: 100%; /* 占满容器宽度 */
+  height: calc(100% - 30px); /* 减去标题的高度 */
+}
+
+
+    </style>
+</head>
+<body>
+<div id="app" style="margin:0;padding:0; height: 100%;">
+    <el-header style="height: 8%;">
+        <div class="headernavbar">
+            <svg class="icon" style="height: 3em;vertical-align: middle;fill: currentColor;overflow: hidden;"
+                 viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2539">
+                <path d="M467.104627 672.205804L110.431373 840.422902l348.300549 159.422745c24.636235 10.842353 43.670588 16.263529 57.123137 16.263529 13.452549 0 33.209725-5.421176 59.231372-16.263529L913.568627 840.44298l-356.673254-168.217098a105.251137 105.251137 0 0 0-89.790746 0z"
+                      fill="#797979" p-id="2540"></path>
+                <path d="M110.431373 791.752784v55.17553c202.912627 91.597804 319.006118 142.898196 348.300549 153.901176 43.951686 16.484392 58.287686 25.660235 129.244862-4.718431 47.304784-20.259137 155.828706-70.194196 325.591843-149.785098v-54.573177c-200.864627 93.043451-309.388549 142.817882-325.591843 149.303216-24.294902 9.758118-101.677176 18.713098-138.782117 0-24.736627-12.448627-137.657725-62.243137-338.763294-149.303216z"
+                      fill="#282F9A" p-id="2541"></path>
+                <path d="M467.104627 623.535686L110.431373 791.752784l348.300549 159.422745c24.636235 10.842353 43.670588 16.243451 57.123137 16.243451 13.452549 0 33.209725-5.421176 59.231372-16.243451L913.568627 791.752784l-356.673254-168.217098a105.251137 105.251137 0 0 0-89.790746 0z"
+                      fill="#727AFF" p-id="2542"></path>
+                <path d="M634.819765 43.369412l-195.604079 402.713098 160.326275 13.874196-110.933334 332.900392 269.050981-472.485647-132.116079-32.225882z"
+                      fill="#FFCB28" p-id="2543"></path>
+                <path d="M438.633412 458.189804l-101.355922 81.116863L595.425882 81.960157l39.393883-38.590745z"
+                      fill="#FF9D00" p-id="2544"></path>
+                <path d="M338.723137 538.001569h157.776314l112.097882-78.72753-163.84-12.609255z" fill="#CD7E00"
+                      p-id="2545"></path>
+                <path d="M496.499451 538.001569L455.981176 811.971765l32.727844-18.873726 117.559215-333.342117z"
+                      fill="#FF9D00" p-id="2546"></path>
+            </svg>
+            <h1>PC进程性能测试平台
+            </h1>
+        </div>
+    </el-header>
+    <el-container style="height: 90%;">
+        <!-- 侧边栏 -->
+        <el-aside style="width: 150px;">
+            <el-menu :default-active="1" class="el-menu-demo" style="border-right: solid 0px">
+                <el-menu-item index="1" class="task-button" @click="switchView('taskList');">
+                    <h3>任务列表</h3>
+                </el-menu-item>
+                <el-menu-item index="2" class="task-button" @click="switchView('createTask')">
+                    <h3>创建任务</h3>
+                </el-menu-item>
+            </el-menu>
+        </el-aside>
+        <!-- 内容区域 -->
+        <el-container>
+            <el-main>
+                <template v-if="currentView === 'taskList'">
+                    <el-table :data="tasks" style="width: 100%" height="100%">
+                        <el-table-column prop="name" label="任务名称" sortable></el-table-column>
+                        <el-table-column prop="serialno" label="被测设备" sortable></el-table-column>
+                        <el-table-column prop="target_pid" label="被测进程" sortable></el-table-column>
+                        <el-table-column prop="target_pid_name" label="进程名称" sortable></el-table-column>
+                        <el-table-column prop="status" label="任务状态" sortable>
+                            <template slot-scope="scope">
+                                <el-button type="info" size="mini" v-if="scope.row.status==0">待执行</el-button>
+                                <el-button type="primary" size="mini" v-if="scope.row.status==1">执行中</el-button>
+                                <el-button type="danger" size="mini" v-if="scope.row.status==-1">执行失败</el-button>
+                                <el-button type="success" size="mini" v-if="scope.row.status==2">执行完成</el-button>
+                            </template>
+                        </el-table-column>
+                        <el-table-column prop="platform" label="设备平台" sortable></el-table-column>
+                        <el-table-column prop="start_time" label="开始时间" sortable></el-table-column>
+                        <el-table-column prop="end_time" label="结束时间" sortable></el-table-column>
+                        <el-table-column label="操作">
+                            <template slot-scope="scope">
+                                <el-button type="danger" size="mini" v-if="scope.row.status==1"
+                                           @click="stop_task(scope.row.id)">停止任务
+                                </el-button>
+                                <el-button type="danger" size="mini" v-if="scope.row.status!=1"
+                                           @click="delete_task(scope.row.id)">删除任务
+                                </el-button>
+                                <el-button type="primary" size="mini" v-if="scope.row.status!=0||scope.row.status!=-1"
+                                           @click="result(scope.row.id);curtaskid=scope.row.id;">查看结果
+                                </el-button>
+                            </template>
+                        </el-table-column>
+                    </el-table>
+                </template>
+                <template v-if="currentView === 'createTask'">
+                    <el-card class="box-card">
+                        <div slot="header" class="clearfix">
+                            <span>设备信息</span>
+                        </div>
+                        <div>
+                            <p>平台: <span>{{ currentSystemInfo.platform }}</span></p>
+                            <p>计算机名称: <span>{{ currentSystemInfo.computer_name }}</span></p>
+                            <p>CPU 核心数: <span>{{ currentSystemInfo.cpu_cores }}</span></p>
+                            <p>RAM: <span>{{ currentSystemInfo.ram }}</span></p>
+                            <p>ROM: <span>{{ currentSystemInfo.rom }}</span></p>
+                        </div>
+                    </el-card>
+                    <el-form ref="newTask" :model="newTask" label-width="5%" class="taskform">
+                        <el-form-item label="任务名称">
+                            <el-input v-model="newTask.name" placeholder="请输入任务名称" clearable></el-input>
+                        </el-form-item>
+                        <el-form-item label="选择 PID">
+                            <el-select v-model="newTask.pid" filterable placeholder="请选择 PID"
+                                       @visible-change="get_pids"
+                                       @change="getPidCmd">
+                                <el-option
+                                        v-for="pid in pids"
+                                        :key="pid.pid"
+                                        :label="pid.name + '_' + pid.pid"
+                                        :value="pid.pid">
+                                </el-option>
+                            </el-select>
+                        </el-form-item>
+                        <el-form-item v-if="cmd" label="pid cmd">
+                            {{cmd}}
+                        </el-form-item>
+                        <el-form-item v-if="cmd" label="pid 截图">
+                            <el-image
+                                    style="width: 100%; height: 100%"
+                                    :src=pid_img
+                            >
+                                <div slot="error" class="image-slot">
+                                </div>
+                            </el-image>
+                        </el-form-item>
+                        <el-form-item>
+                            <el-button type="primary" @click="createTask">创建任务</el-button>
+                        </el-form-item>
+                    </el-form>
+                </template>
+            </el-main>
+        </el-container>
+    </el-container>
+    <el-dialog
+            :visible.sync="dialogVisible"
+            width="80%"
+            @open="handleDialogVisibleChange"
+            @closed="clearInterval(intervalId);"
+            @destroy-on-close="true"
+    >
+        <div style="display: flex;flex-direction: row;flex-wrap: wrap;">
+
+            <div class="chart-container">
+                <div class="chart-title">{{num2time(clicktime)}}进程截图</div>
+                <div class="demo-image">
+                    <el-image
+                            style="width: 100%; height: 100%"
+                            :src='"/static/" + this.opentaskid + "/screenshot/" + this.clicktime + ".png"'
+                    >
+                        <div slot="error" class="image-slot">
+                        </div>
+                    </el-image>
+
+                </div>
+            </div>
+
+
+            <div class="chart-container">
+                <div class="chart-title">
+                    CPU 使用率
+                </div>
+                <div id="cpuChart" class="echarts-chart"></div>
+
+            </div>
+            <div class="chart-container">
+                <div class="chart-title">内存使用量</div>
+                <div id="memoryChart" class="echarts-chart"></div>
+
+            </div>
+            <div class="chart-container">
+                <div class="chart-title">FPS</div>
+                <div id="fpsChart" class="echarts-chart"></div>
+
+            </div>
+            <div class="chart-container">
+                <div class="chart-title">GPU 使用率</div>
+                <div id="gpuChart" class="echarts-chart"></div>
+
+            </div>
+            <div class="chart-container">
+                <div class="chart-title">线程数与句柄数</div>
+                <div id="processInfoChart" class="echarts-chart"></div>
+
+            </div>
+
+        </div>
+    </el-dialog>
+</div>
+
+<script>
+    new Vue({
+        el: '#app',
+        data: function() {
+            return {
+                dialogVisible: false,
+                currentSystemInfo: null,
+                currentView: 'taskList', // 当前视图，默认为任务列表
+                newTask: { // 新任务对象
+                    name: this.getCurrentTimestamp(),
+                    pid: null
+                },
+                pids: [],
+                tasks: [ // 任务列表数据
+
+                ],
+                cmd: '',
+                pid_name: '',
+                pid_img: '',
+                resultOption: null,
+                cpuChart: null,
+                memoryChart: null,
+                fpsChart: null,
+                gpuChart: null,
+                processInfoChart: null,
+                clicktime: null,
+                opentaskid: null, 
+                curtaskid: null,
+                intervalId: null,
+                isloadres: false,
+            };
+        },
+        methods: {
+            switchView(view) {
+                this.currentView = view;
+                this.getAllTask().then()
+            },
+            getCurrentTimestamp() {
+              const date = new Date();
+              const year = date.getFullYear();
+              const month = (date.getMonth() + 1).toString().padStart(2, '0'); // 月份从0开始，所以加1
+              const day = date.getDate().toString().padStart(2, '0');
+              const hours = date.getHours().toString().padStart(2, '0');
+              const minutes = date.getMinutes().toString().padStart(2, '0');
+              const seconds = date.getSeconds().toString().padStart(2, '0');
+
+              return `${year}-${month}-${day} ${hours}:${minutes}:${seconds}`;
+            },
+            getPidCmd(){
+                for (let i = 0; i < this.pids.length; i++) {
+                  if (this.newTask.pid === this.pids[i].pid) {
+                      this.cmd = this.pids[i].cmd.join(" ");
+                      this.pid_name = this.pids[i].name
+                  }
+                }
+                this.getPidImg()
+
+            },
+            syncDataZoom(chartInstance, otherCharts) {
+                chartInstance.getZr().on('click', (params) => {
+                        const pointInPixel = [params.offsetX, params.offsetY];
+                        if (chartInstance.containPixel("grid", pointInPixel)) {
+                            // 转换像素坐标到数据坐标
+                            // 将像素坐标转换为 x 轴的数据索引
+                            let xIndex = chartInstance.convertFromPixel({seriesIndex: 0}, pointInPixel)[0];
+                            let xAxisData = chartInstance.getOption().xAxis[0].data;
+                            let xAxisValue = xAxisData[xIndex];
+                            this.clicktime = xAxisValue
+                            console.log(this.clicktime)
+                            chartInstance.dispatchAction({
+                                type: "brush",
+                                areas: [
+                                {
+                                    brushType: "lineX",
+                                    coordRange: [
+                                        xIndex,
+                                        xIndex,
+                                    ],
+                                    xAxisIndex: 0,
+                                    transformable: false,
+                                },
+                                ],
+                            });
+                            for(let index in otherCharts){
+                                otherCharts[index].dispatchAction({
+                                    type: "brush",
+                                    areas: [
+                                    {
+                                        brushType: "lineX",
+                                        coordRange: [
+                                            xIndex,
+                                            xIndex,
+                                        ],
+                                        xAxisIndex: 0,
+                                        transformable: false,
+                                    },
+                                    ],
+                                }); 
+                            }
+                        }
+                    
+                    });
+            },
+            async get_pids() {
+                const res = await axios({method: 'get',//提交方法
+                            url: '/get_pids/'
+                 })
+				 console.log(res)
+				 this.pids = res.data.msg
+            },
+            async get_system_info() {
+                const res = await axios({method: 'get',//提交方法
+                            url: '/system_info/'
+                 })
+				 console.log(res)
+
+				 this.currentSystemInfo = res.data.msg
+            },
+            async createTask() {
+                const res = await axios({method: 'get',//提交方法
+                            url: '/run_task/?pid='+this.newTask.pid+'&task_name='+this.newTask.name+'&pid_name='+this.pid_name//提交地址
+                 })
+                 this.print_res(res)
+				 console.log(res)
+            },
+            async getAllTask(){
+                 const res = await axios({method: 'get',//提交方法
+							url: '/get_all_task/'//提交地址
+				 })
+				 console.log(res)
+				 this.tasks = res.data.msg
+            },
+            async getPidImg(){
+                 const res = await axios({method: 'get',//提交方法
+							url: '/pid_img/?pid=' + this.newTask.pid//提交地址
+				 })
+				 console.log(res)
+				 this.pid_img = "data:image/png;base64," + res.data
+            },
+            async delete_task(taskId){
+                    const res = await axios({method: 'get',//提交方法
+                                    url: '/delete_task/?task_id=' + taskId//提交地址
+                         })
+                         this.print_res(res)
+				 console.log(res.data)
+				 await this.getAllTask()
+            },
+            async result(taskId, isnotopenvis){
+		const res = await axios({method: 'get',//提交方法
+							url: '/result/?task_id=' + taskId//提交地址
+				 })
+                this.opentaskid = taskId
+				let tempOption={
+				      legend: {
+                        show: true
+                      },
+				      tooltip: {
+                        trigger: 'axis',
+                        axisPointer: {
+                            type: 'cross',
+                            crossStyle: {
+                                color: '#999'
+                            }
+                        }
+                    },
+                    xAxis: {
+                        type: 'category',
+                        boundaryGap: false,
+                        data: [/* 时间戳数据 */],
+                        axisPointer: {
+                            type: 'shadow'
+                        },
+                        axisLabel: {
+                            formatter: timestamp => {
+                                // 将Unix时间戳转换为JavaScript的Date对象
+                                const date = new Date(timestamp * 1000);
+                                // 使用toLocaleString方法格式化时间戳
+                                return date.toLocaleTimeString();
+                                }
+                        }
+                    },
+                    yAxis: {
+                        type: 'value'
+                    },
+                    series: [
+
+                    ],
+                    toolbox: {
+                     show: false,
+                    },
+                    brush: {
+                        xAxisIndex: "all",
+                        brushLink: "all",
+                        brushStyle: {
+                            borderWidth: 3,
+                            color: 'rgba(255,36,36,0.2)',
+                            borderColor: '#ff2424'
+                        }
+                    },
+                    markArea:{},
+					clickable: true,
+					symbol: 'circle',
+                    lineStyle: {
+							width: 0.5,
+					},
+                    showSymbol: false,//是否默认展示圆点
+                    dataZoom: 
+                        {
+                            type: 'slider', // 滑动条型 dataZoom 组件
+                            start: 0,      // 默认起始位置为 0（即最左端）
+                            end: 100,       // 默认结束位置为 100（即最右端）
+                            height: 15, // 设置高度为10像素
+                        }
+                    
+				}
+				let allRes = {}
+            			if(!isnotopenvis){
+					this.dialogVisible = true
+				}
+                
+				res.data.msg.forEach(x=>{
+				    let tempOption_tmp = JSON.parse(JSON.stringify(tempOption));
+                    tempOption_tmp.xAxis.axisLabel.formatter = tempOption.xAxis.axisLabel.formatter
+				    let timeList = []
+				    let cpuList = []
+				    let fpsList = []
+				    let gpuList = []
+				    let memoryList = []
+				    let numThreadList = []
+				    let numHandlesList = []
+				    x.value.forEach(v=>{
+				        if (x.name == "cpu"){
+				            cpuList.push((v["cpu_usage(%)"]||v["cpu_usage(%)"]===0)?v["cpu_usage(%)"]:"-")
+				            timeList.push(v["time"])
+                           
+                        }else if(x.name == "fps"){
+                            fpsList.push(v["fps(帧)"]||v["fps(帧)"]===0?v["fps(帧)"]:"-")
+				            timeList.push(v["time"]?v["time"]:"-")
+                           
+				        }else if(x.name == "gpu"){
+                            gpuList.push(v["gpu(%)"]||v["gpu(%)"]===0?v["gpu(%)"]:"-")
+				            timeList.push(v["time"]?v["time"]:"-")
+                           
+				        }else if(x.name == "memory"){
+                            memoryList.push(v["process_memory_usage(M)"]||v["process_memory_usage(M)"]===0?v["process_memory_usage(M)"]:"-")
+				            timeList.push(v["time"]?v["time"]:"-")
+                           
+				        }else if(x.name == "process_info"){
+                            numHandlesList.push(v["num_handles(个)"]||v["num_handles(个)"]===0?v["num_handles(个)"]:"-")
+				            numThreadList.push(v["num_threads(个)"]||["num_threads(个)"]===0?v["num_threads(个)"]:"-")
+				            timeList.push(v["time"]?v["time"]:"-")
+                           
+				        }
+                    
+				    })
+
+                    tempOption_tmp.xAxis.data = timeList
+				    allRes[x.name] = tempOption_tmp
+
+				  if (x.name == "cpu"){
+                    tempOption_tmp.series.push(
+                                {
+                                    name: 'cpu_usage(%)',
+                                    type: 'line',
+                                    data: cpuList,
+                                    connectNulls: true,
+                                    areaStyle: {},
+
+                                  }
+                                
+				            )
+
+				        }else if(x.name == "fps"){
+				            tempOption_tmp.series.push(
+                                {
+                                    name: 'fps(帧)',
+                                    type: 'line',
+                                    data: fpsList,
+                                    connectNulls: true
+                                }
+				            )
+
+				        }else if(x.name == "gpu"){
+                            tempOption_tmp.series.push(
+                                {
+                                    name: 'gpu(%)',
+                                    type: 'line',
+                                    data: gpuList,
+                                    connectNulls: true,
+                                    areaStyle: {}
+                                }
+				            )
+
+				        }else if(x.name == "memory"){
+                            tempOption_tmp.series.push(
+                                {
+                                    name: 'process_memory_usage(M)',
+                                    type: 'line',
+                                    data: memoryList,
+                                    connectNulls: true,
+                                    areaStyle: {}
+                                }
+				            )
+
+				        }else if(x.name == "process_info"){
+                            tempOption_tmp.series.push(
+                                {
+                                    name: 'num_handles(个)',
+                                    type: 'line',
+                                    data: numHandlesList,
+                                    connectNulls: true
+                                }
+				            )
+				            tempOption_tmp.series.push(
+                                {
+                                    name: 'num_threads(个)',
+                                    type: 'line',
+                                    data: numThreadList,
+                                    connectNulls: true
+                                }
+				            )
+
+				        }
+				})
+				this.resultOption = allRes
+            },
+            num2time(clicktime){
+                if (!clicktime){
+                    return ""
+                }
+                const date = new Date(clicktime * 1000);
+                                // 使用toLocaleString方法格式化时间戳
+                                return date.toLocaleTimeString();
+            },
+            handleDialogVisibleChange(){
+                console.log(this.resultOption)
+                this.$nextTick(() => {
+                    let allRes = this.resultOption
+                    this.cpuChart = echarts.init(document.getElementById('cpuChart'));
+                    this.memoryChart = echarts.init(document.getElementById('memoryChart'));
+                    this.fpsChart = echarts.init(document.getElementById('fpsChart'));
+                    this.gpuChart = echarts.init(document.getElementById('gpuChart'));
+                    this.processInfoChart = echarts.init(document.getElementById('processInfoChart'));
+                    this.cpuChart.setOption(allRes["cpu"]);
+                    this.memoryChart.setOption(allRes["memory"]);
+                    this.fpsChart.setOption(allRes["fps"]);
+                    this.gpuChart.setOption(allRes["gpu"]);  
+                    this.processInfoChart.setOption(allRes["process_info"]);  
+                    this.syncDataZoom(this.cpuChart, [this.memoryChart, this.fpsChart, this.gpuChart, this.processInfoChart]);
+                    this.syncDataZoom(this.memoryChart, [this.cpuChart, this.fpsChart, this.gpuChart, this.processInfoChart]);
+                    this.syncDataZoom(this.fpsChart, [this.cpuChart, this.memoryChart, this.gpuChart, this.processInfoChart]);
+                    this.syncDataZoom(this.gpuChart, [this.cpuChart, this.memoryChart, this.fpsChart, this.processInfoChart]);
+                    this.syncDataZoom(this.processInfoChart, [this.cpuChart, this.memoryChart, this.fpsChart, this.gpuChart]);
+                    
+                });
+                this.intervalId = setInterval(() => {
+                    // 调用加载数据的函数
+                    if (!this.isloadres){
+                        this.reloadchart();
+                    }
+
+                }, 3000);
+                
+            },
+            async stop_task(taskId){
+                const res = await axios({method: 'get',//提交方法
+							url: '/stop_task/?task_id=' + taskId//提交地址
+				 })
+				 console.log(res.data)
+				 this.print_res(res)
+				await this.getAllTask()
+            },
+            print_res(res){
+                if (res.data.code == 200){
+                    this.$message({
+                      showClose: true,
+                      message: res.data.msg,
+                      type: 'success'
+                    });
+                }else{
+                    this.$message.error(res.data.msg);
+                }
+            },
+            async reloadchart(){
+                this.isloadres = true
+                await this.result(this.curtaskid, true)
+                let allRes = this.resultOption
+                this.cpuChart.setOption(allRes["cpu"]);
+                this.memoryChart.setOption(allRes["memory"]);
+                this.fpsChart.setOption(allRes["fps"]);
+                this.gpuChart.setOption(allRes["gpu"]);  
+                this.processInfoChart.setOption(allRes["process_info"]);  
+                this.isloadres = false
+            }
+
+        },
+        async mounted(){
+            await this.getAllTask();
+            await this.get_system_info()
+        }
+    });
+
+
+</script>
+</body>
+</html>
```

