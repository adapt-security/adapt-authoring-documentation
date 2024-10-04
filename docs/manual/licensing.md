# Licensing
When building a business around an open-source product, it is crucially important to understand how that code is licensed, and how those licenses apply to your business. This page aims to clarify which licenses apply to the Adapt authoring tool core package, and gives details on how those licenses may affect its use. **This page is not intended to provide legal advice; qualified legal professionals should be consulted to advise on how your own business may be affected.**

The Adapt authoring tool core package is licensed under the **GNU General Public License v3.0**, which is summarised as follows:

_Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights._

The GNU General Public License v3.0 allows the following:

- Commercial use
- Modifications
- Distribution
- Patent use
- Private use

You can view more information on the GNU General Public License v3.0 license in [License details](#license-details).

## Third-party dependencies

The Adapt authoring tool makes use of 757 third-party Node.js modules. These include transient dependencies (i.e. dependencies not directly imported by the authoring tool code, but used by its dependencies). Each module has its own license which must be taken into consideration when building a business around Adapt products. 

The below table lists all licenses used, as well as the number of dependencies which use each license.

| License | Modules using license |
| - | :-: |
| 0BSD | 2 |
| Apache-2.0 | 25 |
| BSD-2-Clause | 16 |
| BSD-3-Clause | 14 |
| BlueOak-1.0.0 | 3 |
| CC-BY-4.0 | 1 |
| GPL-3.0 | 3 |
| ISC | 44 |
| MIT | 638 |
| MIT-0 | 1 |
| MPL-2.0 | 1 |
| Python-2.0 | 1 |
| Unlicense | 2 |
| WTFPL | 1 |


## License details

Listed below are all licenses used by the Adapt authoring tool and its dependencies. Click each heading to view detailed information, including the full licenses themselves.

<details>
<summary>The Unlicense (Unlicense)</summary>
<p>A license with no conditions whatsoever which dedicates works to the public domain. Unlicensed works, modifications, and larger works may be distributed under different terms and without source code.</p>
<p>This license allows the following:
<ul><li>Private use</li>
<li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li></ul></p>
<p>The original license text is as follows:</p>
<pre>This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <https://unlicense.org>
</pre>
</details>

<details>
<summary>MIT License (MIT)</summary>
<p>A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
</pre>
</details>

<details>
<summary>ISC License (ISC)</summary>
<p>A permissive license lets people do anything with your code with proper attribution and without warranty. The ISC license is functionally equivalent to the <a href="/licenses/bsd-2-clause/">BSD 2-Clause</a> and <a href="/licenses/mit/">MIT</a> licenses, removing some language that is no longer necessary.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Distribution</li>
<li>Modifications</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>ISC License

Copyright (c) [year] [fullname]

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
PERFORMANCE OF THIS SOFTWARE.
</pre>
</details>

<details>
<summary>Apache License 2.0 (Apache-2.0)</summary>
<p>A permissive license whose main conditions require preservation of copyright and license notices. Contributors provide an express grant of patent rights. Licensed works, modifications, and larger works may be distributed under different terms and without source code.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Patent use</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
      outstanding shares, or (iii) beneficial ownership of such entity.

      "You" (or "Your") shall mean an individual or Legal Entity
      exercising permissions granted by this License.

      "Source" form shall mean the preferred form for making modifications,
      including but not limited to software source code, documentation
      source, and configuration files.

      "Object" form shall mean any form resulting from mechanical
      transformation or translation of a Source form, including but
      not limited to compiled object code, generated documentation,
      and conversions to other media types.

      "Work" shall mean the work of authorship, whether in Source or
      Object form, made available under the License, as indicated by a
      copyright notice that is included in or attached to the work
      (an example is provided in the Appendix below).

      "Derivative Works" shall mean any work, whether in Source or Object
      form, that is based on (or derived from) the Work and for which the
      editorial revisions, annotations, elaborations, or other modifications
      represent, as a whole, an original work of authorship. For the purposes
      of this License, Derivative Works shall not include works that remain
      separable from, or merely link (or bind by name) to the interfaces of,
      the Work and Derivative Works thereof.

      "Contribution" shall mean any work of authorship, including
      the original version of the Work and any modifications or additions
      to that Work or Derivative Works thereof, that is intentionally
      submitted to Licensor for inclusion in the Work by the copyright owner
      or by an individual or Legal Entity authorized to submit on behalf of
      the copyright owner. For the purposes of this definition, "submitted"
      means any form of electronic, verbal, or written communication sent
      to the Licensor or its representatives, including but not limited to
      communication on electronic mailing lists, source code control systems,
      and issue tracking systems that are managed by, or on behalf of, the
      Licensor for the purpose of discussing and improving the Work, but
      excluding communication that is conspicuously marked or otherwise
      designated in writing by the copyright owner as "Not a Contribution."

      "Contributor" shall mean Licensor and any individual or Legal Entity
      on behalf of whom a Contribution has been received by Licensor and
      subsequently incorporated within the Work.

   2. Grant of Copyright License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      copyright license to reproduce, prepare Derivative Works of,
      publicly display, publicly perform, sublicense, and distribute the
      Work and such Derivative Works in Source or Object form.

   3. Grant of Patent License. Subject to the terms and conditions of
      this License, each Contributor hereby grants to You a perpetual,
      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
      (except as stated in this section) patent license to make, have made,
      use, offer to sell, sell, import, and otherwise transfer the Work,
      where such license applies only to those patent claims licensable
      by such Contributor that are necessarily infringed by their
      Contribution(s) alone or by combination of their Contribution(s)
      with the Work to which such Contribution(s) was submitted. If You
      institute patent litigation against any entity (including a
      cross-claim or counterclaim in a lawsuit) alleging that the Work
      or a Contribution incorporated within the Work constitutes direct
      or contributory patent infringement, then any patent licenses
      granted to You under this License for that Work shall terminate
      as of the date such litigation is filed.

   4. Redistribution. You may reproduce and distribute copies of the
      Work or Derivative Works thereof in any medium, with or without
      modifications, and in Source or Object form, provided that You
      meet the following conditions:

      (a) You must give any other recipients of the Work or
          Derivative Works a copy of this License; and

      (b) You must cause any modified files to carry prominent notices
          stating that You changed the files; and

      (c) You must retain, in the Source form of any Derivative Works
          that You distribute, all copyright, patent, trademark, and
          attribution notices from the Source form of the Work,
          excluding those notices that do not pertain to any part of
          the Derivative Works; and

      (d) If the Work includes a "NOTICE" text file as part of its
          distribution, then any Derivative Works that You distribute must
          include a readable copy of the attribution notices contained
          within such NOTICE file, excluding those notices that do not
          pertain to any part of the Derivative Works, in at least one
          of the following places: within a NOTICE text file distributed
          as part of the Derivative Works; within the Source form or
          documentation, if provided along with the Derivative Works; or,
          within a display generated by the Derivative Works, if and
          wherever such third-party notices normally appear. The contents
          of the NOTICE file are for informational purposes only and
          do not modify the License. You may add Your own attribution
          notices within Derivative Works that You distribute, alongside
          or as an addendum to the NOTICE text from the Work, provided
          that such additional attribution notices cannot be construed
          as modifying the License.

      You may add Your own copyright statement to Your modifications and
      may provide additional or different license terms and conditions
      for use, reproduction, or distribution of Your modifications, or
      for any such Derivative Works as a whole, provided Your use,
      reproduction, and distribution of the Work otherwise complies with
      the conditions stated in this License.

   5. Submission of Contributions. Unless You explicitly state otherwise,
      any Contribution intentionally submitted for inclusion in the Work
      by You to the Licensor shall be under the terms and conditions of
      this License, without any additional terms or conditions.
      Notwithstanding the above, nothing herein shall supersede or modify
      the terms of any separate license agreement you may have executed
      with Licensor regarding such Contributions.

   6. Trademarks. This License does not grant permission to use the trade
      names, trademarks, service marks, or product names of the Licensor,
      except as required for reasonable and customary use in describing the
      origin of the Work and reproducing the content of the NOTICE file.

   7. Disclaimer of Warranty. Unless required by applicable law or
      agreed to in writing, Licensor provides the Work (and each
      Contributor provides its Contributions) on an "AS IS" BASIS,
      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
      implied, including, without limitation, any warranties or conditions
      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
      PARTICULAR PURPOSE. You are solely responsible for determining the
      appropriateness of using or redistributing the Work and assume any
      risks associated with Your exercise of permissions under this License.

   8. Limitation of Liability. In no event and under no legal theory,
      whether in tort (including negligence), contract, or otherwise,
      unless required by applicable law (such as deliberate and grossly
      negligent acts) or agreed to in writing, shall any Contributor be
      liable to You for damages, including any direct, indirect, special,
      incidental, or consequential damages of any character arising as a
      result of this License or out of the use or inability to use the
      Work (including but not limited to damages for loss of goodwill,
      work stoppage, computer failure or malfunction, or any and all
      other commercial damages or losses), even if such Contributor
      has been advised of the possibility of such damages.

   9. Accepting Warranty or Additional Liability. While redistributing
      the Work or Derivative Works thereof, You may choose to offer,
      and charge a fee for, acceptance of support, warranty, indemnity,
      or other liability obligations and/or rights consistent with this
      License. However, in accepting such obligations, You may act only
      on Your own behalf and on Your sole responsibility, not on behalf
      of any other Contributor, and only if You agree to indemnify,
      defend, and hold each Contributor harmless for any liability
      incurred by, or claims asserted against, such Contributor by reason
      of your accepting any such warranty or additional liability.

   END OF TERMS AND CONDITIONS

   APPENDIX: How to apply the Apache License to your work.

      To apply the Apache License to your work, attach the following
      boilerplate notice, with the fields enclosed by brackets "[]"
      replaced with your own identifying information. (Don't include
      the brackets!)  The text should be enclosed in the appropriate
      comment syntax for the file format. We also recommend that a
      file or class name and description of purpose be included on the
      same "printed page" as the copyright notice for easier
      identification within third-party archives.

   Copyright [yyyy] [name of copyright owner]

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
</pre>
</details>

<details>
<summary>BSD 2-Clause "Simplified" License (BSD-2-Clause)</summary>
<p>A permissive license that comes in two variants, the <a href="/licenses/bsd-2-clause/">BSD 2-Clause</a> and <a href="/licenses/bsd-3-clause/">BSD 3-Clause</a>. Both have very minute differences to the MIT license.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>BSD 2-Clause License

Copyright (c) [year], [fullname]

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
</pre>
</details>

<details>
<summary>BSD Zero Clause License (0BSD)</summary>
<p>The BSD Zero Clause license goes further than the BSD 2-Clause license to allow you unlimited freedom with the software without requirements to include the copyright notice, license text, or disclaimer in either source or binary forms.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Distribution</li>
<li>Modifications</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>BSD Zero Clause License

Copyright (c) [year] [fullname]

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
PERFORMANCE OF THIS SOFTWARE.
</pre>
</details>

<details>
<summary>BSD 3-Clause "New" or "Revised" License (BSD-3-Clause)</summary>
<p>A permissive license similar to the <a href="/licenses/bsd-2-clause/">BSD 2-Clause License</a>, but with a 3rd clause that prohibits others from using the name of the copyright holder or its contributors to promote derived products without written consent.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>BSD 3-Clause License

Copyright (c) [year], [fullname]

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
</pre>
</details>

<details>
<summary>Do What The F*ck You Want To Public License (WTFPL)</summary>
<p>The easiest license out there. It gives the user permissions to do whatever they want with your code.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

 Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

  0. You just DO WHAT THE FUCK YOU WANT TO.
</pre>
</details>

<details>
<summary>MIT No Attribution (MIT-0)</summary>
<p>A short and simple permissive license with no conditions, not even requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>MIT No Attribution

Copyright [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
</pre>
</details>

<details>
<summary>GNU General Public License v3.0 (GPL-3.0)</summary>
<p>Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Patent use</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>                    GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007

 Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

                            Preamble

  The GNU General Public License is a free, copyleft license for
software and other kinds of works.

  The licenses for most software and other practical works are designed
to take away your freedom to share and change the works.  By contrast,
the GNU General Public License is intended to guarantee your freedom to
share and change all versions of a program--to make sure it remains free
software for all its users.  We, the Free Software Foundation, use the
GNU General Public License for most of our software; it applies also to
any other work released this way by its authors.  You can apply it to
your programs, too.

  When we speak of free software, we are referring to freedom, not
price.  Our General Public Licenses are designed to make sure that you
have the freedom to distribute copies of free software (and charge for
them if you wish), that you receive source code or can get it if you
want it, that you can change the software or use pieces of it in new
free programs, and that you know you can do these things.

  To protect your rights, we need to prevent others from denying you
these rights or asking you to surrender the rights.  Therefore, you have
certain responsibilities if you distribute copies of the software, or if
you modify it: responsibilities to respect the freedom of others.

  For example, if you distribute copies of such a program, whether
gratis or for a fee, you must pass on to the recipients the same
freedoms that you received.  You must make sure that they, too, receive
or can get the source code.  And you must show them these terms so they
know their rights.

  Developers that use the GNU GPL protect your rights with two steps:
(1) assert copyright on the software, and (2) offer you this License
giving you legal permission to copy, distribute and/or modify it.

  For the developers' and authors' protection, the GPL clearly explains
that there is no warranty for this free software.  For both users' and
authors' sake, the GPL requires that modified versions be marked as
changed, so that their problems will not be attributed erroneously to
authors of previous versions.

  Some devices are designed to deny users access to install or run
modified versions of the software inside them, although the manufacturer
can do so.  This is fundamentally incompatible with the aim of
protecting users' freedom to change the software.  The systematic
pattern of such abuse occurs in the area of products for individuals to
use, which is precisely where it is most unacceptable.  Therefore, we
have designed this version of the GPL to prohibit the practice for those
products.  If such problems arise substantially in other domains, we
stand ready to extend this provision to those domains in future versions
of the GPL, as needed to protect the freedom of users.

  Finally, every program is threatened constantly by software patents.
States should not allow patents to restrict development and use of
software on general-purpose computers, but in those that do, we wish to
avoid the special danger that patents applied to a free program could
make it effectively proprietary.  To prevent this, the GPL assures that
patents cannot be used to render the program non-free.

  The precise terms and conditions for copying, distribution and
modification follow.

                       TERMS AND CONDITIONS

  0. Definitions.

  "This License" refers to version 3 of the GNU General Public License.

  "Copyright" also means copyright-like laws that apply to other kinds of
works, such as semiconductor masks.

  "The Program" refers to any copyrightable work licensed under this
License.  Each licensee is addressed as "you".  "Licensees" and
"recipients" may be individuals or organizations.

  To "modify" a work means to copy from or adapt all or part of the work
in a fashion requiring copyright permission, other than the making of an
exact copy.  The resulting work is called a "modified version" of the
earlier work or a work "based on" the earlier work.

  A "covered work" means either the unmodified Program or a work based
on the Program.

  To "propagate" a work means to do anything with it that, without
permission, would make you directly or secondarily liable for
infringement under applicable copyright law, except executing it on a
computer or modifying a private copy.  Propagation includes copying,
distribution (with or without modification), making available to the
public, and in some countries other activities as well.

  To "convey" a work means any kind of propagation that enables other
parties to make or receive copies.  Mere interaction with a user through
a computer network, with no transfer of a copy, is not conveying.

  An interactive user interface displays "Appropriate Legal Notices"
to the extent that it includes a convenient and prominently visible
feature that (1) displays an appropriate copyright notice, and (2)
tells the user that there is no warranty for the work (except to the
extent that warranties are provided), that licensees may convey the
work under this License, and how to view a copy of this License.  If
the interface presents a list of user commands or options, such as a
menu, a prominent item in the list meets this criterion.

  1. Source Code.

  The "source code" for a work means the preferred form of the work
for making modifications to it.  "Object code" means any non-source
form of a work.

  A "Standard Interface" means an interface that either is an official
standard defined by a recognized standards body, or, in the case of
interfaces specified for a particular programming language, one that
is widely used among developers working in that language.

  The "System Libraries" of an executable work include anything, other
than the work as a whole, that (a) is included in the normal form of
packaging a Major Component, but which is not part of that Major
Component, and (b) serves only to enable use of the work with that
Major Component, or to implement a Standard Interface for which an
implementation is available to the public in source code form.  A
"Major Component", in this context, means a major essential component
(kernel, window system, and so on) of the specific operating system
(if any) on which the executable work runs, or a compiler used to
produce the work, or an object code interpreter used to run it.

  The "Corresponding Source" for a work in object code form means all
the source code needed to generate, install, and (for an executable
work) run the object code and to modify the work, including scripts to
control those activities.  However, it does not include the work's
System Libraries, or general-purpose tools or generally available free
programs which are used unmodified in performing those activities but
which are not part of the work.  For example, Corresponding Source
includes interface definition files associated with source files for
the work, and the source code for shared libraries and dynamically
linked subprograms that the work is specifically designed to require,
such as by intimate data communication or control flow between those
subprograms and other parts of the work.

  The Corresponding Source need not include anything that users
can regenerate automatically from other parts of the Corresponding
Source.

  The Corresponding Source for a work in source code form is that
same work.

  2. Basic Permissions.

  All rights granted under this License are granted for the term of
copyright on the Program, and are irrevocable provided the stated
conditions are met.  This License explicitly affirms your unlimited
permission to run the unmodified Program.  The output from running a
covered work is covered by this License only if the output, given its
content, constitutes a covered work.  This License acknowledges your
rights of fair use or other equivalent, as provided by copyright law.

  You may make, run and propagate covered works that you do not
convey, without conditions so long as your license otherwise remains
in force.  You may convey covered works to others for the sole purpose
of having them make modifications exclusively for you, or provide you
with facilities for running those works, provided that you comply with
the terms of this License in conveying all material for which you do
not control copyright.  Those thus making or running the covered works
for you must do so exclusively on your behalf, under your direction
and control, on terms that prohibit them from making any copies of
your copyrighted material outside their relationship with you.

  Conveying under any other circumstances is permitted solely under
the conditions stated below.  Sublicensing is not allowed; section 10
makes it unnecessary.

  3. Protecting Users' Legal Rights From Anti-Circumvention Law.

  No covered work shall be deemed part of an effective technological
measure under any applicable law fulfilling obligations under article
11 of the WIPO copyright treaty adopted on 20 December 1996, or
similar laws prohibiting or restricting circumvention of such
measures.

  When you convey a covered work, you waive any legal power to forbid
circumvention of technological measures to the extent such circumvention
is effected by exercising rights under this License with respect to
the covered work, and you disclaim any intention to limit operation or
modification of the work as a means of enforcing, against the work's
users, your or third parties' legal rights to forbid circumvention of
technological measures.

  4. Conveying Verbatim Copies.

  You may convey verbatim copies of the Program's source code as you
receive it, in any medium, provided that you conspicuously and
appropriately publish on each copy an appropriate copyright notice;
keep intact all notices stating that this License and any
non-permissive terms added in accord with section 7 apply to the code;
keep intact all notices of the absence of any warranty; and give all
recipients a copy of this License along with the Program.

  You may charge any price or no price for each copy that you convey,
and you may offer support or warranty protection for a fee.

  5. Conveying Modified Source Versions.

  You may convey a work based on the Program, or the modifications to
produce it from the Program, in the form of source code under the
terms of section 4, provided that you also meet all of these conditions:

    a) The work must carry prominent notices stating that you modified
    it, and giving a relevant date.

    b) The work must carry prominent notices stating that it is
    released under this License and any conditions added under section
    7.  This requirement modifies the requirement in section 4 to
    "keep intact all notices".

    c) You must license the entire work, as a whole, under this
    License to anyone who comes into possession of a copy.  This
    License will therefore apply, along with any applicable section 7
    additional terms, to the whole of the work, and all its parts,
    regardless of how they are packaged.  This License gives no
    permission to license the work in any other way, but it does not
    invalidate such permission if you have separately received it.

    d) If the work has interactive user interfaces, each must display
    Appropriate Legal Notices; however, if the Program has interactive
    interfaces that do not display Appropriate Legal Notices, your
    work need not make them do so.

  A compilation of a covered work with other separate and independent
works, which are not by their nature extensions of the covered work,
and which are not combined with it such as to form a larger program,
in or on a volume of a storage or distribution medium, is called an
"aggregate" if the compilation and its resulting copyright are not
used to limit the access or legal rights of the compilation's users
beyond what the individual works permit.  Inclusion of a covered work
in an aggregate does not cause this License to apply to the other
parts of the aggregate.

  6. Conveying Non-Source Forms.

  You may convey a covered work in object code form under the terms
of sections 4 and 5, provided that you also convey the
machine-readable Corresponding Source under the terms of this License,
in one of these ways:

    a) Convey the object code in, or embodied in, a physical product
    (including a physical distribution medium), accompanied by the
    Corresponding Source fixed on a durable physical medium
    customarily used for software interchange.

    b) Convey the object code in, or embodied in, a physical product
    (including a physical distribution medium), accompanied by a
    written offer, valid for at least three years and valid for as
    long as you offer spare parts or customer support for that product
    model, to give anyone who possesses the object code either (1) a
    copy of the Corresponding Source for all the software in the
    product that is covered by this License, on a durable physical
    medium customarily used for software interchange, for a price no
    more than your reasonable cost of physically performing this
    conveying of source, or (2) access to copy the
    Corresponding Source from a network server at no charge.

    c) Convey individual copies of the object code with a copy of the
    written offer to provide the Corresponding Source.  This
    alternative is allowed only occasionally and noncommercially, and
    only if you received the object code with such an offer, in accord
    with subsection 6b.

    d) Convey the object code by offering access from a designated
    place (gratis or for a charge), and offer equivalent access to the
    Corresponding Source in the same way through the same place at no
    further charge.  You need not require recipients to copy the
    Corresponding Source along with the object code.  If the place to
    copy the object code is a network server, the Corresponding Source
    may be on a different server (operated by you or a third party)
    that supports equivalent copying facilities, provided you maintain
    clear directions next to the object code saying where to find the
    Corresponding Source.  Regardless of what server hosts the
    Corresponding Source, you remain obligated to ensure that it is
    available for as long as needed to satisfy these requirements.

    e) Convey the object code using peer-to-peer transmission, provided
    you inform other peers where the object code and Corresponding
    Source of the work are being offered to the general public at no
    charge under subsection 6d.

  A separable portion of the object code, whose source code is excluded
from the Corresponding Source as a System Library, need not be
included in conveying the object code work.

  A "User Product" is either (1) a "consumer product", which means any
tangible personal property which is normally used for personal, family,
or household purposes, or (2) anything designed or sold for incorporation
into a dwelling.  In determining whether a product is a consumer product,
doubtful cases shall be resolved in favor of coverage.  For a particular
product received by a particular user, "normally used" refers to a
typical or common use of that class of product, regardless of the status
of the particular user or of the way in which the particular user
actually uses, or expects or is expected to use, the product.  A product
is a consumer product regardless of whether the product has substantial
commercial, industrial or non-consumer uses, unless such uses represent
the only significant mode of use of the product.

  "Installation Information" for a User Product means any methods,
procedures, authorization keys, or other information required to install
and execute modified versions of a covered work in that User Product from
a modified version of its Corresponding Source.  The information must
suffice to ensure that the continued functioning of the modified object
code is in no case prevented or interfered with solely because
modification has been made.

  If you convey an object code work under this section in, or with, or
specifically for use in, a User Product, and the conveying occurs as
part of a transaction in which the right of possession and use of the
User Product is transferred to the recipient in perpetuity or for a
fixed term (regardless of how the transaction is characterized), the
Corresponding Source conveyed under this section must be accompanied
by the Installation Information.  But this requirement does not apply
if neither you nor any third party retains the ability to install
modified object code on the User Product (for example, the work has
been installed in ROM).

  The requirement to provide Installation Information does not include a
requirement to continue to provide support service, warranty, or updates
for a work that has been modified or installed by the recipient, or for
the User Product in which it has been modified or installed.  Access to a
network may be denied when the modification itself materially and
adversely affects the operation of the network or violates the rules and
protocols for communication across the network.

  Corresponding Source conveyed, and Installation Information provided,
in accord with this section must be in a format that is publicly
documented (and with an implementation available to the public in
source code form), and must require no special password or key for
unpacking, reading or copying.

  7. Additional Terms.

  "Additional permissions" are terms that supplement the terms of this
License by making exceptions from one or more of its conditions.
Additional permissions that are applicable to the entire Program shall
be treated as though they were included in this License, to the extent
that they are valid under applicable law.  If additional permissions
apply only to part of the Program, that part may be used separately
under those permissions, but the entire Program remains governed by
this License without regard to the additional permissions.

  When you convey a copy of a covered work, you may at your option
remove any additional permissions from that copy, or from any part of
it.  (Additional permissions may be written to require their own
removal in certain cases when you modify the work.)  You may place
additional permissions on material, added by you to a covered work,
for which you have or can give appropriate copyright permission.

  Notwithstanding any other provision of this License, for material you
add to a covered work, you may (if authorized by the copyright holders of
that material) supplement the terms of this License with terms:

    a) Disclaiming warranty or limiting liability differently from the
    terms of sections 15 and 16 of this License; or

    b) Requiring preservation of specified reasonable legal notices or
    author attributions in that material or in the Appropriate Legal
    Notices displayed by works containing it; or

    c) Prohibiting misrepresentation of the origin of that material, or
    requiring that modified versions of such material be marked in
    reasonable ways as different from the original version; or

    d) Limiting the use for publicity purposes of names of licensors or
    authors of the material; or

    e) Declining to grant rights under trademark law for use of some
    trade names, trademarks, or service marks; or

    f) Requiring indemnification of licensors and authors of that
    material by anyone who conveys the material (or modified versions of
    it) with contractual assumptions of liability to the recipient, for
    any liability that these contractual assumptions directly impose on
    those licensors and authors.

  All other non-permissive additional terms are considered "further
restrictions" within the meaning of section 10.  If the Program as you
received it, or any part of it, contains a notice stating that it is
governed by this License along with a term that is a further
restriction, you may remove that term.  If a license document contains
a further restriction but permits relicensing or conveying under this
License, you may add to a covered work material governed by the terms
of that license document, provided that the further restriction does
not survive such relicensing or conveying.

  If you add terms to a covered work in accord with this section, you
must place, in the relevant source files, a statement of the
additional terms that apply to those files, or a notice indicating
where to find the applicable terms.

  Additional terms, permissive or non-permissive, may be stated in the
form of a separately written license, or stated as exceptions;
the above requirements apply either way.

  8. Termination.

  You may not propagate or modify a covered work except as expressly
provided under this License.  Any attempt otherwise to propagate or
modify it is void, and will automatically terminate your rights under
this License (including any patent licenses granted under the third
paragraph of section 11).

  However, if you cease all violation of this License, then your
license from a particular copyright holder is reinstated (a)
provisionally, unless and until the copyright holder explicitly and
finally terminates your license, and (b) permanently, if the copyright
holder fails to notify you of the violation by some reasonable means
prior to 60 days after the cessation.

  Moreover, your license from a particular copyright holder is
reinstated permanently if the copyright holder notifies you of the
violation by some reasonable means, this is the first time you have
received notice of violation of this License (for any work) from that
copyright holder, and you cure the violation prior to 30 days after
your receipt of the notice.

  Termination of your rights under this section does not terminate the
licenses of parties who have received copies or rights from you under
this License.  If your rights have been terminated and not permanently
reinstated, you do not qualify to receive new licenses for the same
material under section 10.

  9. Acceptance Not Required for Having Copies.

  You are not required to accept this License in order to receive or
run a copy of the Program.  Ancillary propagation of a covered work
occurring solely as a consequence of using peer-to-peer transmission
to receive a copy likewise does not require acceptance.  However,
nothing other than this License grants you permission to propagate or
modify any covered work.  These actions infringe copyright if you do
not accept this License.  Therefore, by modifying or propagating a
covered work, you indicate your acceptance of this License to do so.

  10. Automatic Licensing of Downstream Recipients.

  Each time you convey a covered work, the recipient automatically
receives a license from the original licensors, to run, modify and
propagate that work, subject to this License.  You are not responsible
for enforcing compliance by third parties with this License.

  An "entity transaction" is a transaction transferring control of an
organization, or substantially all assets of one, or subdividing an
organization, or merging organizations.  If propagation of a covered
work results from an entity transaction, each party to that
transaction who receives a copy of the work also receives whatever
licenses to the work the party's predecessor in interest had or could
give under the previous paragraph, plus a right to possession of the
Corresponding Source of the work from the predecessor in interest, if
the predecessor has it or can get it with reasonable efforts.

  You may not impose any further restrictions on the exercise of the
rights granted or affirmed under this License.  For example, you may
not impose a license fee, royalty, or other charge for exercise of
rights granted under this License, and you may not initiate litigation
(including a cross-claim or counterclaim in a lawsuit) alleging that
any patent claim is infringed by making, using, selling, offering for
sale, or importing the Program or any portion of it.

  11. Patents.

  A "contributor" is a copyright holder who authorizes use under this
License of the Program or a work on which the Program is based.  The
work thus licensed is called the contributor's "contributor version".

  A contributor's "essential patent claims" are all patent claims
owned or controlled by the contributor, whether already acquired or
hereafter acquired, that would be infringed by some manner, permitted
by this License, of making, using, or selling its contributor version,
but do not include claims that would be infringed only as a
consequence of further modification of the contributor version.  For
purposes of this definition, "control" includes the right to grant
patent sublicenses in a manner consistent with the requirements of
this License.

  Each contributor grants you a non-exclusive, worldwide, royalty-free
patent license under the contributor's essential patent claims, to
make, use, sell, offer for sale, import and otherwise run, modify and
propagate the contents of its contributor version.

  In the following three paragraphs, a "patent license" is any express
agreement or commitment, however denominated, not to enforce a patent
(such as an express permission to practice a patent or covenant not to
sue for patent infringement).  To "grant" such a patent license to a
party means to make such an agreement or commitment not to enforce a
patent against the party.

  If you convey a covered work, knowingly relying on a patent license,
and the Corresponding Source of the work is not available for anyone
to copy, free of charge and under the terms of this License, through a
publicly available network server or other readily accessible means,
then you must either (1) cause the Corresponding Source to be so
available, or (2) arrange to deprive yourself of the benefit of the
patent license for this particular work, or (3) arrange, in a manner
consistent with the requirements of this License, to extend the patent
license to downstream recipients.  "Knowingly relying" means you have
actual knowledge that, but for the patent license, your conveying the
covered work in a country, or your recipient's use of the covered work
in a country, would infringe one or more identifiable patents in that
country that you have reason to believe are valid.

  If, pursuant to or in connection with a single transaction or
arrangement, you convey, or propagate by procuring conveyance of, a
covered work, and grant a patent license to some of the parties
receiving the covered work authorizing them to use, propagate, modify
or convey a specific copy of the covered work, then the patent license
you grant is automatically extended to all recipients of the covered
work and works based on it.

  A patent license is "discriminatory" if it does not include within
the scope of its coverage, prohibits the exercise of, or is
conditioned on the non-exercise of one or more of the rights that are
specifically granted under this License.  You may not convey a covered
work if you are a party to an arrangement with a third party that is
in the business of distributing software, under which you make payment
to the third party based on the extent of your activity of conveying
the work, and under which the third party grants, to any of the
parties who would receive the covered work from you, a discriminatory
patent license (a) in connection with copies of the covered work
conveyed by you (or copies made from those copies), or (b) primarily
for and in connection with specific products or compilations that
contain the covered work, unless you entered into that arrangement,
or that patent license was granted, prior to 28 March 2007.

  Nothing in this License shall be construed as excluding or limiting
any implied license or other defenses to infringement that may
otherwise be available to you under applicable patent law.

  12. No Surrender of Others' Freedom.

  If conditions are imposed on you (whether by court order, agreement or
otherwise) that contradict the conditions of this License, they do not
excuse you from the conditions of this License.  If you cannot convey a
covered work so as to satisfy simultaneously your obligations under this
License and any other pertinent obligations, then as a consequence you may
not convey it at all.  For example, if you agree to terms that obligate you
to collect a royalty for further conveying from those to whom you convey
the Program, the only way you could satisfy both those terms and this
License would be to refrain entirely from conveying the Program.

  13. Use with the GNU Affero General Public License.

  Notwithstanding any other provision of this License, you have
permission to link or combine any covered work with a work licensed
under version 3 of the GNU Affero General Public License into a single
combined work, and to convey the resulting work.  The terms of this
License will continue to apply to the part which is the covered work,
but the special requirements of the GNU Affero General Public License,
section 13, concerning interaction through a network will apply to the
combination as such.

  14. Revised Versions of this License.

  The Free Software Foundation may publish revised and/or new versions of
the GNU General Public License from time to time.  Such new versions will
be similar in spirit to the present version, but may differ in detail to
address new problems or concerns.

  Each version is given a distinguishing version number.  If the
Program specifies that a certain numbered version of the GNU General
Public License "or any later version" applies to it, you have the
option of following the terms and conditions either of that numbered
version or of any later version published by the Free Software
Foundation.  If the Program does not specify a version number of the
GNU General Public License, you may choose any version ever published
by the Free Software Foundation.

  If the Program specifies that a proxy can decide which future
versions of the GNU General Public License can be used, that proxy's
public statement of acceptance of a version permanently authorizes you
to choose that version for the Program.

  Later license versions may give you additional or different
permissions.  However, no additional obligations are imposed on any
author or copyright holder as a result of your choosing to follow a
later version.

  15. Disclaimer of Warranty.

  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

  16. Limitation of Liability.

  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
SUCH DAMAGES.

  17. Interpretation of Sections 15 and 16.

  If the disclaimer of warranty and limitation of liability provided
above cannot be given local legal effect according to their terms,
reviewing courts shall apply local law that most closely approximates
an absolute waiver of all civil liability in connection with the
Program, unless a warranty or assumption of liability accompanies a
copy of the Program in return for a fee.

                     END OF TERMS AND CONDITIONS

            How to Apply These Terms to Your New Programs

  If you develop a new program, and you want it to be of the greatest
possible use to the public, the best way to achieve this is to make it
free software which everyone can redistribute and change under these terms.

  To do so, attach the following notices to the program.  It is safest
to attach them to the start of each source file to most effectively
state the exclusion of warranty; and each file should have at least
the "copyright" line and a pointer to where the full notice is found.

    <one line to give the program's name and a brief idea of what it does.>
    Copyright (C) <year>  <name of author>

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.

Also add information on how to contact you by electronic and paper mail.

  If the program does terminal interaction, make it output a short
notice like this when it starts in an interactive mode:

    <program>  Copyright (C) <year>  <name of author>
    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
    This is free software, and you are welcome to redistribute it
    under certain conditions; type `show c' for details.

The hypothetical commands `show w' and `show c' should show the appropriate
parts of the General Public License.  Of course, your program's commands
might be different; for a GUI interface, you would use an "about box".

  You should also get your employer (if you work as a programmer) or school,
if any, to sign a "copyright disclaimer" for the program, if necessary.
For more information on this, and how to apply and follow the GNU GPL, see
<https://www.gnu.org/licenses/>.

  The GNU General Public License does not permit incorporating your program
into proprietary programs.  If your program is a subroutine library, you
may consider it more useful to permit linking proprietary applications with
the library.  If this is what you want to do, use the GNU Lesser General
Public License instead of this License.  But first, please read
<https://www.gnu.org/licenses/why-not-lgpl.html>.
</pre>
</details>

<details>
<summary>Mozilla Public License 2.0 (MPL-2.0)</summary>
<p>Permissions of this weak copyleft license are conditioned on making available source code of licensed files and modifications of those files under the same license (or in certain cases, one of the GNU licenses). Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. However, a larger work using the licensed work may be distributed under different terms and without source code for files added in the larger work.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Patent use</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>Mozilla Public License Version 2.0
==================================

1. Definitions
--------------

1.1. "Contributor"
    means each individual or legal entity that creates, contributes to
    the creation of, or owns Covered Software.

1.2. "Contributor Version"
    means the combination of the Contributions of others (if any) used
    by a Contributor and that particular Contributor's Contribution.

1.3. "Contribution"
    means Covered Software of a particular Contributor.

1.4. "Covered Software"
    means Source Code Form to which the initial Contributor has attached
    the notice in Exhibit A, the Executable Form of such Source Code
    Form, and Modifications of such Source Code Form, in each case
    including portions thereof.

1.5. "Incompatible With Secondary Licenses"
    means

    (a) that the initial Contributor has attached the notice described
        in Exhibit B to the Covered Software; or

    (b) that the Covered Software was made available under the terms of
        version 1.1 or earlier of the License, but not also under the
        terms of a Secondary License.

1.6. "Executable Form"
    means any form of the work other than Source Code Form.

1.7. "Larger Work"
    means a work that combines Covered Software with other material, in
    a separate file or files, that is not Covered Software.

1.8. "License"
    means this document.

1.9. "Licensable"
    means having the right to grant, to the maximum extent possible,
    whether at the time of the initial grant or subsequently, any and
    all of the rights conveyed by this License.

1.10. "Modifications"
    means any of the following:

    (a) any file in Source Code Form that results from an addition to,
        deletion from, or modification of the contents of Covered
        Software; or

    (b) any new file in Source Code Form that contains any Covered
        Software.

1.11. "Patent Claims" of a Contributor
    means any patent claim(s), including without limitation, method,
    process, and apparatus claims, in any patent Licensable by such
    Contributor that would be infringed, but for the grant of the
    License, by the making, using, selling, offering for sale, having
    made, import, or transfer of either its Contributions or its
    Contributor Version.

1.12. "Secondary License"
    means either the GNU General Public License, Version 2.0, the GNU
    Lesser General Public License, Version 2.1, the GNU Affero General
    Public License, Version 3.0, or any later versions of those
    licenses.

1.13. "Source Code Form"
    means the form of the work preferred for making modifications.

1.14. "You" (or "Your")
    means an individual or a legal entity exercising rights under this
    License. For legal entities, "You" includes any entity that
    controls, is controlled by, or is under common control with You. For
    purposes of this definition, "control" means (a) the power, direct
    or indirect, to cause the direction or management of such entity,
    whether by contract or otherwise, or (b) ownership of more than
    fifty percent (50%) of the outstanding shares or beneficial
    ownership of such entity.

2. License Grants and Conditions
--------------------------------

2.1. Grants

Each Contributor hereby grants You a world-wide, royalty-free,
non-exclusive license:

(a) under intellectual property rights (other than patent or trademark)
    Licensable by such Contributor to use, reproduce, make available,
    modify, display, perform, distribute, and otherwise exploit its
    Contributions, either on an unmodified basis, with Modifications, or
    as part of a Larger Work; and

(b) under Patent Claims of such Contributor to make, use, sell, offer
    for sale, have made, import, and otherwise transfer either its
    Contributions or its Contributor Version.

2.2. Effective Date

The licenses granted in Section 2.1 with respect to any Contribution
become effective for each Contribution on the date the Contributor first
distributes such Contribution.

2.3. Limitations on Grant Scope

The licenses granted in this Section 2 are the only rights granted under
this License. No additional rights or licenses will be implied from the
distribution or licensing of Covered Software under this License.
Notwithstanding Section 2.1(b) above, no patent license is granted by a
Contributor:

(a) for any code that a Contributor has removed from Covered Software;
    or

(b) for infringements caused by: (i) Your and any other third party's
    modifications of Covered Software, or (ii) the combination of its
    Contributions with other software (except as part of its Contributor
    Version); or

(c) under Patent Claims infringed by Covered Software in the absence of
    its Contributions.

This License does not grant any rights in the trademarks, service marks,
or logos of any Contributor (except as may be necessary to comply with
the notice requirements in Section 3.4).

2.4. Subsequent Licenses

No Contributor makes additional grants as a result of Your choice to
distribute the Covered Software under a subsequent version of this
License (see Section 10.2) or under the terms of a Secondary License (if
permitted under the terms of Section 3.3).

2.5. Representation

Each Contributor represents that the Contributor believes its
Contributions are its original creation(s) or it has sufficient rights
to grant the rights to its Contributions conveyed by this License.

2.6. Fair Use

This License is not intended to limit any rights You have under
applicable copyright doctrines of fair use, fair dealing, or other
equivalents.

2.7. Conditions

Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
in Section 2.1.

3. Responsibilities
-------------------

3.1. Distribution of Source Form

All distribution of Covered Software in Source Code Form, including any
Modifications that You create or to which You contribute, must be under
the terms of this License. You must inform recipients that the Source
Code Form of the Covered Software is governed by the terms of this
License, and how they can obtain a copy of this License. You may not
attempt to alter or restrict the recipients' rights in the Source Code
Form.

3.2. Distribution of Executable Form

If You distribute Covered Software in Executable Form then:

(a) such Covered Software must also be made available in Source Code
    Form, as described in Section 3.1, and You must inform recipients of
    the Executable Form how they can obtain a copy of such Source Code
    Form by reasonable means in a timely manner, at a charge no more
    than the cost of distribution to the recipient; and

(b) You may distribute such Executable Form under the terms of this
    License, or sublicense it under different terms, provided that the
    license for the Executable Form does not attempt to limit or alter
    the recipients' rights in the Source Code Form under this License.

3.3. Distribution of a Larger Work

You may create and distribute a Larger Work under terms of Your choice,
provided that You also comply with the requirements of this License for
the Covered Software. If the Larger Work is a combination of Covered
Software with a work governed by one or more Secondary Licenses, and the
Covered Software is not Incompatible With Secondary Licenses, this
License permits You to additionally distribute such Covered Software
under the terms of such Secondary License(s), so that the recipient of
the Larger Work may, at their option, further distribute the Covered
Software under the terms of either this License or such Secondary
License(s).

3.4. Notices

You may not remove or alter the substance of any license notices
(including copyright notices, patent notices, disclaimers of warranty,
or limitations of liability) contained within the Source Code Form of
the Covered Software, except that You may alter any license notices to
the extent required to remedy known factual inaccuracies.

3.5. Application of Additional Terms

You may choose to offer, and to charge a fee for, warranty, support,
indemnity or liability obligations to one or more recipients of Covered
Software. However, You may do so only on Your own behalf, and not on
behalf of any Contributor. You must make it absolutely clear that any
such warranty, support, indemnity, or liability obligation is offered by
You alone, and You hereby agree to indemnify every Contributor for any
liability incurred by such Contributor as a result of warranty, support,
indemnity or liability terms You offer. You may include additional
disclaimers of warranty and limitations of liability specific to any
jurisdiction.

4. Inability to Comply Due to Statute or Regulation
---------------------------------------------------

If it is impossible for You to comply with any of the terms of this
License with respect to some or all of the Covered Software due to
statute, judicial order, or regulation then You must: (a) comply with
the terms of this License to the maximum extent possible; and (b)
describe the limitations and the code they affect. Such description must
be placed in a text file included with all distributions of the Covered
Software under this License. Except to the extent prohibited by statute
or regulation, such description must be sufficiently detailed for a
recipient of ordinary skill to be able to understand it.

5. Termination
--------------

5.1. The rights granted under this License will terminate automatically
if You fail to comply with any of its terms. However, if You become
compliant, then the rights granted under this License from a particular
Contributor are reinstated (a) provisionally, unless and until such
Contributor explicitly and finally terminates Your grants, and (b) on an
ongoing basis, if such Contributor fails to notify You of the
non-compliance by some reasonable means prior to 60 days after You have
come back into compliance. Moreover, Your grants from a particular
Contributor are reinstated on an ongoing basis if such Contributor
notifies You of the non-compliance by some reasonable means, this is the
first time You have received notice of non-compliance with this License
from such Contributor, and You become compliant prior to 30 days after
Your receipt of the notice.

5.2. If You initiate litigation against any entity by asserting a patent
infringement claim (excluding declaratory judgment actions,
counter-claims, and cross-claims) alleging that a Contributor Version
directly or indirectly infringes any patent, then the rights granted to
You by any and all Contributors for the Covered Software under Section
2.1 of this License shall terminate.

5.3. In the event of termination under Sections 5.1 or 5.2 above, all
end user license agreements (excluding distributors and resellers) which
have been validly granted by You or Your distributors under this License
prior to termination shall survive termination.

************************************************************************
*                                                                      *
*  6. Disclaimer of Warranty                                           *
*  -------------------------                                           *
*                                                                      *
*  Covered Software is provided under this License on an "as is"       *
*  basis, without warranty of any kind, either expressed, implied, or  *
*  statutory, including, without limitation, warranties that the       *
*  Covered Software is free of defects, merchantable, fit for a        *
*  particular purpose or non-infringing. The entire risk as to the     *
*  quality and performance of the Covered Software is with You.        *
*  Should any Covered Software prove defective in any respect, You     *
*  (not any Contributor) assume the cost of any necessary servicing,   *
*  repair, or correction. This disclaimer of warranty constitutes an   *
*  essential part of this License. No use of any Covered Software is   *
*  authorized under this License except under this disclaimer.         *
*                                                                      *
************************************************************************

************************************************************************
*                                                                      *
*  7. Limitation of Liability                                          *
*  --------------------------                                          *
*                                                                      *
*  Under no circumstances and under no legal theory, whether tort      *
*  (including negligence), contract, or otherwise, shall any           *
*  Contributor, or anyone who distributes Covered Software as          *
*  permitted above, be liable to You for any direct, indirect,         *
*  special, incidental, or consequential damages of any character      *
*  including, without limitation, damages for lost profits, loss of    *
*  goodwill, work stoppage, computer failure or malfunction, or any    *
*  and all other commercial damages or losses, even if such party      *
*  shall have been informed of the possibility of such damages. This   *
*  limitation of liability shall not apply to liability for death or   *
*  personal injury resulting from such party's negligence to the       *
*  extent applicable law prohibits such limitation. Some               *
*  jurisdictions do not allow the exclusion or limitation of           *
*  incidental or consequential damages, so this exclusion and          *
*  limitation may not apply to You.                                    *
*                                                                      *
************************************************************************

8. Litigation
-------------

Any litigation relating to this License may be brought only in the
courts of a jurisdiction where the defendant maintains its principal
place of business and such litigation shall be governed by laws of that
jurisdiction, without reference to its conflict-of-law provisions.
Nothing in this Section shall prevent a party's ability to bring
cross-claims or counter-claims.

9. Miscellaneous
----------------

This License represents the complete agreement concerning the subject
matter hereof. If any provision of this License is held to be
unenforceable, such provision shall be reformed only to the extent
necessary to make it enforceable. Any law or regulation which provides
that the language of a contract shall be construed against the drafter
shall not be used to construe this License against a Contributor.

10. Versions of the License
---------------------------

10.1. New Versions

Mozilla Foundation is the license steward. Except as provided in Section
10.3, no one other than the license steward has the right to modify or
publish new versions of this License. Each version will be given a
distinguishing version number.

10.2. Effect of New Versions

You may distribute the Covered Software under the terms of the version
of the License under which You originally received the Covered Software,
or under the terms of any subsequent version published by the license
steward.

10.3. Modified Versions

If you create software not governed by this License, and you want to
create a new license for such software, you may create and use a
modified version of this License if you rename the license and remove
any references to the name of the license steward (except to note that
such modified license differs from this License).

10.4. Distributing Source Code Form that is Incompatible With Secondary
Licenses

If You choose to distribute Source Code Form that is Incompatible With
Secondary Licenses under the terms of this version of the License, the
notice described in Exhibit B of this License must be attached.

Exhibit A - Source Code Form License Notice
-------------------------------------------

  This Source Code Form is subject to the terms of the Mozilla Public
  License, v. 2.0. If a copy of the MPL was not distributed with this
  file, You can obtain one at http://mozilla.org/MPL/2.0/.

If it is not possible or desirable to put the notice in a particular
file, then You may include the notice in a location (such as a LICENSE
file in a relevant directory) where a recipient would be likely to look
for such a notice.

You may add additional accurate notices of copyright ownership.

Exhibit B - "Incompatible With Secondary Licenses" Notice
---------------------------------------------------------

  This Source Code Form is "Incompatible With Secondary Licenses", as
  defined by the Mozilla Public License, v. 2.0.
</pre>
</details>

<details>
<summary>Creative Commons Attribution 4.0 International (CC-BY-4.0)</summary>
<p>Permits almost any use subject to providing credit and license notice. Frequently used for media assets and educational materials. The most common license for Open Access scientific publications. Not recommended for software.</p>
<p>This license allows the following:
<ul><li>Commercial use</li>
<li>Modifications</li>
<li>Distribution</li>
<li>Private use</li></ul></p>
<p>The original license text is as follows:</p>
<pre>Attribution 4.0 International

=======================================================================

Creative Commons Corporation ("Creative Commons") is not a law firm and
does not provide legal services or legal advice. Distribution of
Creative Commons public licenses does not create a lawyer-client or
other relationship. Creative Commons makes its licenses and related
information available on an "as-is" basis. Creative Commons gives no
warranties regarding its licenses, any material licensed under their
terms and conditions, or any related information. Creative Commons
disclaims all liability for damages resulting from their use to the
fullest extent possible.

Using Creative Commons Public Licenses

Creative Commons public licenses provide a standard set of terms and
conditions that creators and other rights holders may use to share
original works of authorship and other material subject to copyright
and certain other rights specified in the public license below. The
following considerations are for informational purposes only, are not
exhaustive, and do not form part of our licenses.

     Considerations for licensors: Our public licenses are
     intended for use by those authorized to give the public
     permission to use material in ways otherwise restricted by
     copyright and certain other rights. Our licenses are
     irrevocable. Licensors should read and understand the terms
     and conditions of the license they choose before applying it.
     Licensors should also secure all rights necessary before
     applying our licenses so that the public can reuse the
     material as expected. Licensors should clearly mark any
     material not subject to the license. This includes other CC-
     licensed material, or material used under an exception or
     limitation to copyright. More considerations for licensors:
     wiki.creativecommons.org/Considerations_for_licensors

     Considerations for the public: By using one of our public
     licenses, a licensor grants the public permission to use the
     licensed material under specified terms and conditions. If
     the licensor's permission is not necessary for any reason--for
     example, because of any applicable exception or limitation to
     copyright--then that use is not regulated by the license. Our
     licenses grant only permissions under copyright and certain
     other rights that a licensor has authority to grant. Use of
     the licensed material may still be restricted for other
     reasons, including because others have copyright or other
     rights in the material. A licensor may make special requests,
     such as asking that all changes be marked or described.
     Although not required by our licenses, you are encouraged to
     respect those requests where reasonable. More considerations
     for the public:
     wiki.creativecommons.org/Considerations_for_licensees

=======================================================================

Creative Commons Attribution 4.0 International Public License

By exercising the Licensed Rights (defined below), You accept and agree
to be bound by the terms and conditions of this Creative Commons
Attribution 4.0 International Public License ("Public License"). To the
extent this Public License may be interpreted as a contract, You are
granted the Licensed Rights in consideration of Your acceptance of
these terms and conditions, and the Licensor grants You such rights in
consideration of benefits the Licensor receives from making the
Licensed Material available under these terms and conditions.


Section 1 -- Definitions.

  a. Adapted Material means material subject to Copyright and Similar
     Rights that is derived from or based upon the Licensed Material
     and in which the Licensed Material is translated, altered,
     arranged, transformed, or otherwise modified in a manner requiring
     permission under the Copyright and Similar Rights held by the
     Licensor. For purposes of this Public License, where the Licensed
     Material is a musical work, performance, or sound recording,
     Adapted Material is always produced where the Licensed Material is
     synched in timed relation with a moving image.

  b. Adapter's License means the license You apply to Your Copyright
     and Similar Rights in Your contributions to Adapted Material in
     accordance with the terms and conditions of this Public License.

  c. Copyright and Similar Rights means copyright and/or similar rights
     closely related to copyright including, without limitation,
     performance, broadcast, sound recording, and Sui Generis Database
     Rights, without regard to how the rights are labeled or
     categorized. For purposes of this Public License, the rights
     specified in Section 2(b)(1)-(2) are not Copyright and Similar
     Rights.

  d. Effective Technological Measures means those measures that, in the
     absence of proper authority, may not be circumvented under laws
     fulfilling obligations under Article 11 of the WIPO Copyright
     Treaty adopted on December 20, 1996, and/or similar international
     agreements.

  e. Exceptions and Limitations means fair use, fair dealing, and/or
     any other exception or limitation to Copyright and Similar Rights
     that applies to Your use of the Licensed Material.

  f. Licensed Material means the artistic or literary work, database,
     or other material to which the Licensor applied this Public
     License.

  g. Licensed Rights means the rights granted to You subject to the
     terms and conditions of this Public License, which are limited to
     all Copyright and Similar Rights that apply to Your use of the
     Licensed Material and that the Licensor has authority to license.

  h. Licensor means the individual(s) or entity(ies) granting rights
     under this Public License.

  i. Share means to provide material to the public by any means or
     process that requires permission under the Licensed Rights, such
     as reproduction, public display, public performance, distribution,
     dissemination, communication, or importation, and to make material
     available to the public including in ways that members of the
     public may access the material from a place and at a time
     individually chosen by them.

  j. Sui Generis Database Rights means rights other than copyright
     resulting from Directive 96/9/EC of the European Parliament and of
     the Council of 11 March 1996 on the legal protection of databases,
     as amended and/or succeeded, as well as other essentially
     equivalent rights anywhere in the world.

  k. You means the individual or entity exercising the Licensed Rights
     under this Public License. Your has a corresponding meaning.


Section 2 -- Scope.

  a. License grant.

       1. Subject to the terms and conditions of this Public License,
          the Licensor hereby grants You a worldwide, royalty-free,
          non-sublicensable, non-exclusive, irrevocable license to
          exercise the Licensed Rights in the Licensed Material to:

            a. reproduce and Share the Licensed Material, in whole or
               in part; and

            b. produce, reproduce, and Share Adapted Material.

       2. Exceptions and Limitations. For the avoidance of doubt, where
          Exceptions and Limitations apply to Your use, this Public
          License does not apply, and You do not need to comply with
          its terms and conditions.

       3. Term. The term of this Public License is specified in Section
          6(a).

       4. Media and formats; technical modifications allowed. The
          Licensor authorizes You to exercise the Licensed Rights in
          all media and formats whether now known or hereafter created,
          and to make technical modifications necessary to do so. The
          Licensor waives and/or agrees not to assert any right or
          authority to forbid You from making technical modifications
          necessary to exercise the Licensed Rights, including
          technical modifications necessary to circumvent Effective
          Technological Measures. For purposes of this Public License,
          simply making modifications authorized by this Section 2(a)
          (4) never produces Adapted Material.

       5. Downstream recipients.

            a. Offer from the Licensor -- Licensed Material. Every
               recipient of the Licensed Material automatically
               receives an offer from the Licensor to exercise the
               Licensed Rights under the terms and conditions of this
               Public License.

            b. No downstream restrictions. You may not offer or impose
               any additional or different terms or conditions on, or
               apply any Effective Technological Measures to, the
               Licensed Material if doing so restricts exercise of the
               Licensed Rights by any recipient of the Licensed
               Material.

       6. No endorsement. Nothing in this Public License constitutes or
          may be construed as permission to assert or imply that You
          are, or that Your use of the Licensed Material is, connected
          with, or sponsored, endorsed, or granted official status by,
          the Licensor or others designated to receive attribution as
          provided in Section 3(a)(1)(A)(i).

  b. Other rights.

       1. Moral rights, such as the right of integrity, are not
          licensed under this Public License, nor are publicity,
          privacy, and/or other similar personality rights; however, to
          the extent possible, the Licensor waives and/or agrees not to
          assert any such rights held by the Licensor to the limited
          extent necessary to allow You to exercise the Licensed
          Rights, but not otherwise.

       2. Patent and trademark rights are not licensed under this
          Public License.

       3. To the extent possible, the Licensor waives any right to
          collect royalties from You for the exercise of the Licensed
          Rights, whether directly or through a collecting society
          under any voluntary or waivable statutory or compulsory
          licensing scheme. In all other cases the Licensor expressly
          reserves any right to collect such royalties.


Section 3 -- License Conditions.

Your exercise of the Licensed Rights is expressly made subject to the
following conditions.

  a. Attribution.

       1. If You Share the Licensed Material (including in modified
          form), You must:

            a. retain the following if it is supplied by the Licensor
               with the Licensed Material:

                 i. identification of the creator(s) of the Licensed
                    Material and any others designated to receive
                    attribution, in any reasonable manner requested by
                    the Licensor (including by pseudonym if
                    designated);

                ii. a copyright notice;

               iii. a notice that refers to this Public License;

                iv. a notice that refers to the disclaimer of
                    warranties;

                 v. a URI or hyperlink to the Licensed Material to the
                    extent reasonably practicable;

            b. indicate if You modified the Licensed Material and
               retain an indication of any previous modifications; and

            c. indicate the Licensed Material is licensed under this
               Public License, and include the text of, or the URI or
               hyperlink to, this Public License.

       2. You may satisfy the conditions in Section 3(a)(1) in any
          reasonable manner based on the medium, means, and context in
          which You Share the Licensed Material. For example, it may be
          reasonable to satisfy the conditions by providing a URI or
          hyperlink to a resource that includes the required
          information.

       3. If requested by the Licensor, You must remove any of the
          information required by Section 3(a)(1)(A) to the extent
          reasonably practicable.

       4. If You Share Adapted Material You produce, the Adapter's
          License You apply must not prevent recipients of the Adapted
          Material from complying with this Public License.


Section 4 -- Sui Generis Database Rights.

Where the Licensed Rights include Sui Generis Database Rights that
apply to Your use of the Licensed Material:

  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
     to extract, reuse, reproduce, and Share all or a substantial
     portion of the contents of the database;

  b. if You include all or a substantial portion of the database
     contents in a database in which You have Sui Generis Database
     Rights, then the database in which You have Sui Generis Database
     Rights (but not its individual contents) is Adapted Material; and

  c. You must comply with the conditions in Section 3(a) if You Share
     all or a substantial portion of the contents of the database.

For the avoidance of doubt, this Section 4 supplements and does not
replace Your obligations under this Public License where the Licensed
Rights include other Copyright and Similar Rights.


Section 5 -- Disclaimer of Warranties and Limitation of Liability.

  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.

  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.

  c. The disclaimer of warranties and limitation of liability provided
     above shall be interpreted in a manner that, to the extent
     possible, most closely approximates an absolute disclaimer and
     waiver of all liability.


Section 6 -- Term and Termination.

  a. This Public License applies for the term of the Copyright and
     Similar Rights licensed here. However, if You fail to comply with
     this Public License, then Your rights under this Public License
     terminate automatically.

  b. Where Your right to use the Licensed Material has terminated under
     Section 6(a), it reinstates:

       1. automatically as of the date the violation is cured, provided
          it is cured within 30 days of Your discovery of the
          violation; or

       2. upon express reinstatement by the Licensor.

     For the avoidance of doubt, this Section 6(b) does not affect any
     right the Licensor may have to seek remedies for Your violations
     of this Public License.

  c. For the avoidance of doubt, the Licensor may also offer the
     Licensed Material under separate terms or conditions or stop
     distributing the Licensed Material at any time; however, doing so
     will not terminate this Public License.

  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
     License.


Section 7 -- Other Terms and Conditions.

  a. The Licensor shall not be bound by any additional or different
     terms or conditions communicated by You unless expressly agreed.

  b. Any arrangements, understandings, or agreements regarding the
     Licensed Material not stated herein are separate from and
     independent of the terms and conditions of this Public License.


Section 8 -- Interpretation.

  a. For the avoidance of doubt, this Public License does not, and
     shall not be interpreted to, reduce, limit, restrict, or impose
     conditions on any use of the Licensed Material that could lawfully
     be made without permission under this Public License.

  b. To the extent possible, if any provision of this Public License is
     deemed unenforceable, it shall be automatically reformed to the
     minimum extent necessary to make it enforceable. If the provision
     cannot be reformed, it shall be severed from this Public License
     without affecting the enforceability of the remaining terms and
     conditions.

  c. No term or condition of this Public License will be waived and no
     failure to comply consented to unless expressly agreed to by the
     Licensor.

  d. Nothing in this Public License constitutes or may be interpreted
     as a limitation upon, or waiver of, any privileges and immunities
     that apply to the Licensor or You, including from the legal
     processes of any jurisdiction or authority.


=======================================================================

Creative Commons is not a party to its public licenses.
Notwithstanding, Creative Commons may elect to apply one of its public
licenses to material it publishes and in those instances will be
considered the “Licensor.” The text of the Creative Commons public
licenses is dedicated to the public domain under the CC0 Public Domain
Dedication. Except for the limited purpose of indicating that material
is shared under a Creative Commons public license or as otherwise
permitted by the Creative Commons policies published at
creativecommons.org/policies, Creative Commons does not authorize the
use of the trademark "Creative Commons" or any other trademark or logo
of Creative Commons without its prior written consent including,
without limitation, in connection with any unauthorized modifications
to any of its public licenses or any other arrangements,
understandings, or agreements concerning use of licensed material. For
the avoidance of doubt, this paragraph does not form part of the public
licenses.

Creative Commons may be contacted at creativecommons.org.
</pre>
</details>



No information is held on the following licenses, please do your own research to dermine their suitability.

- BlueOak-1.0.0
- Python-2.0


### Full dependency list

Click the heading below to view a complete list of all third-party dependencies.

<details>
<summary>Module dependency list</summary>
<table><tr><th>Name</th><th>Version</th><th>License</th><th>Description</th></tr>
<tr><td><a href="https://github.com/taylortom/zipper" target="_blank">zipper</a></td><td>1.0.0</td><td>undefined</td><td>Module for zipping/unzipping files</tr>
<tr><td><a href="https://zengabor.github.io/zenscroll/" target="_blank">zenscroll</a></td><td>4.0.2</td><td>Unlicense</td><td>A module to smooth-scroll web pages and scrollable elements (like DIVs)</tr>
<tr><td>yocto-queue</td><td>1.1.1</td><td>MIT</td><td>Tiny queue data structure</tr>
<tr><td><a href="https://github.com/thejoshwolfe/yauzl" target="_blank">yauzl</a></td><td>2.10.0</td><td>MIT</td><td>yet another unzip library for node</tr>
<tr><td><a href="https://github.com/yargs/yargs-unparser" target="_blank">yargs-unparser</a></td><td>2.0.0</td><td>MIT</td><td>Converts back a yargs argv object to its original array form</tr>
<tr><td><a href="https://yargs.js.org/" target="_blank">yargs</a></td><td>15.4.1</td><td>MIT</td><td>yargs the modern, pirate-themed, successor to optimist.</tr>
<tr><td>yargs-parser</td><td>20.2.9</td><td>ISC</td><td>the mighty option parser used by yargs</tr>
<tr><td><a href="https://github.com/nexdrew/yargonaut#readme" target="_blank">yargonaut</a></td><td>1.1.4</td><td>Apache-2.0</td><td>Decorate yargs content with chalk styles and figlet fonts</tr>
<tr><td>yallist</td><td>3.1.1</td><td>ISC</td><td>Yet Another Linked List</tr>
<tr><td><a href="https://github.com/yargs/y18n" target="_blank">y18n</a></td><td>4.0.3</td><td>ISC</td><td>the bare-bones internationalization library used by yargs</tr>
<tr><td><a href="https://github.com/Raynos/xtend" target="_blank">xtend</a></td><td>4.0.2</td><td>MIT</td><td>extend like a boss</tr>
<tr><td><a href="https://github.com/leizongmin/js-xss" target="_blank">xss</a></td><td>1.0.15</td><td>MIT</td><td>Sanitize untrusted HTML (to prevent XSS) with a configuration specified by a Whitelist</tr>
<tr><td>xmlcreate</td><td>2.0.4</td><td>Apache-2.0</td><td>Simple XML builder for Node.js</tr>
<tr><td><a href="http://github.com/dylang/node-xml" target="_blank">xml</a></td><td>1.0.1</td><td>MIT</td><td>Fast and simple xml generator. Supports attributes, CDATA, etc. Includes tests and examples.</tr>
<tr><td>xml-but-prettier</td><td>1.0.1</td><td>MIT</td><td>Beautifies XML documents by putting each tag and text node on their own line and correctly indents everything</tr>
<tr><td>xdg-basedir</td><td>4.0.0</td><td>MIT</td><td>Get XDG Base Directory paths</tr>
<tr><td><a href="https://github.com/websockets/ws" target="_blank">ws</a></td><td>7.5.10</td><td>MIT</td><td>Simple to use, blazing fast and thoroughly tested websocket client and server for Node.js</tr>
<tr><td><a href="https://github.com/npm/write-file-atomic" target="_blank">write-file-atomic</a></td><td>3.0.3</td><td>ISC</td><td>Write files in an atomic fashion w/configurable ownership</tr>
<tr><td><a href="https://github.com/npm/wrappy" target="_blank">wrappy</a></td><td>1.0.2</td><td>ISC</td><td>Callback wrapping utility</tr>
<tr><td>wrap-ansi</td><td>7.0.0</td><td>MIT</td><td>Wordwrap a string with ANSI escape codes</tr>
<tr><td>wrap-ansi</td><td>8.1.0</td><td>MIT</td><td>Wordwrap a string with ANSI escape codes</tr>
<tr><td><a href="https://github.com/josdejong/workerpool" target="_blank">workerpool</a></td><td>6.5.1</td><td>Apache-2.0</td><td>Offload tasks to a pool of workers on node.js and in the browser</tr>
<tr><td>wordwrap</td><td>1.0.0</td><td>MIT</td><td>Wrap those words. Show them at what columns to start and stop.</tr>
<tr><td><a href="https://github.com/jonschlinkert/word-wrap" target="_blank">word-wrap</a></td><td>1.2.5</td><td>MIT</td><td>Wrap words to a specified length.</tr>
<tr><td>widest-line</td><td>3.1.0</td><td>MIT</td><td>Get the visual width of the widest line in a string - the number of columns required to display it</tr>
<tr><td><a href="https://github.com/nexdrew/which-module#readme" target="_blank">which-module</a></td><td>2.0.1</td><td>ISC</td><td>Find the module object for something that was require()d</tr>
<tr><td><a href="https://github.com/inspect-js/which-collection#readme" target="_blank">which-collection</a></td><td>1.0.2</td><td>MIT</td><td>Which kind of Collection (Map, Set, WeakMap, WeakSet) is this JavaScript value? Works cross-realm, without `instanceof`, and despite Symbol.toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/which-boxed-primitive#readme" target="_blank">which-boxed-primitive</a></td><td>1.0.2</td><td>MIT</td><td>Which kind of boxed JS primitive is this?</tr>
<tr><td><a href="https://github.com/inspect-js/which-builtin-type#readme" target="_blank">which-builtin-type</a></td><td>1.1.4</td><td>MIT</td><td>What is the type of this builtin JS value?</tr>
<tr><td>whatwg-url</td><td>13.0.0</td><td>MIT</td><td>An implementation of the WHATWG URL Standard's URL API and parsing machinery</tr>
<tr><td>which</td><td>2.0.2</td><td>ISC</td><td>Like which(1) unix command. Find the first instance of an executable in the PATH.</tr>
<tr><td>whatwg-encoding</td><td>2.0.0</td><td>MIT</td><td>Decode strings according to the WHATWG Encoding Standard</tr>
<tr><td>which-typed-array</td><td>1.1.15</td><td>MIT</td><td>Which kind of Typed Array is this JavaScript value? Works cross-realm, without `instanceof`, and despite Symbol.toStringTag.</tr>
<tr><td>webidl-conversions</td><td>7.0.0</td><td>BSD-2-Clause</td><td>Implements the WebIDL algorithms for converting to and from JavaScript values</tr>
<tr><td><a href="https://github.com/tree-sitter/tree-sitter/tree/master/lib/binding_web" target="_blank">web-tree-sitter</a></td><td>0.20.3</td><td>MIT</td><td>Tree-sitter bindings for the web</tr>
<tr><td><a href="https://git.coolaj86.com/coolaj86/fs-walk.js" target="_blank">walk</a></td><td>2.3.15</td><td>(MIT OR Apache-2.0)</td><td>A node port of python's os.walk</tr>
<tr><td><a href="https://github.com/MattiasBuelens/web-streams-polyfill#readme" target="_blank">web-streams-polyfill</a></td><td>3.3.3</td><td>MIT</td><td>Web Streams, based on the WHATWG spec reference implementation</tr>
<tr><td><a href="http://github.com/voxpelli/version-guard" target="_blank">version-guard</a></td><td>1.1.3</td><td>0BSD</td><td>Used to ensure modern CLI scripts fail silently on old js versions. Useful for static analysis tools and similar</tr>
<tr><td>vary</td><td>1.1.2</td><td>MIT</td><td>Manipulate the HTTP Vary header</tr>
<tr><td>uuid</td><td>8.3.2</td><td>MIT</td><td>RFC4122 (v1, v4, and v5) UUIDs</tr>
<tr><td>utils-merge</td><td>1.0.1</td><td>MIT</td><td>merge() utility function</tr>
<tr><td><a href="https://github.com/TooTallNate/util-deprecate" target="_blank">util-deprecate</a></td><td>1.0.2</td><td>MIT</td><td>The Node.js `util.deprecate()` function with browser support</tr>
<tr><td>use-sync-external-store</td><td>1.2.2</td><td>MIT</td><td>Backwards compatible shim for React's useSyncExternalStore. Works with any React that supports hooks.</tr>
<tr><td>url-to-options</td><td>1.0.1</td><td>MIT</td><td>Convert a WHATWG URL to an http(s).request options object.</tr>
<tr><td>url-join</td><td>4.0.1</td><td>MIT</td><td>Join urls and normalize as in path.join.</tr>
<tr><td>url-parse</td><td>1.5.10</td><td>MIT</td><td>Small footprint URL parser that works seamlessly across Node.js and browser environments</tr>
<tr><td>url-parse-lax</td><td>3.0.0</td><td>MIT</td><td>Lax url.parse() with support for protocol-less URLs & IPs</tr>
<tr><td><a href="https://github.com/garycourt/uri-js" target="_blank">uri-js</a></td><td>4.4.1</td><td>BSD-2-Clause</td><td>An RFC 3986/3987 compliant, scheme extendable URI/IRI parsing/validating/resolving library for JavaScript.</tr>
<tr><td>update-notifier</td><td>4.1.3</td><td>BSD-2-Clause</td><td>Update notifications for your CLI app</tr>
<tr><td>update-browserslist-db</td><td>1.1.1</td><td>MIT</td><td>CLI tool to update caniuse-lite to refresh target browsers from Browserslist config</tr>
<tr><td><a href="http://github.com/anodynos/upath/" target="_blank">upath</a></td><td>2.0.1</td><td>MIT</td><td>A proxy to `path`, replacing `\` with `/` for all results (supports UNC paths) & new methods to normalize & join keeping leading `./` and add, change, default, trim file extensions.</tr>
<tr><td>unraw</td><td>3.0.0</td><td>MIT</td><td>Convert raw escape sequences to their respective characters (undo String.raw).</tr>
<tr><td><a href="https://github.com/RyanZim/universalify#readme" target="_blank">universalify</a></td><td>2.0.1</td><td>MIT</td><td>Make a callback- or promise-based function support both promises and callbacks.</tr>
<tr><td>unpipe</td><td>1.0.0</td><td>MIT</td><td>Unpipe a stream from all destinations</tr>
<tr><td>unique-string</td><td>2.0.0</td><td>MIT</td><td>Generate a unique random string</tr>
<tr><td>union</td><td>0.5.0</td><td>undefined</td><td>A hybrid buffered / streaming middleware kernel backwards compatible with connect.</tr>
<tr><td><a href="https://github.com/mathiasbynens/unicode-property-aliases-ecmascript" target="_blank">unicode-property-aliases-ecmascript</a></td><td>2.1.0</td><td>MIT</td><td>Unicode property alias mappings in JavaScript format for property names that are supported in ECMAScript RegExp property escapes.</tr>
<tr><td><a href="https://github.com/mathiasbynens/unicode-match-property-value-ecmascript" target="_blank">unicode-match-property-value-ecmascript</a></td><td>2.2.0</td><td>MIT</td><td>Match a Unicode property or property alias to its canonical property name per the algorithm used for RegExp Unicode property escapes in ECMAScript.</tr>
<tr><td><a href="https://github.com/mathiasbynens/unicode-match-property-ecmascript" target="_blank">unicode-match-property-ecmascript</a></td><td>2.0.0</td><td>MIT</td><td>Match a Unicode property or property alias to its canonical property name per the algorithm used for RegExp Unicode property escapes in ECMAScript.</tr>
<tr><td><a href="https://underscorejs.org" target="_blank">underscore</a></td><td>1.13.7</td><td>MIT</td><td>JavaScript's functional programming helper library.</tr>
<tr><td><a href="https://github.com/mathiasbynens/unicode-canonical-property-names-ecmascript" target="_blank">unicode-canonical-property-names-ecmascript</a></td><td>2.0.1</td><td>MIT</td><td>The set of canonical Unicode property names supported in ECMAScript RegExp property escapes.</tr>
<tr><td><a href="https://github.com/ljharb/unbox-primitive#readme" target="_blank">unbox-primitive</a></td><td>1.0.2</td><td>MIT</td><td>Unbox a boxed JS primitive value.</tr>
<tr><td>uid-safe</td><td>2.1.5</td><td>MIT</td><td>URL and cookie safe UIDs</tr>
<tr><td>unbzip2-stream</td><td>1.4.3</td><td>MIT</td><td>streaming unbzip2 implementation in pure javascript for node and browsers</tr>
<tr><td>uglify-js</td><td>3.19.3</td><td>BSD-2-Clause</td><td>JavaScript parser, mangler/compressor and beautifier toolkit</tr>
<tr><td>uc.micro</td><td>2.1.0</td><td>MIT</td><td>Micro subset of unicode data files for markdown-it projects.</tr>
<tr><td>types-ramda</td><td>0.30.1</td><td>MIT</td><td>Dedicated types library for ramda</tr>
<tr><td><a href="http://feross.org" target="_blank">typedarray-to-buffer</a></td><td>3.1.5</td><td>MIT</td><td>Convert a typed array to a Buffer without a copy</tr>
<tr><td><a href="https://github.com/substack/typedarray" target="_blank">typedarray</a></td><td>0.0.6</td><td>MIT</td><td>TypedArray polyfill for old browsers</tr>
<tr><td><a href="https://github.com/inspect-js/typed-array-length#readme" target="_blank">typed-array-length</a></td><td>1.0.6</td><td>MIT</td><td>Robustly get the length of a Typed Array</tr>
<tr><td><a href="https://github.com/ljharb/typed-array-buffer#readme" target="_blank">typed-array-buffer</a></td><td>1.0.2</td><td>MIT</td><td>Get the ArrayBuffer out of a TypedArray, robustly.</tr>
<tr><td><a href="https://github.com/inspect-js/typed-array-byte-offset#readme" target="_blank">typed-array-byte-offset</a></td><td>1.0.2</td><td>MIT</td><td>Robustly get the byte offset of a Typed Array</tr>
<tr><td><a href="https://github.com/inspect-js/typed-array-byte-length#readme" target="_blank">typed-array-byte-length</a></td><td>1.0.1</td><td>MIT</td><td>Robustly get the byte length of a Typed Array</tr>
<tr><td>type-is</td><td>1.6.18</td><td>MIT</td><td>Infer the content-type of a request.</tr>
<tr><td>type-fest</td><td>0.21.3</td><td>(MIT OR CC0-1.0)</td><td>A collection of essential TypeScript types</tr>
<tr><td><a href="https://github.com/gkz/type-check" target="_blank">type-check</a></td><td>0.4.0</td><td>MIT</td><td>type-check allows you to check the types of JavaScript values at runtime with a Haskell like type syntax.</tr>
<tr><td>tweezer.js</td><td>1.5.0</td><td>MIT</td><td>A small, dependency-free, ES6 tweening library for smooth animations</tr>
<tr><td>tunnel-agent</td><td>0.6.0</td><td>Apache-2.0</td><td>HTTP proxy tunneling agent. Formerly part of mikeal/request, now a standalone module.</tr>
<tr><td><a href="https://www.typescriptlang.org/" target="_blank">tslib</a></td><td>2.7.0</td><td>0BSD</td><td>Runtime library for TypeScript helper functions</tr>
<tr><td><a href="https://github.com/millsp/ts-toolbelt" target="_blank">ts-toolbelt</a></td><td>9.6.0</td><td>Apache-2.0</td><td>TypeScript's largest utility library</tr>
<tr><td>tsconfig-paths</td><td>3.15.0</td><td>MIT</td><td>Load node modules according to tsconfig paths, in run-time or via API.</tr>
<tr><td><a href="https://github.com/tannerntannern/ts-mixer#readme" target="_blank">ts-mixer</a></td><td>6.0.4</td><td>MIT</td><td>A very small TypeScript library that provides tolerable Mixin functionality.</tr>
<tr><td>trim-repeated</td><td>1.0.0</td><td>MIT</td><td>Trim a consecutively repeated substring: foo--bar---baz → foo-bar-baz</tr>
<tr><td><a href="https://github.com/ikatyang/tree-sitter-yaml#readme" target="_blank">tree-sitter-yaml</a></td><td>0.5.0</td><td>MIT</td><td>YAML grammar for tree-sitter</tr>
<tr><td>tree-sitter-json</td><td>0.20.2</td><td>MIT</td><td>JSON grammar for tree-sitter</tr>
<tr><td>tree-sitter</td><td>0.20.4</td><td>MIT</td><td>Incremental parsers for node</tr>
<tr><td>tr46</td><td>4.1.1</td><td>MIT</td><td>An implementation of the Unicode UTS #46: Unicode IDNA Compatibility Processing</tr>
<tr><td>token-types</td><td>5.0.1</td><td>MIT</td><td>Common token types for decoding and encoding numeric and string values</tr>
<tr><td>toidentifier</td><td>1.0.1</td><td>MIT</td><td>Convert a string of words to a JavaScript identifier</tr>
<tr><td>toggle-selection</td><td>1.0.6</td><td>MIT</td><td>Toggle current selected content in browser</tr>
<tr><td><a href="https://github.com/micromatch/to-regex-range" target="_blank">to-regex-range</a></td><td>5.0.1</td><td>MIT</td><td>Pass two numbers, get a regex-compatible source string for matching ranges. Validated against more than 2.78 million test assertions.</tr>
<tr><td>to-readable-stream</td><td>1.0.0</td><td>MIT</td><td>Convert a string/Buffer/Uint8Array to a readable stream</tr>
<tr><td>to-fast-properties</td><td>2.0.0</td><td>MIT</td><td>Force V8 to use fast properties for an object</tr>
<tr><td><a href="https://github.com/mafintosh/to-buffer" target="_blank">to-buffer</a></td><td>1.1.1</td><td>MIT</td><td>Pass in a string, get a buffer back. Pass in a buffer, get the same buffer back</tr>
<tr><td><a href="http://github.com/raszi/node-tmp" target="_blank">tmp</a></td><td>0.0.33</td><td>MIT</td><td>Temporary file and directory creator</tr>
<tr><td>tinydate</td><td>1.3.0</td><td>MIT</td><td>A tiny (349B) reusable date formatter. Extremely fast!</tr>
<tr><td>timed-out</td><td>4.0.1</td><td>MIT</td><td>Emit `ETIMEDOUT` or `ESOCKETTIMEDOUT` when ClientRequest is hanged</tr>
<tr><td><a href="https://github.com/dominictarr/through" target="_blank">through</a></td><td>2.3.8</td><td>MIT</td><td>simplified stream construction</tr>
<tr><td><a href="https://github.com/substack/text-table" target="_blank">text-table</a></td><td>0.2.0</td><td>MIT</td><td>borderless text tables with alignment</tr>
<tr><td>term-size</td><td>2.2.1</td><td>MIT</td><td>Reliably get the terminal window size (columns & rows)</tr>
<tr><td><a href="https://github.com/mafintosh/tar-stream" target="_blank">tar-stream</a></td><td>1.6.2</td><td>MIT</td><td>tar-stream is a streaming tar parser and generator and nothing else. It is streams2 and operates purely using streams which means you can easily extract/parse tarballs without ever hitting the file system.</tr>
<tr><td><a href="https://github.com/mafintosh/tar-fs" target="_blank">tar-fs</a></td><td>2.1.1</td><td>MIT</td><td>filesystem bindings for tar-stream</tr>
<tr><td><a href="https://github.com/swagger-api/swagger-ui" target="_blank">swagger-ui</a></td><td>5.17.14</td><td>Apache-2.0</td><td>undefined</tr>
<tr><td>swagger-client</td><td>3.29.3</td><td>Apache-2.0</td><td>SwaggerJS - a collection of interfaces for OAI specs</tr>
<tr><td><a href="https://github.com/inspect-js/node-supports-preserve-symlinks-flag#readme" target="_blank">supports-preserve-symlinks-flag</a></td><td>1.0.0</td><td>MIT</td><td>Determine if the current node version supports the `--preserve-symlinks` flag.</tr>
<tr><td>supports-color</td><td>7.2.0</td><td>MIT</td><td>Detect whether a terminal supports color</tr>
<tr><td>supertest</td><td>4.0.2</td><td>MIT</td><td>SuperAgent driven library for testing HTTP servers</tr>
<tr><td>superagent</td><td>3.8.3</td><td>MIT</td><td>elegant & feature rich browser / node HTTP with a fluent API</tr>
<tr><td>strtok3</td><td>7.1.1</td><td>MIT</td><td>A promise based streaming tokenizer</tr>
<tr><td>strnum</td><td>1.0.5</td><td>MIT</td><td>Parse String to Number based on configuration</tr>
<tr><td>strip-outer</td><td>1.0.1</td><td>MIT</td><td>Strip a substring from the start/end of a string</tr>
<tr><td>strip-json-comments</td><td>3.1.1</td><td>MIT</td><td>Strip comments from JSON. Lets you use comments in your JSON files!</tr>
<tr><td>strip-indent</td><td>3.0.0</td><td>MIT</td><td>Strip leading whitespace from each line in a string</tr>
<tr><td>strip-dirs</td><td>2.1.0</td><td>MIT</td><td>Remove leading directory components from a path, like tar's --strip-components option</tr>
<tr><td>strip-ansi</td><td>6.0.1</td><td>MIT</td><td>Strip ANSI escape codes from a string</tr>
<tr><td>strip-ansi</td><td>6.0.1</td><td>MIT</td><td>Strip ANSI escape codes from a string</tr>
<tr><td>strip-bom</td><td>3.0.0</td><td>MIT</td><td>Strip UTF-8 byte order mark (BOM) from a string</tr>
<tr><td>string.prototype.trimstart</td><td>1.0.8</td><td>MIT</td><td>ES2019 spec-compliant String.prototype.trimStart shim.</tr>
<tr><td><a href="https://github.com/nodejs/string_decoder" target="_blank">string_decoder</a></td><td>1.3.0</td><td>MIT</td><td>The string_decoder module from Node core</tr>
<tr><td>string.prototype.trimend</td><td>1.0.8</td><td>MIT</td><td>ES2019 spec-compliant String.prototype.trimEnd shim.</tr>
<tr><td>string.prototype.trim</td><td>1.2.9</td><td>MIT</td><td>ES5 spec-compliant shim for String.prototype.trim</tr>
<tr><td><a href="https://mths.be/repeat" target="_blank">string.prototype.repeat</a></td><td>1.0.0</td><td>MIT</td><td>A robust & optimized `String.prototype.repeat` polyfill, based on the ECMAScript 6 specification.</tr>
<tr><td><a href="https://github.com/es-shims/String.prototype.matchAll#readme" target="_blank">string.prototype.matchall</a></td><td>4.0.11</td><td>MIT</td><td>Spec-compliant polyfill for String.prototype.matchAll</tr>
<tr><td>string-width</td><td>4.2.3</td><td>MIT</td><td>Get the visual width of a string - the number of columns required to display it</tr>
<tr><td>strict-uri-encode</td><td>1.1.0</td><td>MIT</td><td>A stricter URI encode adhering to RFC 3986</tr>
<tr><td>string-width</td><td>4.2.3</td><td>MIT</td><td>Get the visual width of a string - the number of columns required to display it</tr>
<tr><td>statuses</td><td>2.0.1</td><td>MIT</td><td>HTTP status utility</tr>
<tr><td>standard-engine</td><td>15.1.0</td><td>MIT</td><td>Wrap your standards in a tortilla and cover it in special sauce.</tr>
<tr><td><a href="https://standardjs.com" target="_blank">standard</a></td><td>17.1.2</td><td>MIT</td><td>JavaScript Standard Style</tr>
<tr><td>sprintf-js</td><td>1.1.3</td><td>BSD-3-Clause</td><td>JavaScript sprintf implementation</tr>
<tr><td><a href="http://pid.github.io/speakingurl/" target="_blank">speakingurl</a></td><td>14.0.1</td><td>BSD-3-Clause</td><td>Generate a slug – transliteration with a lot of options</tr>
<tr><td><a href="https://github.com/mafintosh/sparse-bitfield" target="_blank">sparse-bitfield</a></td><td>3.0.3</td><td>MIT</td><td>Bitfield that allocates a series of small buffers to support sparse bits without allocating a massive buffer</tr>
<tr><td><a href="https://github.com/mozilla/source-map" target="_blank">source-map</a></td><td>0.6.1</td><td>BSD-3-Clause</td><td>Generates and consumes source maps</tr>
<tr><td>space-separated-tokens</td><td>1.1.5</td><td>MIT</td><td>Parse and stringify space-separated tokens</tr>
<tr><td>sort-keys-length</td><td>1.0.1</td><td>MIT</td><td>Sort objecy keys by length</tr>
<tr><td><a href="https://github.com/JoshGlazebrook/smart-buffer/" target="_blank">smart-buffer</a></td><td>4.2.0</td><td>MIT</td><td>smart-buffer is a Buffer wrapper that adds automatic read & write offset tracking, string operations, data insertions, and more.</tr>
<tr><td>sort-keys</td><td>2.0.0</td><td>MIT</td><td>Sort the keys of an object</tr>
<tr><td>sisteransi</td><td>1.0.5</td><td>MIT</td><td>ANSI escape codes for some terminal swag</tr>
<tr><td><a href="https://github.com/JoshGlazebrook/socks/" target="_blank">socks</a></td><td>2.8.3</td><td>MIT</td><td>Fully featured SOCKS proxy client supporting SOCKSv4, SOCKSv4a, and SOCKSv5. Includes Bind and Associate functionality.</tr>
<tr><td><a href="https://github.com/feross/simple-get" target="_blank">simple-get</a></td><td>4.0.1</td><td>MIT</td><td>Simplest way to make http get requests. Supports HTTPS, redirects, gzip/deflate, streams in < 100 lines.</tr>
<tr><td><a href="https://github.com/feross/simple-concat" target="_blank">simple-concat</a></td><td>1.0.1</td><td>MIT</td><td>Super-minimalist version of `concat-stream`. Less than 15 lines!</tr>
<tr><td>signal-exit</td><td>4.1.0</td><td>ISC</td><td>when you want to fire an event no matter how a process exits.</tr>
<tr><td><a href="https://github.com/ljharb/side-channel#readme" target="_blank">side-channel</a></td><td>1.0.6</td><td>MIT</td><td>Store information about any JS value in a side channel. Uses WeakMap if available.</tr>
<tr><td><a href="https://github.com/shouldjs/util#readme" target="_blank">should-util</a></td><td>1.0.1</td><td>MIT</td><td>Utility functions</tr>
<tr><td><a href="https://github.com/shouldjs/type-adaptors#readme" target="_blank">should-type-adaptors</a></td><td>1.1.0</td><td>MIT</td><td>Small utility functions to use the same traversing etc code on different types</tr>
<tr><td><a href="https://github.com/shouldjs/type" target="_blank">should-type</a></td><td>1.4.0</td><td>MIT</td><td>Simple module to get instance type. Like a bit more advanced version of typeof</tr>
<tr><td>should-format</td><td>3.0.3</td><td>MIT</td><td>Formatting of objects for should.js</tr>
<tr><td><a href="https://github.com/shouldjs/should.js" target="_blank">should</a></td><td>13.2.3</td><td>MIT</td><td>test framework agnostic BDD-style assertions</tr>
<tr><td><a href="https://github.com/shouldjs/equal" target="_blank">should-equal</a></td><td>2.0.0</td><td>MIT</td><td>Deep comparison of 2 instances for should.js</tr>
<tr><td><a href="https://shortunique.id" target="_blank">short-unique-id</a></td><td>5.2.0</td><td>Apache-2.0</td><td>Generate random or sequential UUID of any length</tr>
<tr><td>shebang-command</td><td>2.0.0</td><td>MIT</td><td>Get the command from a shebang</tr>
<tr><td>shebang-regex</td><td>3.0.0</td><td>MIT</td><td>Regular expression for matching a shebang line</tr>
<tr><td><a href="https://github.com/crypto-browserify/sha.js" target="_blank">sha.js</a></td><td>2.4.11</td><td>(MIT AND BSD-3-Clause)</td><td>Streamable SHA hashes in pure javascript</tr>
<tr><td><a href="https://github.com/wesleytodd/setprototypeof" target="_blank">setprototypeof</a></td><td>1.2.0</td><td>ISC</td><td>A small polyfill for Object.setprototypeof</tr>
<tr><td>setimmediate</td><td>1.0.5</td><td>MIT</td><td>A shim for the setImmediate efficient script yielding API</tr>
<tr><td><a href="https://github.com/ljharb/set-function-name#readme" target="_blank">set-function-name</a></td><td>2.0.2</td><td>MIT</td><td>Set a function's name property</tr>
<tr><td><a href="https://github.com/ljharb/set-function-length#readme" target="_blank">set-function-length</a></td><td>1.2.2</td><td>MIT</td><td>Set a function's length property</tr>
<tr><td><a href="https://github.com/yahoo/serialize-javascript" target="_blank">serialize-javascript</a></td><td>6.0.2</td><td>BSD-3-Clause</td><td>Serialize JavaScript to a superset of JSON that includes regular expressions and functions.</tr>
<tr><td><a href="https://github.com/yargs/set-blocking#readme" target="_blank">set-blocking</a></td><td>2.0.0</td><td>ISC</td><td>set blocking stdio and stderr ensuring that terminal output does not truncate</tr>
<tr><td>serialize-error</td><td>8.1.0</td><td>MIT</td><td>Serialize/deserialize an error into a plain object</tr>
<tr><td>send</td><td>0.19.0</td><td>MIT</td><td>Better streaming static file server with Range and conditional-GET support</tr>
<tr><td>semver-diff</td><td>3.1.1</td><td>MIT</td><td>Get the diff type of two semver versions: 0.0.1 0.0.2 → patch</tr>
<tr><td>seek-bzip</td><td>1.0.6</td><td>MIT</td><td>a pure-JavaScript Node.JS module for random-access decoding bzip2 data</tr>
<tr><td>semver</td><td>7.6.3</td><td>ISC</td><td>The semantic version parser used by npm.</tr>
<tr><td><a href="https://github.com/vdemedes/secure-compare" target="_blank">secure-compare</a></td><td>3.0.1</td><td>MIT</td><td>Securely compare two strings, copied from cryptiles</tr>
<tr><td><a href="https://reactjs.org/" target="_blank">scheduler</a></td><td>0.23.2</td><td>MIT</td><td>Cooperative scheduler for the browser environment.</tr>
<tr><td>sax</td><td>1.4.1</td><td>ISC</td><td>An evented streaming XML parser in JavaScript</tr>
<tr><td>safer-buffer</td><td>2.1.2</td><td>MIT</td><td>Modern Buffer API polyfill without footguns</tr>
<tr><td>serve-static</td><td>1.16.2</td><td>MIT</td><td>Serve static files</tr>
<tr><td><a href="https://github.com/ljharb/safe-regex-test#readme" target="_blank">safe-regex-test</a></td><td>1.0.3</td><td>MIT</td><td>Give a regex, get a robust predicate function that tests it against a string.</tr>
<tr><td><a href="https://github.com/davisjam/safe-regex" target="_blank">safe-regex</a></td><td>2.1.1</td><td>MIT</td><td>detect possibly catastrophic, exponential-time regular expressions</tr>
<tr><td><a href="https://github.com/feross/safe-buffer" target="_blank">safe-buffer</a></td><td>5.1.2</td><td>MIT</td><td>Safer Node.js Buffer API</tr>
<tr><td><a href="https://github.com/ljharb/safe-array-concat#readme" target="_blank">safe-array-concat</a></td><td>1.1.2</td><td>MIT</td><td>`Array.prototype.concat`, but made safe by ignoring Symbol.isConcatSpreadable</tr>
<tr><td><a href="https://github.com/ReactiveX/RxJS" target="_blank">rxjs</a></td><td>6.6.7</td><td>Apache-2.0</td><td>Reactive Extensions for modern JavaScript</tr>
<tr><td><a href="https://github.com/feross/run-parallel" target="_blank">run-parallel</a></td><td>1.2.0</td><td>MIT</td><td>Run an array of functions in parallel</tr>
<tr><td>run-async</td><td>2.4.1</td><td>MIT</td><td>Utility method to run function either synchronously or asynchronously using the common `this.async()` style.</tr>
<tr><td>rimraf</td><td>3.0.2</td><td>ISC</td><td>A deep deletion module for node (like `rm -rf`)</tr>
<tr><td><a href="https://github.com/mcollina/reusify#readme" target="_blank">reusify</a></td><td>1.0.4</td><td>MIT</td><td>Reuse objects and functions with style</tr>
<tr><td>restore-cursor</td><td>3.1.0</td><td>MIT</td><td>Gracefully restore the CLI cursor on exit</tr>
<tr><td>ret</td><td>0.2.2</td><td>MIT</td><td>Tokenizes a string that represents a regular expression.</tr>
<tr><td>responselike</td><td>1.0.2</td><td>MIT</td><td>A response-like object for mocking a Node.js HTTP response stream</tr>
<tr><td>resolve-pathname</td><td>3.0.0</td><td>MIT</td><td>Resolve URL pathnames using JavaScript</tr>
<tr><td>resolve-from</td><td>4.0.0</td><td>MIT</td><td>Resolve the path of a module like `require.resolve()` but from a given path</tr>
<tr><td>reselect</td><td>5.1.1</td><td>MIT</td><td>Selectors for Redux.</tr>
<tr><td>resolve</td><td>1.22.8</td><td>MIT</td><td>resolve like require.resolve() on behalf of files asynchronously and synchronously</tr>
<tr><td><a href="https://github.com/hegemonic/requizzle" target="_blank">requizzle</a></td><td>0.2.4</td><td>MIT</td><td>Swizzle a little something into your require() calls.</tr>
<tr><td><a href="http://github.com/jrburke/r.js" target="_blank">requirejs</a></td><td>2.3.7</td><td>MIT</td><td>Node adapter for RequireJS, for loading AMD modules. Includes RequireJS optimizer</tr>
<tr><td><a href="https://github.com/unshiftio/requires-port" target="_blank">requires-port</a></td><td>1.0.0</td><td>MIT</td><td>Check if a protocol requires a certain port number to be added to an URL.</tr>
<tr><td><a href="https://github.com/yargs/require-main-filename#readme" target="_blank">require-main-filename</a></td><td>2.0.0</td><td>ISC</td><td>shim for require.main.filename() that works in as many environments as possible</tr>
<tr><td><a href="https://github.com/troygoode/node-require-directory/" target="_blank">require-directory</a></td><td>2.1.1</td><td>MIT</td><td>Recursively iterates over specified directory, require()'ing each file, and returning a nested hash structure containing those modules.</tr>
<tr><td><a href="https://github.com/jonschlinkert/repeat-string" target="_blank">repeat-string</a></td><td>1.6.1</td><td>MIT</td><td>Repeat the given string n times. Fastest implementation for repeating a string.</tr>
<tr><td>require-from-string</td><td>2.0.2</td><td>MIT</td><td>Require module from string</tr>
<tr><td><a href="https://github.com/jonschlinkert/remarkable" target="_blank">remarkable</a></td><td>2.0.1</td><td>MIT</td><td>Markdown parser, done right. 100% Commonmark support, extensions, syntax plugins, high speed - all in one.</tr>
<tr><td><a href="https://github.com/bnjmnt4n/regjsgen" target="_blank">regjsgen</a></td><td>0.8.0</td><td>MIT</td><td>Generate regular expressions from regjsparser’s AST.</tr>
<tr><td><a href="https://github.com/jviereck/regjsparser" target="_blank">regjsparser</a></td><td>0.11.0</td><td>BSD-2-Clause</td><td>undefined</tr>
<tr><td>registry-url</td><td>5.1.0</td><td>MIT</td><td>Get the set npm registry URL</tr>
<tr><td><a href="https://github.com/rexxars/registry-auth-token#readme" target="_blank">registry-auth-token</a></td><td>4.2.2</td><td>MIT</td><td>Get the auth token set for an npm registry (if any)</tr>
<tr><td><a href="https://mths.be/regexpu" target="_blank">regexpu-core</a></td><td>6.1.1</td><td>MIT</td><td>regexpu’s core functionality (i.e. `rewritePattern(pattern, flag)`), capable of translating ES6 Unicode regular expressions to ES5.</tr>
<tr><td><a href="https://github.com/mysticatea/regexpp#readme" target="_blank">regexpp</a></td><td>3.2.0</td><td>MIT</td><td>Regular expression parser for ECMAScript.</tr>
<tr><td>regexp.prototype.flags</td><td>1.5.3</td><td>MIT</td><td>ES6 spec-compliant RegExp.prototype.flags shim.</tr>
<tr><td>regenerator-transform</td><td>0.15.2</td><td>MIT</td><td>Explode async and generator functions into a state machine.</tr>
<tr><td><a href="https://github.com/DmitrySoshnikov/regexp-tree" target="_blank">regexp-tree</a></td><td>0.1.27</td><td>MIT</td><td>Regular Expressions parser in JavaScript</tr>
<tr><td>regenerator-runtime</td><td>0.14.1</td><td>MIT</td><td>Runtime for Regenerator-compiled generator and async functions.</tr>
<tr><td><a href="https://github.com/mathiasbynens/regenerate-unicode-properties" target="_blank">regenerate-unicode-properties</a></td><td>10.2.0</td><td>MIT</td><td>Regenerate sets for Unicode properties and values.</tr>
<tr><td><a href="https://mths.be/regenerate" target="_blank">regenerate</a></td><td>1.4.2</td><td>MIT</td><td>Generate JavaScript-compatible regular expressions based on a given set of Unicode symbols or code points.</tr>
<tr><td>refractor</td><td>3.6.0</td><td>MIT</td><td>Lightweight, robust, elegant virtual syntax highlighting using Prism</tr>
<tr><td><a href="https://github.com/es-shims/Reflect.getPrototypeOf" target="_blank">reflect.getprototypeof</a></td><td>1.0.6</td><td>MIT</td><td>An ES2015 mostly-spec-compliant `Reflect.getPrototypeOf` sham/polyfill/replacement that works in as many engines as possible</tr>
<tr><td>redux-immutable</td><td>4.0.0</td><td>BSD-3-Clause</td><td>redux-immutable is used to create an equivalent function of Redux combineReducers that works with Immutable.js state.</tr>
<tr><td><a href="http://redux.js.org" target="_blank">redux</a></td><td>5.0.1</td><td>MIT</td><td>Predictable state container for JavaScript apps</tr>
<tr><td><a href="https://github.com/paulmillr/readdirp" target="_blank">readdirp</a></td><td>3.6.0</td><td>MIT</td><td>Recursive version of fs.readdir with streaming API.</tr>
<tr><td>readable-web-to-node-stream</td><td>3.0.2</td><td>MIT</td><td>Converts a Web-API readable-stream into a Node readable-stream.</tr>
<tr><td><a href="https://github.com/react-syntax-highlighter/react-syntax-highlighter#readme" target="_blank">react-syntax-highlighter</a></td><td>15.5.0</td><td>MIT</td><td>syntax highlighting component for react with prismjs or highlightjs ast using inline styles</tr>
<tr><td>readable-stream</td><td>3.6.2</td><td>MIT</td><td>Streams3, a user-land copy of the stream library from Node.js</tr>
<tr><td><a href="https://github.com/reduxjs/react-redux" target="_blank">react-redux</a></td><td>9.1.2</td><td>MIT</td><td>Official React bindings for Redux</tr>
<tr><td><a href="https://github.com/xyc/react-inspector" target="_blank">react-inspector</a></td><td>6.0.2</td><td>MIT</td><td>Power of Browser DevTools inspectors right inside your React app</tr>
<tr><td>react-immutable-pure-component</td><td>2.2.2</td><td>MIT</td><td>React PureComponent implementation embracing Immutable.js</tr>
<tr><td><a href="https://reactjs.org/" target="_blank">react-is</a></td><td>16.13.1</td><td>MIT</td><td>Brand checking of React Elements.</tr>
<tr><td><a href="https://github.com/HurricaneJames/react-immutable-proptypes" target="_blank">react-immutable-proptypes</a></td><td>2.2.0</td><td>MIT</td><td>PropType validators that work with Immutable.js.</tr>
<tr><td><a href="https://github.com/nkbt/react-debounce-input" target="_blank">react-debounce-input</a></td><td>3.3.0</td><td>MIT</td><td>React component that renders Input with debounced onChange</tr>
<tr><td><a href="https://github.com/nkbt/react-copy-to-clipboard" target="_blank">react-copy-to-clipboard</a></td><td>5.1.0</td><td>MIT</td><td>Copy-to-clipboard React component</tr>
<tr><td><a href="https://reactjs.org/" target="_blank">react</a></td><td>18.3.1</td><td>MIT</td><td>React is a JavaScript library for building user interfaces.</tr>
<tr><td><a href="https://reactjs.org/" target="_blank">react-dom</a></td><td>18.3.1</td><td>MIT</td><td>React package for working with the DOM.</tr>
<tr><td>raw-body</td><td>2.5.2</td><td>MIT</td><td>Get and validate the raw body of a readable stream.</tr>
<tr><td><a href="https://github.com/animir/node-rate-limiter-flexible#readme" target="_blank">rate-limiter-flexible</a></td><td>2.4.2</td><td>ISC</td><td>Node.js rate limiter by key and protection from DDoS and Brute-Force attacks in process Memory, Redis, MongoDb, Memcached, MySQL, PostgreSQL, Cluster or PM</tr>
<tr><td>range-parser</td><td>1.2.1</td><td>MIT</td><td>Range header field string parser</tr>
<tr><td>rc</td><td>1.2.8</td><td>(BSD-2-Clause OR MIT OR Apache-2.0)</td><td>hardwired configuration loader</tr>
<tr><td><a href="https://github.com/crypto-browserify/randombytes" target="_blank">randombytes</a></td><td>2.1.0</td><td>MIT</td><td>random bytes from browserify stand alone</tr>
<tr><td>random-bytes</td><td>1.0.0</td><td>MIT</td><td>URL and cookie safe UIDs</tr>
<tr><td><a href="http://fent.github.io/randexp.js/" target="_blank">randexp</a></td><td>0.5.3</td><td>MIT</td><td>Create random strings that match a given regular expression.</tr>
<tr><td><a href="https://ramdajs.com/" target="_blank">ramda</a></td><td>0.30.1</td><td>MIT</td><td>A practical functional library for JavaScript programmers.</tr>
<tr><td><a href="https://github.com/char0n/ramda-adjunct" target="_blank">ramda-adjunct</a></td><td>5.1.0</td><td>BSD-3-Clause</td><td>Ramda Adjunct is the most popular and most comprehensive set of utilities for use with Ramda, providing a variety of useful, well tested functions with excellent documentation.</tr>
<tr><td><a href="https://github.com/unshiftio/querystringify" target="_blank">querystringify</a></td><td>2.2.0</td><td>MIT</td><td>Querystringify - Small, simple but powerful query string parser.</tr>
<tr><td><a href="https://github.com/ljharb/qs" target="_blank">qs</a></td><td>6.13.0</td><td>BSD-3-Clause</td><td>A querystring parser that supports nesting and arrays, with a depth limit</tr>
<tr><td>query-string</td><td>5.1.1</td><td>MIT</td><td>Parse and stringify URL query strings</tr>
<tr><td>pupa</td><td>2.1.1</td><td>MIT</td><td>Simple micro templating</tr>
<tr><td><a href="https://mths.be/punycode" target="_blank">punycode.js</a></td><td>2.3.1</td><td>MIT</td><td>A robust Punycode converter that fully complies to RFC 3492 and RFC 5891, and works on nearly all JavaScript platforms.</tr>
<tr><td><a href="https://mths.be/punycode" target="_blank">punycode</a></td><td>2.3.1</td><td>MIT</td><td>A robust Punycode converter that fully complies to RFC 3492 and RFC 5891, and works on nearly all JavaScript platforms.</tr>
<tr><td><a href="https://github.com/feross/queue-microtask" target="_blank">queue-microtask</a></td><td>1.2.3</td><td>MIT</td><td>fast, tiny `queueMicrotask` shim for modern engines</tr>
<tr><td>pump</td><td>3.0.2</td><td>MIT</td><td>pipe streams together and close all of them if one of them closes</tr>
<tr><td><a href="https://github.com/Rob--W/proxy-from-env#readme" target="_blank">proxy-from-env</a></td><td>1.1.0</td><td>MIT</td><td>Offers getProxyForUrl to get the proxy URL for a URL, respecting the *_PROXY (e.g. HTTP_PROXY) and NO_PROXY environment variables.</tr>
<tr><td><a href="https://github.com/rvagg/prr" target="_blank">prr</a></td><td>1.0.1</td><td>MIT</td><td>A better Object.defineProperty()</tr>
<tr><td>proxy-addr</td><td>2.0.7</td><td>MIT</td><td>Determine address of proxied request</tr>
<tr><td>proto-list</td><td>1.2.4</td><td>ISC</td><td>A utility for managing a prototype chain</tr>
<tr><td>property-information</td><td>5.6.0</td><td>MIT</td><td>Information for HTML properties</tr>
<tr><td><a href="https://facebook.github.io/react/" target="_blank">prop-types</a></td><td>15.8.1</td><td>MIT</td><td>Runtime type checking for React props and similar objects.</tr>
<tr><td>prompts</td><td>2.4.2</td><td>MIT</td><td>Lightweight, beautiful and user-friendly prompts</tr>
<tr><td><a href="https://github.com/calvinmetcalf/process-nextick-args" target="_blank">process-nextick-args</a></td><td>2.0.1</td><td>MIT</td><td>process.nextTick but always with args</tr>
<tr><td>process</td><td>0.11.10</td><td>MIT</td><td>process information for node.js and browsers</tr>
<tr><td>prismjs</td><td>1.29.0</td><td>MIT</td><td>Lightweight, robust, elegant syntax highlighting. A spin-off project from Dabblet.</tr>
<tr><td>progress</td><td>2.0.3</td><td>MIT</td><td>Flexible ascii progress bar</tr>
<tr><td>prepend-http</td><td>2.0.0</td><td>MIT</td><td>Prepend `http://` to humanized URLs like todomvc.com and localhost</tr>
<tr><td><a href="https://github.com/prebuild/prebuild-install" target="_blank">prebuild-install</a></td><td>7.1.2</td><td>MIT</td><td>A command line tool to easily install prebuilt binaries for multiple version of node/iojs on a specific platform</tr>
<tr><td><a href="http://preludels.com" target="_blank">prelude-ls</a></td><td>1.2.1</td><td>MIT</td><td>prelude.ls is a functionally oriented utility library. It is powerful and flexible. Almost all of its functions are curried. It is written in, and is the recommended base library for, LiveScript.</tr>
<tr><td><a href="https://github.com/ljharb/possible-typed-array-names#readme" target="_blank">possible-typed-array-names</a></td><td>1.0.0</td><td>MIT</td><td>A simple list of possible Typed Array names.</tr>
<tr><td>portfinder</td><td>1.0.32</td><td>MIT</td><td>A simple tool to find an open port on the current machine</tr>
<tr><td>pkg-conf</td><td>3.1.0</td><td>MIT</td><td>Get namespaced config from the closest package.json</tr>
<tr><td>pinkie-promise</td><td>2.0.1</td><td>MIT</td><td>ES2015 Promise ponyfill</tr>
<tr><td><a href="https://github.com/micromatch/picomatch" target="_blank">picomatch</a></td><td>2.3.1</td><td>MIT</td><td>Blazing fast and accurate glob matcher written in JavaScript, with no dependencies and full support for standard and extended Bash glob features, including braces, extglobs, POSIX brackets, and regular expressions.</tr>
<tr><td>pinkie</td><td>2.0.4</td><td>MIT</td><td>Itty bitty little widdle twinkie pinkie ES2015 Promise implementation</tr>
<tr><td>pify</td><td>2.3.0</td><td>MIT</td><td>Promisify a callback-style function</tr>
<tr><td>picocolors</td><td>1.1.0</td><td>ISC</td><td>The tiniest and the fastest library for terminal output formatting with ANSI colors</tr>
<tr><td>peek-readable</td><td>5.2.0</td><td>MIT</td><td>Read and peek from a readable stream</tr>
<tr><td>path-to-regexp</td><td>8.2.0</td><td>MIT</td><td>Express style path to RegExp utility</tr>
<tr><td>path-scurry</td><td>2.0.0</td><td>BlueOak-1.0.0</td><td>walk paths fast and efficiently</tr>
<tr><td>pend</td><td>1.2.0</td><td>MIT</td><td>dead-simple optimistic async helper</tr>
<tr><td><a href="https://github.com/jbgutierrez/path-parse#readme" target="_blank">path-parse</a></td><td>1.0.7</td><td>MIT</td><td>Node.js path.parse() ponyfill</tr>
<tr><td>path-is-absolute</td><td>1.0.1</td><td>MIT</td><td>Node.js 0.12 path.isAbsolute() ponyfill</tr>
<tr><td>path-exists</td><td>5.0.0</td><td>MIT</td><td>Check if a path exists</tr>
<tr><td>parseurl</td><td>1.3.3</td><td>MIT</td><td>parse a url with memoization</tr>
<tr><td>parse-node-version</td><td>1.0.1</td><td>MIT</td><td>Turn node's process.version into something useful.</tr>
<tr><td>path-key</td><td>3.1.1</td><td>MIT</td><td>Get the PATH environment variable key cross-platform</tr>
<tr><td>parse-json</td><td>4.0.0</td><td>MIT</td><td>Parse JSON with more helpful errors</tr>
<tr><td><a href="https://github.com/jonschlinkert/parse-github-url" target="_blank">parse-github-url</a></td><td>1.0.3</td><td>MIT</td><td>Parse a github URL into an object.</tr>
<tr><td>parse-entities</td><td>2.0.0</td><td>MIT</td><td>Parse HTML character references: fast, spec-compliant, positional information</tr>
<tr><td>parse-cache-control</td><td>1.0.1</td><td>undefined</td><td>Parse Cache-Control headers.</tr>
<tr><td>parent-require</td><td>1.0.0</td><td>undefined</td><td>Require modules from parent modules.</tr>
<tr><td><a href="https://github.com/nodeca/pako" target="_blank">pako</a></td><td>1.0.11</td><td>(MIT AND Zlib)</td><td>zlib port to javascript - fast, modularized, with browser support</tr>
<tr><td>parent-module</td><td>1.0.1</td><td>MIT</td><td>Get the path of the parent module</tr>
<tr><td>package-json-from-dist</td><td>1.0.1</td><td>BlueOak-1.0.0</td><td>Load the local package.json from either src or dist folder</tr>
<tr><td>package-json</td><td>6.5.0</td><td>MIT</td><td>Get metadata of a package from the npm registry</tr>
<tr><td>p-try</td><td>2.2.0</td><td>MIT</td><td>`Start a promise chain</tr>
<tr><td>p-locate</td><td>6.0.0</td><td>MIT</td><td>Get the first fulfilled promise that satisfies the provided testing function</tr>
<tr><td>p-timeout</td><td>2.0.1</td><td>MIT</td><td>Timeout a promise after a specified amount of time</tr>
<tr><td>p-limit</td><td>4.0.0</td><td>MIT</td><td>Run multiple promise-returning & async functions with limited concurrency</tr>
<tr><td>p-finally</td><td>1.0.0</td><td>MIT</td><td>`Promise#finally()` ponyfill - Invoked when the promise is settled regardless of outcome</tr>
<tr><td>p-event</td><td>4.2.0</td><td>MIT</td><td>Promisify an event by waiting for it to be emitted</tr>
<tr><td>p-is-promise</td><td>1.1.0</td><td>MIT</td><td>Check if something is a promise</tr>
<tr><td>os-tmpdir</td><td>1.0.2</td><td>MIT</td><td>Node.js os.tmpdir() ponyfill</tr>
<tr><td>p-cancelable</td><td>0.4.1</td><td>MIT</td><td>Create a promise that can be canceled</tr>
<tr><td><a href="http://khtdr.com/opts" target="_blank">opts</a></td><td>2.0.2</td><td>BSD-2-Clause</td><td>Command line argument parser with automatic help text generation.</tr>
<tr><td>opener</td><td>1.5.2</td><td>(WTFPL OR MIT)</td><td>Opens stuff, like webpages and files and executables, cross-platform</tr>
<tr><td><a href="https://github.com/gkz/optionator" target="_blank">optionator</a></td><td>0.9.4</td><td>MIT</td><td>option parsing and help generation</tr>
<tr><td>open</td><td>6.4.0</td><td>MIT</td><td>Open stuff like URLs, files, executables. Cross-platform.</tr>
<tr><td><a href="https://github.com/opencollective/opencollective-postinstall#readme" target="_blank">opencollective-postinstall</a></td><td>2.0.3</td><td>MIT</td><td>Lightweight npm postinstall message to invite people to donate to your collective</tr>
<tr><td><a href="https://github.com/swaggerexpert/openapi-path-templating#readme" target="_blank">openapi-path-templating</a></td><td>1.6.0</td><td>Apache-2.0</td><td>OpenAPI Path Templating parser, validator and resolver.</tr>
<tr><td>onetime</td><td>5.1.2</td><td>MIT</td><td>Ensure a function is only called once</tr>
<tr><td><a href="https://github.com/swaggerexpert/openapi-server-url-templating#readme" target="_blank">openapi-server-url-templating</a></td><td>1.1.0</td><td>Apache-2.0</td><td>OpenAPI Server URL templating parser, validator and substitution mechanism.</tr>
<tr><td>once</td><td>1.4.0</td><td>ISC</td><td>Run a function exactly one time</tr>
<tr><td>on-headers</td><td>1.0.2</td><td>MIT</td><td>Execute a listener when a response is about to write headers</tr>
<tr><td>on-finished</td><td>2.4.1</td><td>MIT</td><td>Execute a callback when a request closes, finishes, or errors</tr>
<tr><td><a href="https://github.com/es-shims/Object.groupBy#readme" target="_blank">object.groupby</a></td><td>1.0.3</td><td>MIT</td><td>An ESnext spec-compliant `Object.groupBy` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td>object.values</td><td>1.2.0</td><td>MIT</td><td>ES2017 spec-compliant Object.values shim.</tr>
<tr><td>object.entries</td><td>1.1.8</td><td>MIT</td><td>ES2017 spec-compliant Object.entries shim.</tr>
<tr><td>object.fromentries</td><td>2.0.8</td><td>MIT</td><td>ES proposal-spec-compliant Object.fromEntries shim.</tr>
<tr><td>object-keys</td><td>1.1.1</td><td>MIT</td><td>An Object.keys replacement, in case Object.keys is not available. From https://github.com/es-shims/es5-shim</tr>
<tr><td><a href="https://github.com/inspect-js/object-inspect" target="_blank">object-inspect</a></td><td>1.13.2</td><td>MIT</td><td>string representations of objects in node and the browser</tr>
<tr><td>object.assign</td><td>4.1.5</td><td>MIT</td><td>ES6 spec-compliant Object.assign shim. From https://github.com/es-shims/es6-shim</tr>
<tr><td>object-assign</td><td>4.1.1</td><td>MIT</td><td>ES2015 `Object.assign()` ponyfill</tr>
<tr><td>normalize-url</td><td>2.0.1</td><td>MIT</td><td>Normalize a URL</tr>
<tr><td>npm-conf</td><td>1.1.3</td><td>MIT</td><td>Get the npm config</tr>
<tr><td><a href="https://github.com/jonschlinkert/normalize-path" target="_blank">normalize-path</a></td><td>3.0.0</td><td>MIT</td><td>Normalize slashes in a file path to be posix/unix-like forward slashes. Also condenses repeat slashes to a single slash and removes and trailing slashes, unless disabled.</tr>
<tr><td><a href="https://nodemailer.com/" target="_blank">nodemailer</a></td><td>6.9.15</td><td>MIT-0</td><td>Easy as cake e-mail sending from your Node.js applications</tr>
<tr><td>node-releases</td><td>2.0.18</td><td>MIT</td><td>Node.js releases data</tr>
<tr><td>node-fetch-commonjs</td><td>3.3.2</td><td>MIT</td><td>A light-weight module that brings Fetch API to node.js</tr>
<tr><td><a href="https://github.com/node-fetch/node-fetch" target="_blank">node-fetch</a></td><td>3.3.2</td><td>MIT</td><td>A light-weight module that brings Fetch API to node.js</tr>
<tr><td><a href="https://github.com/jimmywarting/node-domexception#readme" target="_blank">node-domexception</a></td><td>1.0.0</td><td>MIT</td><td>An implementation of the DOMException class from NodeJS</tr>
<tr><td><a href="https://github.com/electron/node-abi#readme" target="_blank">node-abi</a></td><td>3.68.0</td><td>MIT</td><td>Get the Node ABI for a given target and runtime, and vice versa.</tr>
<tr><td><a href="https://github.com/southpolesteve/node-abort-controller#readme" target="_blank">node-abort-controller</a></td><td>3.1.1</td><td>MIT</td><td>AbortController for Node based on EventEmitter</tr>
<tr><td>nested-error-stacks</td><td>2.1.1</td><td>MIT</td><td>An Error subclass that will chain nested Errors and dump nested stacktraces</tr>
<tr><td><a href="https://github.com/PuruVJ/neotraverse" target="_blank">neotraverse</a></td><td>0.6.18</td><td>MIT</td><td>traverse and transform objects by visiting every node on a recursive walk</tr>
<tr><td>negotiator</td><td>0.6.3</td><td>MIT</td><td>HTTP content negotiation</tr>
<tr><td><a href="https://github.com/suguru03/neo-async" target="_blank">neo-async</a></td><td>2.6.2</td><td>MIT</td><td>Neo-Async is a drop-in replacement for Async, it almost fully covers its functionality and runs faster </tr>
<tr><td>needle</td><td>3.3.1</td><td>MIT</td><td>The leanest and most handsome HTTP client in the Nodelands.</tr>
<tr><td>natural-compare</td><td>1.4.0</td><td>MIT</td><td>Compare strings containing a mix of letters and numbers in the way a human being would in sort order.</tr>
<tr><td><a href="https://github.com/inspiredware/napi-build-utils#readme" target="_blank">napi-build-utils</a></td><td>1.0.2</td><td>MIT</td><td>A set of utilities to assist developers of tools that build N-API native add-ons</tr>
<tr><td>nan</td><td>2.20.0</td><td>MIT</td><td>Native Abstractions for Node.js: C++ header for Node 0.8 -> 22 compatibility</tr>
<tr><td>mute-stream</td><td>0.0.8</td><td>ISC</td><td>Bytes go in, but they don't come out (when muted).</tr>
<tr><td>ms</td><td>2.1.3</td><td>MIT</td><td>Tiny millisecond conversion utility</tr>
<tr><td><a href="https://github.com/mongodb/node-mongodb-native" target="_blank">mongodb</a></td><td>6.9.0</td><td>Apache-2.0</td><td>The official MongoDB driver for Node.js</tr>
<tr><td><a href="https://github.com/mongodb-js/mongodb-connection-string-url" target="_blank">mongodb-connection-string-url</a></td><td>3.0.1</td><td>Apache-2.0</td><td>MongoDB connection strings, based on the WhatWG URL API</tr>
<tr><td><a href="https://mochajs.org/" target="_blank">mocha</a></td><td>10.7.3</td><td>MIT</td><td>simple, flexible, fun test framework</tr>
<tr><td>mkdirp</td><td>1.0.4</td><td>MIT</td><td>Recursively mkdir, like `mkdir -p`</tr>
<tr><td><a href="https://github.com/mafintosh/mkdirp-classic" target="_blank">mkdirp-classic</a></td><td>0.5.3</td><td>MIT</td><td>Mirror of mkdirp 0.5.2</tr>
<tr><td>minipass</td><td>7.1.2</td><td>ISC</td><td>minimal implementation of a PassThrough stream</tr>
<tr><td><a href="https://github.com/minimistjs/minimist" target="_blank">minimist</a></td><td>1.2.8</td><td>MIT</td><td>parse argument options</tr>
<tr><td><a href="https://github.com/calvinmetcalf/minimalistic-assert" target="_blank">minimalistic-assert</a></td><td>1.0.1</td><td>ISC</td><td>minimalistic-assert ===</tr>
<tr><td>minimatch</td><td>3.1.2</td><td>ISC</td><td>a glob matcher in javascript</tr>
<tr><td><a href="https://github.com/refractproject/minim" target="_blank">minim</a></td><td>0.23.8</td><td>MIT</td><td>A library for interacting with JSON through Refract elements</tr>
<tr><td>min-indent</td><td>1.0.1</td><td>MIT</td><td>Get the shortest leading whitespace from lines in a string</tr>
<tr><td>mimic-fn</td><td>2.1.0</td><td>MIT</td><td>Make a function mimic another one</tr>
<tr><td>mimic-response</td><td>1.0.1</td><td>MIT</td><td>Mimic a Node.js HTTP response stream</tr>
<tr><td>mime-types</td><td>2.1.35</td><td>MIT</td><td>The ultimate javascript content-type utility.</tr>
<tr><td>mime-db</td><td>1.53.0</td><td>MIT</td><td>Media Type Database</tr>
<tr><td>methods</td><td>1.1.2</td><td>MIT</td><td>HTTP methods that node supports</tr>
<tr><td>mime</td><td>1.6.0</td><td>MIT</td><td>A comprehensive library for mime-type mapping</tr>
<tr><td>merge-descriptors</td><td>1.0.3</td><td>MIT</td><td>Merge objects using descriptors</tr>
<tr><td><a href="https://github.com/mafintosh/memory-pager" target="_blank">memory-pager</a></td><td>1.5.0</td><td>MIT</td><td>Access memory using small fixed sized buffers</tr>
<tr><td>medium-zoom</td><td>1.1.0</td><td>MIT</td><td>A JavaScript library for zooming images like Medium</tr>
<tr><td>media-typer</td><td>0.3.0</td><td>MIT</td><td>Simple RFC 6838 media type parser and formatter</tr>
<tr><td>mdurl</td><td>2.0.0</td><td>MIT</td><td>URL utilities for markdown-it</tr>
<tr><td>markdown-it-anchor</td><td>8.6.7</td><td>Unlicense</td><td>Header anchors for markdown-it.</tr>
<tr><td><a href="https://marked.js.org" target="_blank">marked</a></td><td>1.2.9</td><td>MIT</td><td>A markdown parser built for speed</tr>
<tr><td>markdown-it</td><td>14.1.0</td><td>MIT</td><td>Markdown-it - modern pluggable markdown parser.</tr>
<tr><td>make-dir</td><td>1.3.0</td><td>MIT</td><td>Make a directory and its parents if needed - Think `mkdir -p`</tr>
<tr><td>lowlight</td><td>1.20.0</td><td>MIT</td><td>Virtual syntax highlighting for virtual DOMs and non-HTML things</tr>
<tr><td>lowercase-keys</td><td>1.0.1</td><td>MIT</td><td>Lowercase the keys of an object</tr>
<tr><td>lru-cache</td><td>5.1.1</td><td>ISC</td><td>A cache object that deletes the least-recently-used items.</tr>
<tr><td><a href="https://github.com/zertosh/loose-envify" target="_blank">loose-envify</a></td><td>1.4.0</td><td>MIT</td><td>Fast (and loose) selective `process.env` replacer using js-tokens instead of an AST</tr>
<tr><td>log-symbols</td><td>4.1.0</td><td>MIT</td><td>Colored symbols for various log levels. Example: `✔︎ Success`</tr>
<tr><td><a href="https://lodash.com/" target="_blank">lodash.merge</a></td><td>4.6.2</td><td>MIT</td><td>The Lodash method `_.merge` exported as a module.</tr>
<tr><td><a href="https://lodash.com/" target="_blank">lodash.debounce</a></td><td>4.0.8</td><td>MIT</td><td>The lodash method `_.debounce` exported as a module.</tr>
<tr><td><a href="https://lodash.com/custom-builds" target="_blank">lodash-es</a></td><td>4.17.21</td><td>MIT</td><td>Lodash exported as ES modules.</tr>
<tr><td><a href="https://lodash.com/" target="_blank">lodash</a></td><td>4.17.21</td><td>MIT</td><td>Lodash modular utilities.</tr>
<tr><td>locate-path</td><td>7.2.0</td><td>MIT</td><td>Get the first path that exists on disk of multiple paths</tr>
<tr><td>load-json-file</td><td>5.3.0</td><td>MIT</td><td>Read and parse a JSON file</tr>
<tr><td><a href="https://github.com/livereload/livereload-js" target="_blank">livereload-js</a></td><td>3.4.1</td><td>MIT</td><td>LiveReload JS client - auto reload browser on changes</tr>
<tr><td>livereload</td><td>0.9.3</td><td>MIT</td><td>LiveReload server</tr>
<tr><td>linkify-it</td><td>5.0.0</td><td>MIT</td><td>Links recognition library with FULL unicode support</tr>
<tr><td>lie</td><td>3.3.0</td><td>MIT</td><td>A basic but performant promise implementation</tr>
<tr><td><a href="https://github.com/gkz/levn" target="_blank">levn</a></td><td>0.4.1</td><td>MIT</td><td>Light ECMAScript (JavaScript) Value Notation - human written, concise, typed, flexible</tr>
<tr><td><a href="http://lesscss.org" target="_blank">less</a></td><td>4.2.0</td><td>Apache-2.0</td><td>Leaner CSS</tr>
<tr><td>kleur</td><td>3.0.3</td><td>MIT</td><td>The fastest Node.js library for formatting terminal text with ANSI colors~!</tr>
<tr><td>kruptein</td><td>3.0.7</td><td>MIT</td><td>crypto; from kruptein to hide or conceal</tr>
<tr><td>latest-version</td><td>5.1.0</td><td>MIT</td><td>Get the latest version of an npm package</tr>
<tr><td><a href="https://github.com/jaredwray/keyv" target="_blank">keyv</a></td><td>4.5.4</td><td>MIT</td><td>Simple key-value storage with support for multiple backends</tr>
<tr><td><a href="https://github.com/jprichardson/node-klaw#readme" target="_blank">klaw</a></td><td>3.0.0</td><td>MIT</td><td>File system walker with Readable stream interface.</tr>
<tr><td>jws</td><td>3.2.2</td><td>MIT</td><td>Implementation of JSON Web Signatures</tr>
<tr><td>jwa</td><td>1.4.1</td><td>MIT</td><td>JWA implementation (supports all JWS algorithms)</tr>
<tr><td>jszip</td><td>3.10.1</td><td>(MIT OR GPL-3.0-or-later)</td><td>Create, read and edit .zip files with JavaScript http://stuartk.com/jszip</tr>
<tr><td>jsx-ast-utils</td><td>3.3.5</td><td>MIT</td><td>AST utility module for statically analyzing JSX</tr>
<tr><td>jsonfile</td><td>6.1.0</td><td>MIT</td><td>Easily read/write JSON files.</tr>
<tr><td>jsonwebtoken</td><td>9.0.0</td><td>MIT</td><td>JSON Web Token implementation (symmetric and asymmetric)</tr>
<tr><td><a href="http://json5.org/" target="_blank">json5</a></td><td>2.2.3</td><td>MIT</td><td>JSON for Humans</tr>
<tr><td><a href="https://github.com/samn/json-stable-stringify" target="_blank">json-stable-stringify-without-jsonify</a></td><td>1.0.1</td><td>MIT</td><td>deterministic JSON.stringify() with custom sorting to get deterministic hashes from stringified results, with no public domain dependencies</tr>
<tr><td><a href="https://github.com/epoberezkin/json-schema-traverse#readme" target="_blank">json-schema-traverse</a></td><td>1.0.0</td><td>MIT</td><td>Traverse JSON Schema passing each schema object to callback</tr>
<tr><td><a href="https://github.com/codenothing/jsonlint" target="_blank">json-lint</a></td><td>0.1.0</td><td>undefined</td><td>JSON Lint with comments</tr>
<tr><td>json-parse-better-errors</td><td>1.0.2</td><td>MIT</td><td>JSON.parse with context information on error</tr>
<tr><td><a href="https://github.com/dominictarr/json-buffer" target="_blank">json-buffer</a></td><td>3.0.1</td><td>MIT</td><td>JSON parse & stringify that supports binary via bops & base64</tr>
<tr><td><a href="https://mths.be/jsesc" target="_blank">jsesc</a></td><td>3.0.2</td><td>MIT</td><td>Given some data, jsesc returns the shortest possible stringified & ASCII-safe representation of that data.</tr>
<tr><td>jsbn</td><td>1.1.0</td><td>MIT</td><td>The jsbn library is a fast, portable implementation of large-number math in pure JavaScript, enabling public-key crypto and other applications on desktop and mobile browsers.</tr>
<tr><td>jsdoc</td><td>4.0.3</td><td>Apache-2.0</td><td>An API documentation generator for JavaScript.</tr>
<tr><td>js2xmlparser</td><td>4.0.2</td><td>Apache-2.0</td><td>Parses JavaScript objects into XML</tr>
<tr><td>js-yaml</td><td>4.1.0</td><td>MIT</td><td>YAML 1.2 parser and serializer</tr>
<tr><td>js-tokens</td><td>4.0.0</td><td>MIT</td><td>A regex that tokenizes JavaScript.</tr>
<tr><td><a href="https://github.com/kennethjiang/js-file-download" target="_blank">js-file-download</a></td><td>0.4.12</td><td>MIT</td><td>Javascript function that triggers browser to save javascript-generated content to a file</tr>
<tr><td>jackspeak</td><td>4.0.2</td><td>BlueOak-1.0.0</td><td>A very strict and proper argument parser.</tr>
<tr><td>isurl</td><td>1.0.0</td><td>MIT</td><td>Checks whether a value is a WHATWG URL.</tr>
<tr><td><a href="https://github.com/isaacs/isexe#readme" target="_blank">isexe</a></td><td>2.0.0</td><td>ISC</td><td>Minimal module to check if a file is executable.</tr>
<tr><td><a href="https://github.com/ljharb/Iterator.prototype#readme" target="_blank">iterator.prototype</a></td><td>1.1.2</td><td>MIT</td><td>`Iterator.prototype`, or a shared object to use.</tr>
<tr><td>is-yarn-global</td><td>0.3.0</td><td>MIT</td><td>Check if installed by yarn globally without any `fs` calls</tr>
<tr><td><a href="https://github.com/juliangruber/isarray" target="_blank">isarray</a></td><td>2.0.5</td><td>MIT</td><td>Array#isArray for older browsers</tr>
<tr><td>is-wsl</td><td>1.1.0</td><td>MIT</td><td>Check if the process is running inside Windows Subsystem for Linux (Bash on Windows)</tr>
<tr><td><a href="https://github.com/mesqueeb/is-what#readme" target="_blank">is-what</a></td><td>3.14.1</td><td>MIT</td><td>JS type check (TypeScript supported) functions like `isPlainObject() isArray()` etc. A simple & small integration.</tr>
<tr><td><a href="https://github.com/inspect-js/is-weakset#readme" target="_blank">is-weakset</a></td><td>2.0.3</td><td>MIT</td><td>Is this value a JS WeakSet? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-weakref#readme" target="_blank">is-weakref</a></td><td>1.0.2</td><td>MIT</td><td>Is this value a JS WeakRef? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-weakmap#readme" target="_blank">is-weakmap</a></td><td>2.0.2</td><td>MIT</td><td>Is this value a JS WeakMap? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td>is-unicode-supported</td><td>0.1.0</td><td>MIT</td><td>Detect whether the terminal supports Unicode</tr>
<tr><td>is-typed-array</td><td>1.1.13</td><td>MIT</td><td>Is this value a JS Typed Array? This module works cross-realm/iframe, does not depend on `instanceof` or mutable properties, and despite ES6 Symbol.toStringTag.</tr>
<tr><td><a href="https://github.com/hughsk/is-typedarray" target="_blank">is-typedarray</a></td><td>1.0.0</td><td>MIT</td><td>Detect whether or not an object is a Typed Array</tr>
<tr><td>is-string</td><td>1.0.7</td><td>MIT</td><td>Is this value a JS String object or primitive? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-shared-array-buffer#readme" target="_blank">is-shared-array-buffer</a></td><td>1.0.3</td><td>MIT</td><td>Is this value a JS SharedArrayBuffer?</tr>
<tr><td>is-symbol</td><td>1.0.4</td><td>MIT</td><td>Determine if a value is an ES6 Symbol or not.</tr>
<tr><td>is-stream</td><td>1.1.0</td><td>MIT</td><td>Check if something is a Node.js stream</tr>
<tr><td><a href="https://github.com/inspect-js/is-set#readme" target="_blank">is-set</a></td><td>2.0.3</td><td>MIT</td><td>Is this value a JS Set? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td>is-retry-allowed</td><td>1.2.0</td><td>MIT</td><td>Is retry allowed for Error?</tr>
<tr><td>is-plain-obj</td><td>1.1.0</td><td>MIT</td><td>Check if a value is a plain object</tr>
<tr><td><a href="https://github.com/inspect-js/is-regex" target="_blank">is-regex</a></td><td>1.1.4</td><td>MIT</td><td>Is this value a JS regex? Works cross-realm/iframe, and despite ES6 @@toStringTag</tr>
<tr><td>is-path-inside</td><td>3.0.3</td><td>MIT</td><td>Check if a path is inside another path</tr>
<tr><td><a href="https://github.com/inspect-js/is-number-object#readme" target="_blank">is-number-object</a></td><td>1.0.7</td><td>MIT</td><td>Is this value a JS Number object? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-object" target="_blank">is-object</a></td><td>1.0.2</td><td>MIT</td><td>Checks whether a value is an object</tr>
<tr><td>is-obj</td><td>2.0.0</td><td>MIT</td><td>Check if a value is an object</tr>
<tr><td><a href="https://github.com/jonschlinkert/is-number" target="_blank">is-number</a></td><td>7.0.0</td><td>MIT</td><td>Returns true if a number or string value is a finite number. Useful for regex matches, parsing, user input, etc.</tr>
<tr><td>is-npm</td><td>4.0.0</td><td>MIT</td><td>Check if your code is running as an npm script</tr>
<tr><td><a href="https://github.com/inspect-js/is-negative-zero" target="_blank">is-negative-zero</a></td><td>2.0.3</td><td>MIT</td><td>Is this value negative zero? === will lie to you</tr>
<tr><td>is-natural-number</td><td>4.0.1</td><td>MIT</td><td>Check if a value is a natural number</tr>
<tr><td><a href="https://github.com/inspect-js/is-map#readme" target="_blank">is-map</a></td><td>2.0.3</td><td>MIT</td><td>Is this value a JS Map? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td>is-hexadecimal</td><td>1.0.4</td><td>MIT</td><td>Check if a character is hexadecimal</tr>
<tr><td><a href="https://github.com/micromatch/is-glob" target="_blank">is-glob</a></td><td>4.0.3</td><td>MIT</td><td>Returns `true` if the given string looks like a glob pattern or an extglob pattern. This makes it easy to create code that only uses external modules like node-glob when necessary, resulting in much faster code execution and initialization time, and a better user experience.</tr>
<tr><td>is-installed-globally</td><td>0.3.2</td><td>MIT</td><td>Check if your package was installed globally</tr>
<tr><td><a href="https://github.com/inspect-js/is-finalizationregistry#readme" target="_blank">is-finalizationregistry</a></td><td>1.0.2</td><td>MIT</td><td>Is this value a JS FinalizationRegistry? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td>is-generator-function</td><td>1.0.10</td><td>MIT</td><td>Determine if a function is a native generator function.</tr>
<tr><td>is-fullwidth-code-point</td><td>3.0.0</td><td>MIT</td><td>Check if the character represented by a given Unicode code point is fullwidth</tr>
<tr><td><a href="https://github.com/jonschlinkert/is-extglob" target="_blank">is-extglob</a></td><td>2.1.1</td><td>MIT</td><td>Returns true if a string has an extglob.</tr>
<tr><td>is-decimal</td><td>1.0.4</td><td>MIT</td><td>Check if a character is decimal</tr>
<tr><td>is-date-object</td><td>1.0.5</td><td>MIT</td><td>Is this value a JS Date object? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-data-view#readme" target="_blank">is-data-view</a></td><td>1.0.1</td><td>MIT</td><td>Is this value a JS DataView? This module works cross-realm/iframe, does not depend on `instanceof` or mutable properties, and despite ES6 Symbol.toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-core-module" target="_blank">is-core-module</a></td><td>2.15.1</td><td>MIT</td><td>Is this specifier a node.js core module?</tr>
<tr><td><a href="https://github.com/watson/is-ci" target="_blank">is-ci</a></td><td>2.0.0</td><td>MIT</td><td>Detect if the current environment is a CI server</tr>
<tr><td>is-callable</td><td>1.2.7</td><td>MIT</td><td>Is this JS value callable? Works with Functions and GeneratorFunctions, despite ES6 @@toStringTag.</tr>
<tr><td>is-binary-path</td><td>2.1.0</td><td>MIT</td><td>Check if a file path is a binary file</tr>
<tr><td>is-boolean-object</td><td>1.1.2</td><td>MIT</td><td>Is this value a JS Boolean? This module works cross-realm/iframe, and despite ES6 @@toStringTag.</tr>
<tr><td><a href="https://github.com/inspect-js/is-bigint#readme" target="_blank">is-bigint</a></td><td>1.0.4</td><td>MIT</td><td>Is this value an ES BigInt?</tr>
<tr><td>is-async-function</td><td>2.0.0</td><td>MIT</td><td>Determine if a function is a native async function.</tr>
<tr><td><a href="https://github.com/inspect-js/is-array-buffer#readme" target="_blank">is-array-buffer</a></td><td>3.0.4</td><td>MIT</td><td>Is this value a JS ArrayBuffer?</tr>
<tr><td>is-arrayish</td><td>0.2.1</td><td>MIT</td><td>Determines if an object can be used as an array</tr>
<tr><td>is-alphanumerical</td><td>1.0.4</td><td>MIT</td><td>Check if a character is alphanumerical</tr>
<tr><td>ip-address</td><td>9.0.5</td><td>MIT</td><td>A library for parsing IPv4 and IPv6 IP addresses in node and the browser.</tr>
<tr><td>ipaddr.js</td><td>1.9.1</td><td>MIT</td><td>A library for manipulating IPv4 and IPv6 addresses in JavaScript.</tr>
<tr><td>is-alphabetical</td><td>1.0.4</td><td>MIT</td><td>Check if a character is alphabetical</tr>
<tr><td>invariant</td><td>2.2.4</td><td>MIT</td><td>invariant</tr>
<tr><td><a href="https://github.com/ljharb/internal-slot#readme" target="_blank">internal-slot</a></td><td>1.0.7</td><td>MIT</td><td>ES spec-like internal slots</tr>
<tr><td>into-stream</td><td>3.1.0</td><td>MIT</td><td>Convert a buffer/string/array/object/iterable/promise into a stream</tr>
<tr><td>inquirer</td><td>7.3.3</td><td>MIT</td><td>A collection of common interactive command line user interfaces.</tr>
<tr><td>ini</td><td>1.3.8</td><td>ISC</td><td>An ini encoder/decoder for node</tr>
<tr><td>inherits</td><td>2.0.4</td><td>ISC</td><td>Browser-friendly inheritance fully compatible with standard node.js inherits()</tr>
<tr><td><a href="https://github.com/isaacs/inflight" target="_blank">inflight</a></td><td>1.0.6</td><td>ISC</td><td>Add callbacks to requests in flight to avoid async duplication</tr>
<tr><td>import-lazy</td><td>2.1.0</td><td>MIT</td><td>Import modules lazily</tr>
<tr><td><a href="https://github.com/jensyt/imurmurhash-js" target="_blank">imurmurhash</a></td><td>0.1.4</td><td>MIT</td><td>An incremental implementation of MurmurHash3</tr>
<tr><td>import-fresh</td><td>3.3.0</td><td>MIT</td><td>Import a module while bypassing the cache</tr>
<tr><td><a href="https://facebook.github.com/immutable-js" target="_blank">immutable</a></td><td>3.8.2</td><td>MIT</td><td>Immutable Data Collections</tr>
<tr><td>immediate</td><td>3.0.6</td><td>MIT</td><td>A cross browser microtask library</tr>
<tr><td>ignore</td><td>5.3.2</td><td>MIT</td><td>Ignore is a manager and filter for .gitignore rules, the one used by eslint, gitbook and many others.</tr>
<tr><td>ieee754</td><td>1.2.1</td><td>BSD-3-Clause</td><td>Read/write IEEE754 floating point numbers from/to a Buffer or array-like object</tr>
<tr><td>https-proxy-agent</td><td>5.0.1</td><td>MIT</td><td>An HTTP(s) proxy `http.Agent` implementation for HTTPS</tr>
<tr><td>http-server</td><td>14.1.1</td><td>MIT</td><td>A simple zero-configuration command-line http server</tr>
<tr><td><a href="https://github.com/ashtuchkin/iconv-lite" target="_blank">iconv-lite</a></td><td>0.4.24</td><td>MIT</td><td>Convert character encodings in pure javascript.</tr>
<tr><td>http-response-object</td><td>3.0.2</td><td>MIT</td><td>A simple object to represent an http response</tr>
<tr><td>http-errors</td><td>2.0.0</td><td>MIT</td><td>Create HTTP error objects</tr>
<tr><td>http-proxy</td><td>1.18.1</td><td>MIT</td><td>HTTP proxying for the masses</tr>
<tr><td>http-cache-semantics</td><td>3.8.1</td><td>BSD-2-Clause</td><td>Parses Cache-Control and other headers. Helps building correct HTTP caches and proxies</tr>
<tr><td>html-encoding-sniffer</td><td>3.0.0</td><td>MIT</td><td>Sniff the encoding from a HTML byte stream</tr>
<tr><td>hexoid</td><td>1.0.0</td><td>MIT</td><td>A tiny (190B) and extremely fast utility to generate random IDs of fixed length</tr>
<tr><td><a href="https://helmetjs.github.io/" target="_blank">helmet</a></td><td>6.2.0</td><td>MIT</td><td>help secure Express/Connect apps with various HTTP headers</tr>
<tr><td><a href="https://highlightjs.org/" target="_blank">highlight.js</a></td><td>10.7.3</td><td>BSD-3-Clause</td><td>Syntax highlighting with language autodetection.</tr>
<tr><td><a href="https://mths.be/he" target="_blank">he</a></td><td>1.2.0</td><td>MIT</td><td>A robust HTML entities encoder/decoder with full Unicode support.</tr>
<tr><td>hbs</td><td>4.2.0</td><td>MIT</td><td>Express.js template engine plugin for Handlebars</tr>
<tr><td>hastscript</td><td>6.0.0</td><td>MIT</td><td>hast utility to create trees</tr>
<tr><td>hast-util-parse-selector</td><td>2.2.5</td><td>MIT</td><td>hast utility to create an element from a simple CSS selector</tr>
<tr><td><a href="https://github.com/inspect-js/hasOwn#readme" target="_blank">hasown</a></td><td>2.0.2</td><td>MIT</td><td>A robust, ES3 compatible, "has own property" predicate.</tr>
<tr><td><a href="https://github.com/inspect-js/has-tostringtag#readme" target="_blank">has-tostringtag</a></td><td>1.0.2</td><td>MIT</td><td>Determine if the JS environment has `Symbol.toStringTag` support. Supports spec, or shams.</tr>
<tr><td>has-yarn</td><td>2.1.0</td><td>MIT</td><td>Check if a project is using Yarn</tr>
<tr><td><a href="https://github.com/Xotic750/has-to-string-tag-x" target="_blank">has-to-string-tag-x</a></td><td>1.4.1</td><td>MIT</td><td>Tests if ES6 @@toStringTag is supported.</tr>
<tr><td><a href="https://github.com/ljharb/has-symbols#readme" target="_blank">has-symbols</a></td><td>1.0.3</td><td>MIT</td><td>Determine if the JS environment has Symbol support. Supports spec, or shams.</tr>
<tr><td><a href="https://github.com/inspect-js/has-proto#readme" target="_blank">has-proto</a></td><td>1.0.3</td><td>MIT</td><td>Does this environment have the ability to get the [[Prototype]] of an object on creation with `__proto__`?</tr>
<tr><td><a href="https://github.com/Xotic750/has-symbol-support-x" target="_blank">has-symbol-support-x</a></td><td>1.4.2</td><td>MIT</td><td>Tests if ES6 Symbol is supported.</tr>
<tr><td>has-flag</td><td>4.0.0</td><td>MIT</td><td>Check if argv has a specific flag</tr>
<tr><td><a href="https://github.com/inspect-js/has-property-descriptors#readme" target="_blank">has-property-descriptors</a></td><td>1.0.2</td><td>MIT</td><td>Does the environment have full property descriptor support? Handles IE 8's broken defineProperty/gOPD.</tr>
<tr><td><a href="https://github.com/ljharb/has-bigints#readme" target="_blank">has-bigints</a></td><td>1.0.2</td><td>MIT</td><td>Determine if the JS environment has BigInt support.</tr>
<tr><td>has-ansi</td><td>2.0.0</td><td>MIT</td><td>Check if a string has ANSI escape codes</tr>
<tr><td><a href="https://github.com/flmnt/graphemer" target="_blank">graphemer</a></td><td>1.4.0</td><td>MIT</td><td>A JavaScript library that breaks strings into their individual user-perceived characters (including emojis!)</tr>
<tr><td><a href="https://www.handlebarsjs.com/" target="_blank">handlebars</a></td><td>4.7.8</td><td>MIT</td><td>Handlebars provides the power necessary to let you build semantic templates effectively with no frustration</tr>
<tr><td>graceful-fs</td><td>4.2.11</td><td>ISC</td><td>A drop-in replacement for fs, making various improvements.</tr>
<tr><td>got</td><td>8.3.2</td><td>MIT</td><td>Simplified HTTP requests</tr>
<tr><td><a href="https://github.com/ljharb/gopd#readme" target="_blank">gopd</a></td><td>1.0.1</td><td>MIT</td><td>`Object.getOwnPropertyDescriptor`, but accounts for IE's broken implementation.</tr>
<tr><td>globalthis</td><td>1.0.4</td><td>MIT</td><td>ECMAScript spec-compliant polyfill/shim for `globalThis`</tr>
<tr><td>globs</td><td>0.1.4</td><td>MIT</td><td>An extension of glob, allowing you to provide one or more patterns to match.</tr>
<tr><td>globals</td><td>11.12.0</td><td>MIT</td><td>Global identifiers from different JavaScript environments</tr>
<tr><td>global-dirs</td><td>2.1.0</td><td>MIT</td><td>Get the directory of globally installed packages and binaries</tr>
<tr><td>glob-parent</td><td>6.0.2</td><td>ISC</td><td>Extract the non-magic parent path from a glob string.</tr>
<tr><td>glob</td><td>11.0.0</td><td>ISC</td><td>the most correct and second fastest glob implementation in JavaScript</tr>
<tr><td><a href="https://github.com/substack/github-from-package" target="_blank">github-from-package</a></td><td>0.0.0</td><td>MIT</td><td>return the github url from a package.json file</tr>
<tr><td>get-stream</td><td>2.3.1</td><td>MIT</td><td>Get a stream as a string, buffer, or array</tr>
<tr><td><a href="https://github.com/inspect-js/get-symbol-description#readme" target="_blank">get-symbol-description</a></td><td>1.0.2</td><td>MIT</td><td>Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.</tr>
<tr><td>get-stdin</td><td>8.0.0</td><td>MIT</td><td>Get stdin as a string or buffer</tr>
<tr><td>get-port</td><td>5.1.1</td><td>MIT</td><td>Get an available port</tr>
<tr><td>get-proxy</td><td>2.1.0</td><td>MIT</td><td>Get configured proxy</tr>
<tr><td><a href="https://github.com/ljharb/get-intrinsic#readme" target="_blank">get-intrinsic</a></td><td>1.2.4</td><td>MIT</td><td>Get and robustly cache all JS language-level intrinsics at first require time</tr>
<tr><td><a href="https://github.com/loganfsmyth/gensync" target="_blank">gensync</a></td><td>1.0.0-beta.2</td><td>MIT</td><td>Allows users to use generators in order to write common functions that can be both sync or async.</tr>
<tr><td><a href="https://github.com/stefanpenner/get-caller-file#readme" target="_blank">get-caller-file</a></td><td>2.0.5</td><td>ISC</td><td></tr>
<tr><td><a href="https://github.com/inspect-js/functions-have-names#readme" target="_blank">functions-have-names</a></td><td>1.2.3</td><td>MIT</td><td>Does this JS environment support the `name` property on functions?</tr>
<tr><td>function.prototype.name</td><td>1.1.6</td><td>MIT</td><td>An ES2015 spec-compliant `Function.prototype.name` shim</tr>
<tr><td><a href="https://github.com/Raynos/function-bind" target="_blank">function-bind</a></td><td>1.1.2</td><td>MIT</td><td>Implementation of Function.prototype.bind</tr>
<tr><td>fs.realpath</td><td>1.0.0</td><td>ISC</td><td>Use node's fs.realpath, but fall back to the JS implementation if the native one fails</tr>
<tr><td><a href="https://github.com/jprichardson/node-fs-extra" target="_blank">fs-extra</a></td><td>11.2.0</td><td>MIT</td><td>fs-extra contains methods that aren't included in the vanilla Node.js fs package. Such as recursive mkdir, copy, and remove.</tr>
<tr><td><a href="https://github.com/mafintosh/fs-constants" target="_blank">fs-constants</a></td><td>1.0.0</td><td>MIT</td><td>Require constants across node and the browser</tr>
<tr><td><a href="https://github.com/hughsk/from2" target="_blank">from2</a></td><td>2.3.0</td><td>MIT</td><td>Convenience wrapper for ReadableStream, with an API lifted from "from" and "through2"</tr>
<tr><td>fresh</td><td>0.5.2</td><td>MIT</td><td>HTTP response freshness testing</tr>
<tr><td>forwarded</td><td>0.2.0</td><td>MIT</td><td>Parse HTTP X-Forwarded-For header</tr>
<tr><td><a href="https://github.com/node-formidable/formidable" target="_blank">formidable</a></td><td>3.5.1</td><td>MIT</td><td>A node.js module for parsing form data, especially file uploads.</tr>
<tr><td>form-data</td><td>4.0.0</td><td>MIT</td><td>A library to create readable "multipart/form-data" streams. Can be used to submit forms and file uploads to other web applications.</tr>
<tr><td><a href="https://github.com/jimmywarting/FormData#readme" target="_blank">formdata-polyfill</a></td><td>4.0.10</td><td>MIT</td><td>HTML5 `FormData` for Browsers and Node.</tr>
<tr><td><a href="https://github.com/FuturesJS/forEachAsync" target="_blank">foreachasync</a></td><td>3.0.0</td><td>Apache2</td><td>A node- and browser-ready async counterpart of Array.prototype.forEach</tr>
<tr><td><a href="http://samhuri.net/proj/format" target="_blank">format</a></td><td>0.2.2</td><td>undefined</td><td>printf, sprintf, and vsprintf for JavaScript</tr>
<tr><td>foreground-child</td><td>3.3.0</td><td>ISC</td><td>Run a child as if it's the foreground process. Give it stdio. Exit when it exits.</tr>
<tr><td><a href="https://github.com/Raynos/for-each" target="_blank">for-each</a></td><td>0.3.3</td><td>MIT</td><td>A better forEach</tr>
<tr><td><a href="https://github.com/follow-redirects/follow-redirects" target="_blank">follow-redirects</a></td><td>1.15.9</td><td>MIT</td><td>HTTP and HTTPS modules that follow redirects.</tr>
<tr><td><a href="https://github.com/WebReflection/flatted#readme" target="_blank">flatted</a></td><td>3.3.1</td><td>ISC</td><td>A super light and fast circular JSON parser.</tr>
<tr><td>fluent-ffmpeg</td><td>2.1.3</td><td>MIT</td><td>A fluent API to FFMPEG (http://www.ffmpeg.org)</tr>
<tr><td>flat-cache</td><td>3.2.0</td><td>MIT</td><td>A stupidly simple key/value storage using files to persist some data</tr>
<tr><td><a href="https://github.com/hughsk/flat" target="_blank">flat</a></td><td>5.0.2</td><td>BSD-3-Clause</td><td>Take a nested Javascript object and flatten it, or unflatten an object with delimited keys</tr>
<tr><td>find-up</td><td>6.3.0</td><td>MIT</td><td>Find a file or directory by walking up parent directories</tr>
<tr><td>finalhandler</td><td>1.1.2</td><td>MIT</td><td>Node.js final http responder</tr>
<tr><td>filenamify</td><td>2.1.0</td><td>MIT</td><td>Convert a string to a valid safe filename</tr>
<tr><td>filename-reserved-regex</td><td>2.0.0</td><td>MIT</td><td>Regular expression for matching reserved filename characters</tr>
<tr><td>file-type</td><td>18.7.0</td><td>MIT</td><td>Detect the file type of a Buffer/Uint8Array/ArrayBuffer</tr>
<tr><td><a href="https://github.com/jonschlinkert/fill-range" target="_blank">fill-range</a></td><td>7.1.1</td><td>MIT</td><td>Fill in a range of numbers or letters, optionally passing an increment or `step` to use, or create a regex-compatible range with `options.toRegex`</tr>
<tr><td>file-entry-cache</td><td>6.0.1</td><td>MIT</td><td>Super simple cache for file metadata, useful for process that work o a given series of files and that only need to repeat the job on the changed ones since the previous run of the process</tr>
<tr><td>figures</td><td>3.2.0</td><td>MIT</td><td>Unicode symbols with Windows CMD fallbacks</tr>
<tr><td>figlet</td><td>1.7.0</td><td>MIT</td><td>Creates ASCII Art from text. A full implementation of the FIGfont spec.</tr>
<tr><td>ffprobe-static</td><td>3.1.0</td><td>MIT</td><td>Static binaries for ffprobe.</tr>
<tr><td>ffmpeg-static</td><td>4.4.1</td><td>GPL-3.0-or-later</td><td>ffmpeg static binaries for Mac OSX and Linux and Windows</tr>
<tr><td><a href="https://github.com/node-fetch/fetch-blob#readme" target="_blank">fetch-blob</a></td><td>3.2.0</td><td>MIT</td><td>Blob & File implementation in Node.js, originally from node-fetch.</tr>
<tr><td>fault</td><td>1.0.4</td><td>MIT</td><td>Functional errors with formatted output</tr>
<tr><td>fd-slicer</td><td>1.1.0</td><td>MIT</td><td>safely create multiple ReadStream or WriteStream objects from the same file descriptor</tr>
<tr><td>fast-xml-parser</td><td>4.4.1</td><td>MIT</td><td>Validate XML, Parse XML, Build XML without C/C++ based libraries</tr>
<tr><td><a href="https://github.com/mcollina/fastq#readme" target="_blank">fastq</a></td><td>1.17.1</td><td>ISC</td><td>Fast, in memory work queue</tr>
<tr><td><a href="https://github.com/fastify/fast-uri" target="_blank">fast-uri</a></td><td>3.0.2</td><td>MIT</td><td>Dependency free RFC 3986 URI toolbox</tr>
<tr><td>fast-levenshtein</td><td>2.0.6</td><td>MIT</td><td>Efficient implementation of Levenshtein algorithm  with locale-specific collator support.</tr>
<tr><td><a href="https://github.com/epoberezkin/fast-json-stable-stringify" target="_blank">fast-json-stable-stringify</a></td><td>2.1.0</td><td>MIT</td><td>deterministic `JSON.stringify()` - a faster version of substack's json-stable-strigify without jsonify</tr>
<tr><td><a href="https://github.com/Starcounter-Jack/JSON-Patch" target="_blank">fast-json-patch</a></td><td>3.1.1</td><td>MIT</td><td>Fast implementation of JSON-Patch (RFC-6902) with duplex (observe changes) capabilities</tr>
<tr><td><a href="https://github.com/mrkmg/node-external-editor#readme" target="_blank">external-editor</a></td><td>3.1.0</td><td>MIT</td><td>Edit a string with the users preferred text editor using $VISUAL or $ENVIRONMENT</tr>
<tr><td><a href="https://github.com/epoberezkin/fast-deep-equal#readme" target="_blank">fast-deep-equal</a></td><td>3.1.3</td><td>MIT</td><td>Fast deep equal</tr>
<tr><td>extend</td><td>3.0.2</td><td>MIT</td><td>Port of jQuery.extend for node.js and the browser</tr>
<tr><td>ext-name</td><td>5.0.0</td><td>MIT</td><td>Get the file extension and MIME type from a file</tr>
<tr><td>ext-list</td><td>2.2.2</td><td>MIT</td><td>List of known file extensions and their MIME types</tr>
<tr><td>express-session</td><td>1.17.2</td><td>MIT</td><td>Simple session middleware for Express</tr>
<tr><td><a href="http://expressjs.com/" target="_blank">express</a></td><td>4.21.0</td><td>MIT</td><td>Fast, unopinionated, minimalist web framework</tr>
<tr><td><a href="https://github.com/ralphtheninja/expand-template" target="_blank">expand-template</a></td><td>2.0.3</td><td>(MIT OR WTFPL)</td><td>Expand placeholders in a template string</tr>
<tr><td>eventemitter3</td><td>4.0.7</td><td>MIT</td><td>EventEmitter3 focuses on performance while maintaining a Node.js AND browser compatible interface.</tr>
<tr><td>etag</td><td>1.8.1</td><td>MIT</td><td>Create simple HTTP ETags</tr>
<tr><td><a href="https://github.com/estools/estraverse" target="_blank">estraverse</a></td><td>5.3.0</td><td>BSD-2-Clause</td><td>ECMAScript JS AST traversal functions</tr>
<tr><td><a href="https://github.com/estools/esutils" target="_blank">esutils</a></td><td>2.0.3</td><td>BSD-2-Clause</td><td>utility box for ECMAScript language tools</tr>
<tr><td><a href="https://github.com/estools/esrecurse" target="_blank">esrecurse</a></td><td>4.3.0</td><td>BSD-2-Clause</td><td>ECMAScript AST recursive visitor</tr>
<tr><td><a href="https://github.com/estools/esquery/" target="_blank">esquery</a></td><td>1.6.0</td><td>BSD-3-Clause</td><td>A query library for ECMAScript AST using a CSS selector like query language.</tr>
<tr><td><a href="https://github.com/eslint/espree" target="_blank">espree</a></td><td>9.6.1</td><td>BSD-2-Clause</td><td>An Esprima-compatible JavaScript parser built on Acorn</tr>
<tr><td><a href="https://github.com/eslint/eslint-visitor-keys#readme" target="_blank">eslint-visitor-keys</a></td><td>3.4.3</td><td>Apache-2.0</td><td>Constants and utilities about visitor keys to traverse AST.</tr>
<tr><td><a href="https://github.com/mysticatea/eslint-utils#readme" target="_blank">eslint-utils</a></td><td>3.0.0</td><td>MIT</td><td>Utilities for ESLint plugins.</tr>
<tr><td><a href="http://github.com/eslint/eslint-scope" target="_blank">eslint-scope</a></td><td>7.2.2</td><td>BSD-2-Clause</td><td>ECMAScript scope analyzer for ESLint</tr>
<tr><td><a href="https://github.com/jsx-eslint/eslint-plugin-react" target="_blank">eslint-plugin-react</a></td><td>7.37.1</td><td>MIT</td><td>React specific linting rules for ESLint</tr>
<tr><td><a href="https://github.com/eslint-community/eslint-plugin-promise" target="_blank">eslint-plugin-promise</a></td><td>6.6.0</td><td>ISC</td><td>Enforce best practices for JavaScript promises</tr>
<tr><td><a href="https://github.com/eslint-community/eslint-plugin-n#readme" target="_blank">eslint-plugin-n</a></td><td>15.7.0</td><td>MIT</td><td>Additional ESLint's rules for Node.js</tr>
<tr><td><a href="https://github.com/import-js/eslint-plugin-import" target="_blank">eslint-plugin-import</a></td><td>2.31.0</td><td>MIT</td><td>Import with sanity.</tr>
<tr><td><a href="https://github.com/mysticatea/eslint-plugin-es#readme" target="_blank">eslint-plugin-es</a></td><td>4.1.0</td><td>MIT</td><td>ESLint plugin about ECMAScript syntactic features.</tr>
<tr><td><a href="https://github.com/import-js/eslint-plugin-import#readme" target="_blank">eslint-module-utils</a></td><td>2.12.0</td><td>MIT</td><td>Core utilities to support eslint-plugin-import and other module-related plugins.</tr>
<tr><td><a href="https://github.com/standard/eslint-config-standard-jsx" target="_blank">eslint-config-standard-jsx</a></td><td>11.0.0</td><td>MIT</td><td>JavaScript Standard Style JSX support - ESLint Shareable Config</tr>
<tr><td><a href="https://github.com/standard/eslint-config-standard" target="_blank">eslint-config-standard</a></td><td>17.1.0</td><td>MIT</td><td>JavaScript Standard Style - ESLint Shareable Config</tr>
<tr><td><a href="https://github.com/import-js/eslint-plugin-import" target="_blank">eslint-import-resolver-node</a></td><td>0.3.9</td><td>MIT</td><td>Node default behavior import resolution plugin for eslint-plugin-import.</tr>
<tr><td><a href="https://eslint.org" target="_blank">eslint</a></td><td>8.57.1</td><td>MIT</td><td>An AST-based pattern checker for JavaScript.</tr>
<tr><td>escape-string-regexp</td><td>4.0.0</td><td>MIT</td><td>Escape RegExp special characters</tr>
<tr><td>escape-html</td><td>1.0.3</td><td>MIT</td><td>Escape string for use in HTML</tr>
<tr><td>escape-goat</td><td>2.1.1</td><td>MIT</td><td>Escape a string for use in HTML or the inverse</tr>
<tr><td>escalade</td><td>3.2.0</td><td>MIT</td><td>A tiny (183B to 210B) and fast utility to ascend parent directories</tr>
<tr><td>es-to-primitive</td><td>1.2.1</td><td>MIT</td><td>ECMAScript “ToPrimitive” algorithm. Provides ES5 and ES2015 versions.</tr>
<tr><td><a href="https://github.com/ljharb/es-shim-unscopables#readme" target="_blank">es-shim-unscopables</a></td><td>1.0.2</td><td>MIT</td><td>Helper package to shim a method into `Array.prototype[Symbol.unscopables]`</tr>
<tr><td><a href="https://github.com/es-shims/es-set-tostringtag#readme" target="_blank">es-set-tostringtag</a></td><td>2.0.3</td><td>MIT</td><td>A helper to optimistically set Symbol.toStringTag, when possible.</tr>
<tr><td><a href="https://github.com/ljharb/es-object-atoms#readme" target="_blank">es-object-atoms</a></td><td>1.0.0</td><td>MIT</td><td>ES Object-related atoms: Object, ToObject, RequireObjectCoercible</tr>
<tr><td><a href="https://github.com/es-shims/iterator-helpers#readme" target="_blank">es-iterator-helpers</a></td><td>1.0.19</td><td>MIT</td><td>An ESnext spec-compliant iterator helpers shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td><a href="https://github.com/ljharb/es-errors#readme" target="_blank">es-errors</a></td><td>1.3.0</td><td>MIT</td><td>A simple cache for a few of the JS Error constructors.</tr>
<tr><td><a href="https://github.com/ljharb/es-define-property#readme" target="_blank">es-define-property</a></td><td>1.0.0</td><td>MIT</td><td>`Object.defineProperty`, but not IE 8's broken one.</tr>
<tr><td>errno</td><td>0.1.8</td><td>MIT</td><td>libuv errno details exposed</tr>
<tr><td>es-abstract</td><td>1.23.3</td><td>MIT</td><td>ECMAScript spec abstract operations.</tr>
<tr><td>error-ex</td><td>1.3.2</td><td>MIT</td><td>Easy error subclassing and stack customization</tr>
<tr><td>env-paths</td><td>2.2.1</td><td>MIT</td><td>Get paths for storing things like data, config, cache, etc</tr>
<tr><td>entities</td><td>4.5.0</td><td>BSD-2-Clause</td><td>Encode & decode XML and HTML entities with ease & speed</tr>
<tr><td><a href="https://github.com/enquirer/enquirer" target="_blank">enquirer</a></td><td>2.4.1</td><td>MIT</td><td>Stylish, intuitive and user-friendly prompt system. Fast and lightweight enough for small projects, powerful and extensible enough for the most advanced use cases.</tr>
<tr><td><a href="https://github.com/mafintosh/end-of-stream" target="_blank">end-of-stream</a></td><td>1.4.4</td><td>MIT</td><td>Call a callback when a readable/writable/duplex stream has completed or failed.</tr>
<tr><td>encodeurl</td><td>2.0.0</td><td>MIT</td><td>Encode a URL to a percent-encoded form, excluding already-encoded sequences</tr>
<tr><td><a href="https://mths.be/emoji-regex" target="_blank">emoji-regex</a></td><td>8.0.0</td><td>MIT</td><td>A regular expression to match all Emoji-only symbols as per the Unicode Standard.</tr>
<tr><td>electron-to-chromium</td><td>1.5.32</td><td>ISC</td><td>Provides a list of electron-to-chromium version mappings</tr>
<tr><td>ee-first</td><td>1.1.1</td><td>MIT</td><td>return the first event in a set of ee/event pairs</tr>
<tr><td>eastasianwidth</td><td>0.2.0</td><td>MIT</td><td>Get East Asian Width from a character.</tr>
<tr><td><a href="https://github.com/Brightspace/node-ecdsa-sig-formatter#readme" target="_blank">ecdsa-sig-formatter</a></td><td>1.0.11</td><td>Apache-2.0</td><td>Translate ECDSA signatures between ASN.1/DER and JOSE-style concatenation</tr>
<tr><td>duplexer3</td><td>0.1.5</td><td>BSD-3-Clause</td><td>Like duplexer but using streams3</tr>
<tr><td>drange</td><td>1.1.1</td><td>MIT</td><td>For adding, subtracting, and indexing discontinuous ranges of numbers</tr>
<tr><td>download</td><td>7.1.0</td><td>MIT</td><td>Download and extract files</tr>
<tr><td>dot-prop</td><td>5.3.0</td><td>MIT</td><td>Get, set, or delete a property from a nested object using a dot path</tr>
<tr><td><a href="https://github.com/cure53/DOMPurify" target="_blank">dompurify</a></td><td>3.1.4</td><td>(MPL-2.0 OR Apache-2.0)</td><td>DOMPurify is a DOM-only, super-fast, uber-tolerant XSS sanitizer for HTML, MathML and SVG. It's written in JavaScript and works in all modern browsers (Safari, Opera (15+), Internet Explorer (10+), Firefox and Chrome - as well as almost anything else using Blink or WebKit). DOMPurify is written by security people who have vast background in web attacks and XSS. Fear not.</tr>
<tr><td><a href="https://github.com/eslint/doctrine" target="_blank">doctrine</a></td><td>3.0.0</td><td>Apache-2.0</td><td>JSDoc parser</tr>
<tr><td><a href="https://docsify.js.org" target="_blank">docsify-server-renderer</a></td><td>4.13.1</td><td>MIT</td><td>docsify server renderer</tr>
<tr><td><a href="https://github.com/docsifyjs/docsify-cli#readme" target="_blank">docsify-cli</a></td><td>4.4.4</td><td>MIT</td><td>A magical documentation generator.</tr>
<tr><td><a href="https://docsify.js.org" target="_blank">docsify</a></td><td>4.13.1</td><td>MIT</td><td>A magical documentation generator.</tr>
<tr><td>docdash</td><td>2.0.2</td><td>Apache-2.0</td><td>A clean, responsive documentation template theme for JSDoc 3 inspired by lodash and minami</tr>
<tr><td>detect-libc</td><td>2.0.3</td><td>Apache-2.0</td><td>Node.js module to detect the C standard library (libc) implementation family and version</tr>
<tr><td>diff</td><td>5.2.0</td><td>BSD-3-Clause</td><td>A JavaScript text diff implementation.</tr>
<tr><td><a href="https://github.com/npm/dezalgo" target="_blank">dezalgo</a></td><td>1.0.4</td><td>ISC</td><td>Contain async insanity so that the dark pony lord doesn't eat souls</tr>
<tr><td>destroy</td><td>1.2.0</td><td>MIT</td><td>destroy a stream if possible</tr>
<tr><td>depd</td><td>2.0.0</td><td>MIT</td><td>Deprecate all the things</tr>
<tr><td><a href="https://github.com/felixge/node-delayed-stream" target="_blank">delayed-stream</a></td><td>1.0.0</td><td>MIT</td><td>Buffers events from a stream until you are ready to handle them.</tr>
<tr><td><a href="https://github.com/ljharb/define-data-property#readme" target="_blank">define-data-property</a></td><td>1.1.4</td><td>MIT</td><td>Define a data property on an object. Will fall back to assignment in an engine without descriptors.</tr>
<tr><td>define-properties</td><td>1.2.1</td><td>MIT</td><td>Define multiple non-enumerable properties at once. Uses `Object.defineProperty` when available; falls back to standard assignment in older engines.</tr>
<tr><td><a href="https://github.com/szmarczak/defer-to-connect#readme" target="_blank">defer-to-connect</a></td><td>1.1.3</td><td>MIT</td><td>The safe way to handle the `connect` socket event</tr>
<tr><td>deep-is</td><td>0.1.4</td><td>MIT</td><td>node's assert.deepEqual algorithm except for NaN being equal to NaN</tr>
<tr><td><a href="https://github.com/unclechu/node-deep-extend" target="_blank">deep-extend</a></td><td>0.6.0</td><td>MIT</td><td>Recursive object extending</tr>
<tr><td><a href="https://github.com/TehShrike/deepmerge" target="_blank">deepmerge</a></td><td>4.3.1</td><td>MIT</td><td>A library for deep (recursive) merging of Javascript objects</tr>
<tr><td>decompress-targz</td><td>4.1.1</td><td>MIT</td><td>decompress tar.gz plugin</tr>
<tr><td>decompress-unzip</td><td>4.0.1</td><td>MIT</td><td>decompress zip plugin</tr>
<tr><td>decompress-tarbz2</td><td>4.1.1</td><td>MIT</td><td>decompress tar.bz2 plugin</tr>
<tr><td>decompress-tar</td><td>4.1.1</td><td>MIT</td><td>decompress tar plugin</tr>
<tr><td>decompress-response</td><td>3.3.0</td><td>MIT</td><td>Decompress a HTTP response if needed</tr>
<tr><td>decamelize</td><td>1.2.0</td><td>MIT</td><td>Convert a camelized string into a lowercased one with a custom separator: unicornRainbow → unicorn_rainbow</tr>
<tr><td>decompress</td><td>4.2.1</td><td>MIT</td><td>Extracting archives made easy</tr>
<tr><td>debug</td><td>4.3.7</td><td>MIT</td><td>Lightweight debugging utility for Node.js and the browser</tr>
<tr><td>decode-uri-component</td><td>0.2.2</td><td>MIT</td><td>A better decodeURIComponent</tr>
<tr><td>date-fns</td><td>2.30.0</td><td>MIT</td><td>Modern JavaScript date utility library</tr>
<tr><td><a href="https://github.com/ljharb/data-view-byte-offset#readme" target="_blank">data-view-byte-offset</a></td><td>1.0.0</td><td>MIT</td><td>Get the byteOffset out of a DataView, robustly.</tr>
<tr><td><a href="https://github.com/ljharb/data-view-byte-length#readme" target="_blank">data-view-byte-length</a></td><td>1.0.1</td><td>MIT</td><td>Get the byteLength out of a DataView, robustly.</tr>
<tr><td><a href="https://github.com/ljharb/data-view-buffer#readme" target="_blank">data-view-buffer</a></td><td>1.0.1</td><td>MIT</td><td>Get the ArrayBuffer out of a DataView, robustly.</tr>
<tr><td><a href="https://github.com/TooTallNate/node-data-uri-to-buffer" target="_blank">data-uri-to-buffer</a></td><td>4.0.1</td><td>MIT</td><td>Generate a Buffer instance from a Data URI string</tr>
<tr><td><a href="https://github.com/leizongmin/js-css-filter" target="_blank">cssfilter</a></td><td>0.0.10</td><td>MIT</td><td>Sanitize untrusted CSS with a configuration specified by a Whitelist. 根据白名单过滤CSS</tr>
<tr><td>crypto-random-string</td><td>2.0.0</td><td>MIT</td><td>Generate a cryptographically strong random string</tr>
<tr><td><a href="https://mths.be/cssescape" target="_blank">css.escape</a></td><td>1.5.1</td><td>MIT</td><td>A robust polyfill for the `CSS.escape` utility method as defined in CSSOM.</tr>
<tr><td><a href="https://github.com/moxystudio/node-cross-spawn" target="_blank">cross-spawn</a></td><td>7.0.3</td><td>MIT</td><td>Cross platform child_process#spawn and child_process#spawnSync</tr>
<tr><td>core-util-is</td><td>1.0.3</td><td>MIT</td><td>The `util.is*` functions introduced in Node v0.12.</tr>
<tr><td>cp-file</td><td>7.0.0</td><td>MIT</td><td>Copy a file</tr>
<tr><td>corser</td><td>2.0.1</td><td>MIT</td><td>A highly configurable, middleware compatible implementation of CORS.</tr>
<tr><td>core-js-pure</td><td>3.38.1</td><td>MIT</td><td>Standard library</tr>
<tr><td>copy-to-clipboard</td><td>3.3.3</td><td>MIT</td><td>Copy stuff into clipboard using JS with fallbacks</tr>
<tr><td>core-js-compat</td><td>3.38.1</td><td>MIT</td><td>core-js compat</tr>
<tr><td><a href="https://github.com/mesqueeb/copy-anything#readme" target="_blank">copy-anything</a></td><td>2.0.6</td><td>MIT</td><td>An optimised way to copy'ing an object. A small and simple integration</tr>
<tr><td>cookiejar</td><td>2.1.4</td><td>MIT</td><td>simple persistent cookiejar system</tr>
<tr><td>cookie-signature</td><td>1.0.6</td><td>MIT</td><td>Sign and unsign cookies</tr>
<tr><td>cookie</td><td>0.6.0</td><td>MIT</td><td>HTTP server cookie parsing and serialization</tr>
<tr><td><a href="https://github.com/thlorenz/convert-source-map" target="_blank">convert-source-map</a></td><td>2.0.0</td><td>MIT</td><td>Converts a source-map from/to  different formats and allows adding/changing properties.</tr>
<tr><td>content-type</td><td>1.0.5</td><td>MIT</td><td>Create and parse HTTP Content-Type header</tr>
<tr><td>content-disposition</td><td>0.5.4</td><td>MIT</td><td>Create and parse Content-Disposition header</tr>
<tr><td>connect-livereload</td><td>0.6.1</td><td>MIT</td><td>connect middleware for adding the livereload script to the response</tr>
<tr><td>connect-history-api-fallback</td><td>1.6.0</td><td>MIT</td><td>Provides a fallback for non-existing directories so that the HTML 5 history API can be used.</tr>
<tr><td>connect</td><td>3.7.0</td><td>MIT</td><td>High performance middleware framework</tr>
<tr><td><a href="http://github.com/dominictarr/config-chain" target="_blank">config-chain</a></td><td>1.1.13</td><td>MIT</td><td>HANDLE CONFIGURATION ONCE AND FOR ALL</tr>
<tr><td>concat-stream</td><td>2.0.0</td><td>MIT</td><td>writable stream that concatenates strings or binary data and calls a callback with the result</tr>
<tr><td>configstore</td><td>5.0.1</td><td>BSD-2-Clause</td><td>Easily load and save config without having to think about where and how</tr>
<tr><td>concat-map</td><td>0.0.1</td><td>MIT</td><td>concatenative mapdashery</tr>
<tr><td>compression</td><td>1.7.4</td><td>MIT</td><td>Node.js compression middleware</tr>
<tr><td>compressible</td><td>2.0.18</td><td>MIT</td><td>Compressible Content-Type / mime checking</tr>
<tr><td>component-emitter</td><td>1.3.1</td><td>MIT</td><td>Event emitter</tr>
<tr><td><a href="https://github.com/syavorsky/comment-parser" target="_blank">comment-parser</a></td><td>1.4.1</td><td>MIT</td><td>Generic JSDoc-like comment parser</tr>
<tr><td>commander</td><td>11.1.0</td><td>MIT</td><td>the complete solution for node.js command-line programs</tr>
<tr><td>comma-separated-tokens</td><td>1.0.8</td><td>MIT</td><td>Parse and stringify comma-separated tokens</tr>
<tr><td><a href="https://github.com/colorjs/color-name" target="_blank">color-name</a></td><td>1.1.4</td><td>MIT</td><td>A list of color names and its values</tr>
<tr><td><a href="https://github.com/felixge/node-combined-stream" target="_blank">combined-stream</a></td><td>1.0.8</td><td>MIT</td><td>A stream that emits multiple other streams one after another.</tr>
<tr><td>color-convert</td><td>2.0.1</td><td>MIT</td><td>Plain color conversion functions</tr>
<tr><td><a href="https://github.com/lukechilds/clone-response" target="_blank">clone-response</a></td><td>1.0.2</td><td>MIT</td><td>Clone a Node.js HTTP response stream</tr>
<tr><td>cliui</td><td>6.0.0</td><td>ISC</td><td>easily create complex multi-column command-line-interfaces</tr>
<tr><td><a href="https://github.com/knownasilya/cli-width" target="_blank">cli-width</a></td><td>3.0.0</td><td>ISC</td><td>Get stdout window width, with two fallbacks, tty and then a default.</tr>
<tr><td>cli-cursor</td><td>3.1.0</td><td>MIT</td><td>Toggle the CLI cursor</tr>
<tr><td>cli-boxes</td><td>2.2.1</td><td>MIT</td><td>Boxes for use in the terminal</tr>
<tr><td>classnames</td><td>2.5.1</td><td>MIT</td><td>A simple utility for conditionally joining classNames together</tr>
<tr><td>chownr</td><td>1.1.4</td><td>ISC</td><td>like `chown -R`</tr>
<tr><td><a href="https://github.com/watson/ci-info" target="_blank">ci-info</a></td><td>2.0.0</td><td>MIT</td><td>Get details about the current Continuous Integration environment</tr>
<tr><td><a href="https://github.com/paulmillr/chokidar" target="_blank">chokidar</a></td><td>3.6.0</td><td>MIT</td><td>Minimal and efficient cross-platform file watching library</tr>
<tr><td>character-reference-invalid</td><td>1.1.4</td><td>MIT</td><td>HTML invalid numeric character reference information</tr>
<tr><td><a href="https://github.com/runk/node-chardet" target="_blank">chardet</a></td><td>0.7.0</td><td>MIT</td><td>Character detector</tr>
<tr><td>character-entities-legacy</td><td>1.1.4</td><td>MIT</td><td>HTML legacy character entity information</tr>
<tr><td>chalk</td><td>4.1.2</td><td>MIT</td><td>Terminal string styling done right</tr>
<tr><td>character-entities</td><td>1.2.4</td><td>MIT</td><td>HTML character entity information</tr>
<tr><td>caw</td><td>2.0.1</td><td>MIT</td><td>Construct HTTP/HTTPS agents for tunneling proxies</tr>
<tr><td>catharsis</td><td>0.9.0</td><td>MIT</td><td>A JavaScript parser for Google Closure Compiler and JSDoc type expressions.</tr>
<tr><td>caseless</td><td>0.12.0</td><td>Apache-2.0</td><td>Caseless object set/get/has, very useful when working with HTTP headers.</tr>
<tr><td>caniuse-lite</td><td>1.0.30001667</td><td>CC-BY-4.0</td><td>A smaller version of caniuse-db, with only the essentials!</tr>
<tr><td>camelcase</td><td>5.3.1</td><td>MIT</td><td>Convert a dash/dot/underscore/space separated string to camelCase or PascalCase: `foo-bar` → `fooBar`</tr>
<tr><td><a href="https://github.com/ljharb/call-bind#readme" target="_blank">call-bind</a></td><td>1.0.7</td><td>MIT</td><td>Robustly `.call.bind()` a function</tr>
<tr><td>callsites</td><td>3.1.0</td><td>MIT</td><td>Get callsites from the V8 stack trace API</tr>
<tr><td><a href="https://github.com/lukechilds/cacheable-request" target="_blank">cacheable-request</a></td><td>2.1.4</td><td>MIT</td><td>Wrap native HTTP requests with RFC compliant cache support</tr>
<tr><td>bytes</td><td>3.1.2</td><td>MIT</td><td>Utility to parse a string bytes to bytes and vice-versa</tr>
<tr><td>builtins</td><td>5.1.0</td><td>MIT</td><td>List of node.js builtin modules</tr>
<tr><td>buffer-from</td><td>1.1.2</td><td>MIT</td><td>undefined</tr>
<tr><td>buffer-fill</td><td>1.0.0</td><td>MIT</td><td>undefined</tr>
<tr><td><a href="https://github.com/brianloveswords/buffer-crc32" target="_blank">buffer-crc32</a></td><td>0.2.13</td><td>MIT</td><td>A pure javascript CRC32 algorithm that plays nice with binary data</tr>
<tr><td>buffer-equal-constant-time</td><td>1.0.1</td><td>BSD-3-Clause</td><td>Constant-time comparison of Buffers</tr>
<tr><td>buffer-alloc-unsafe</td><td>1.1.0</td><td>MIT</td><td>undefined</tr>
<tr><td><a href="https://github.com/feross/buffer" target="_blank">buffer</a></td><td>5.7.1</td><td>MIT</td><td>Node.js Buffer API, for the browser</tr>
<tr><td>bson</td><td>6.8.0</td><td>Apache-2.0</td><td>A bson parser for node.js and the browser</tr>
<tr><td>browserslist</td><td>4.24.0</td><td>MIT</td><td>Share target browsers between different front-end tools, like Autoprefixer, Stylelint and babel-env-preset</tr>
<tr><td>buffer-alloc</td><td>1.2.0</td><td>MIT</td><td>undefined</tr>
<tr><td>browser-stdout</td><td>1.3.1</td><td>ISC</td><td></tr>
<tr><td><a href="https://github.com/micromatch/braces" target="_blank">braces</a></td><td>3.0.3</td><td>MIT</td><td>Bash-like brace expansion, implemented in JavaScript. Safer than other brace expansion libs, with complete support for the Bash 4.3 braces specification, without sacrificing speed.</tr>
<tr><td><a href="https://github.com/juliangruber/brace-expansion" target="_blank">brace-expansion</a></td><td>1.1.11</td><td>MIT</td><td>Brace expansion as known from sh/bash</tr>
<tr><td>boxen</td><td>4.2.0</td><td>MIT</td><td>Create boxes in the terminal</tr>
<tr><td>bower-endpoint-parser</td><td>0.2.2</td><td>undefined</td><td>Little module that helps with endpoints parsing.</tr>
<tr><td><a href="https://github.com/lancedikson/bowser" target="_blank">bowser</a></td><td>2.11.0</td><td>MIT</td><td>Lightweight browser detector</tr>
<tr><td>body-parser</td><td>1.20.3</td><td>MIT</td><td>Node.js body parsing middleware</tr>
<tr><td><a href="https://github.com/indutny/bn.js" target="_blank">bn.js</a></td><td>4.12.0</td><td>MIT</td><td>Big number implementation in pure javascript</tr>
<tr><td><a href="http://bower.io" target="_blank">bower</a></td><td>1.8.14</td><td>MIT</td><td>The browser package manager</tr>
<tr><td><a href="https://github.com/petkaantonov/bluebird" target="_blank">bluebird</a></td><td>3.7.2</td><td>MIT</td><td>Full featured Promises/A+ implementation with exceptionally good performance</tr>
<tr><td><a href="https://github.com/rvagg/bl" target="_blank">bl</a></td><td>1.2.3</td><td>MIT</td><td>Buffer List: collect buffers and access with a standard readable Buffer interface, streamable too!</tr>
<tr><td>binary-extensions</td><td>2.3.0</td><td>MIT</td><td>List of binary file extensions</tr>
<tr><td>bcryptjs</td><td>2.4.3</td><td>MIT</td><td>Optimized bcrypt in plain JavaScript with zero dependencies. Compatible to 'bcrypt'.</tr>
<tr><td><a href="https://github.com/beatgammit/base64-js" target="_blank">base64-js</a></td><td>1.5.1</td><td>MIT</td><td>Base64 encoding/decoding in pure JS</tr>
<tr><td>basic-auth</td><td>2.0.1</td><td>MIT</td><td>node.js basic auth parser</tr>
<tr><td><a href="https://github.com/juliangruber/balanced-match" target="_blank">balanced-match</a></td><td>1.0.2</td><td>MIT</td><td>Match balanced character pairs, like "{" and "}"</tr>
<tr><td>babel-plugin-polyfill-corejs3</td><td>0.10.6</td><td>MIT</td><td>A Babel plugin to inject imports to core-js@3 polyfills</tr>
<tr><td>babel-plugin-polyfill-regenerator</td><td>0.6.2</td><td>MIT</td><td>A Babel plugin to inject imports to regenerator-runtime</tr>
<tr><td>babel-plugin-polyfill-corejs2</td><td>0.4.11</td><td>MIT</td><td>A Babel plugin to inject imports to core-js@2 polyfills</tr>
<tr><td><a href="https://github.com/inspect-js/available-typed-arrays#readme" target="_blank">available-typed-arrays</a></td><td>1.0.7</td><td>MIT</td><td>Returns an array of Typed Array names that are available in the current environment</tr>
<tr><td><a href="https://axios-http.com" target="_blank">axios</a></td><td>1.7.7</td><td>MIT</td><td>Promise based HTTP client for the browser and node.js</tr>
<tr><td><a href="https://github.com/gregjacobs/Autolinker.js" target="_blank">autolinker</a></td><td>3.16.2</td><td>MIT</td><td>Utility to automatically link the URLs, email addresses, phone numbers, hashtags, and mentions (Twitter, Instagram) in a given block of text/HTML</tr>
<tr><td><a href="https://github.com/adapt-security/at-utils#readme" target="_blank">at-utils</a></td><td>0.6.3</td><td>MIT</td><td>A collection of CLI helper utilities for maintaining installations of the Adapt authoring tool.</tr>
<tr><td><a href="https://github.com/indutny/asn1.js" target="_blank">asn1.js</a></td><td>5.4.1</td><td>MIT</td><td>ASN.1 encoder and decoder</tr>
<tr><td><a href="https://github.com/alexindigo/asynckit#readme" target="_blank">asynckit</a></td><td>0.4.0</td><td>MIT</td><td>Minimal async jobs utility library, with streams support</tr>
<tr><td><a href="https://caolan.github.io/async/" target="_blank">async</a></td><td>3.2.6</td><td>MIT</td><td>Higher-order functions and common patterns for asynchronous code</tr>
<tr><td>asap</td><td>2.0.6</td><td>MIT</td><td>High-priority task queue for Node.js and browsers</tr>
<tr><td><a href="https://github.com/es-shims/ArrayBuffer.prototype.slice#readme" target="_blank">arraybuffer.prototype.slice</a></td><td>1.0.3</td><td>MIT</td><td>ES spec-compliant shim for ArrayBuffer.prototype.slice</tr>
<tr><td><a href="https://github.com/es-shims/Array.prototype.toSorted#readme" target="_blank">array.prototype.tosorted</a></td><td>1.1.4</td><td>MIT</td><td>An ESnext spec-compliant `Array.prototype.toSorted` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td>array.prototype.flat</td><td>1.3.2</td><td>MIT</td><td>An ES2019 spec-compliant `Array.prototype.flat` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td>array.prototype.flatmap</td><td>1.3.2</td><td>MIT</td><td>An ES2019 spec-compliant `Array.prototype.flatMap` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td><a href="https://github.com/es-shims/Array.prototype.findLast#readme" target="_blank">array.prototype.findlast</a></td><td>1.2.5</td><td>MIT</td><td>An ESnext spec-compliant `Array.prototype.findLast` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td><a href="https://github.com/es-shims/Array.prototype.findLastIndex#readme" target="_blank">array.prototype.findlastindex</a></td><td>1.2.5</td><td>MIT</td><td>An ESnext spec-compliant `Array.prototype.findLastIndex` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td>array-includes</td><td>3.1.8</td><td>MIT</td><td>An ES7/ES2016 spec-compliant `Array.prototype.includes` shim/polyfill/replacement that works as far down as ES3.</tr>
<tr><td><a href="https://github.com/inspect-js/array-buffer-byte-length#readme" target="_blank">array-buffer-byte-length</a></td><td>1.0.1</td><td>MIT</td><td>Get the byte length of an ArrayBuffer, even in engines without a `.byteLength` method.</tr>
<tr><td><a href="https://github.com/blakeembrey/array-flatten" target="_blank">array-flatten</a></td><td>1.1.1</td><td>MIT</td><td>Flatten an array of nested arrays into a single flat array</tr>
<tr><td>argparse</td><td>2.0.1</td><td>Python-2.0</td><td>CLI arguments parser. Native port of python's argparse.</tr>
<tr><td>archive-type</td><td>4.0.0</td><td>MIT</td><td>Detect the archive type of a Buffer/Uint8Array</tr>
<tr><td><a href="https://github.com/ldthomas/apg-lite#readme" target="_blank">apg-lite</a></td><td>1.0.4</td><td>BSD-2-Clause</td><td>lightweight JavaScript APG parser</tr>
<tr><td><a href="https://github.com/micromatch/anymatch" target="_blank">anymatch</a></td><td>3.1.3</td><td>ISC</td><td>Matches strings against configurable strings, globs, regular expressions, and/or functions</tr>
<tr><td>ansi-escapes</td><td>4.3.2</td><td>MIT</td><td>ANSI escape codes for manipulating the terminal</tr>
<tr><td>ansi-styles</td><td>4.3.0</td><td>MIT</td><td>ANSI escape codes for styling strings in the terminal</tr>
<tr><td>ansi-regex</td><td>5.0.1</td><td>MIT</td><td>Regular expression for matching ANSI escape codes</tr>
<tr><td><a href="https://github.com/doowb/ansi-colors" target="_blank">ansi-colors</a></td><td>4.1.3</td><td>MIT</td><td>Easily add ANSI colors to your text and symbols in the terminal. A faster drop-in replacement for chalk, kleur and turbocolor (without the dependencies and rendering bugs).</tr>
<tr><td><a href="https://ajv.js.org" target="_blank">ajv</a></td><td>8.17.1</td><td>MIT</td><td>Another JSON Schema Validator</tr>
<tr><td><a href="https://github.com/nexdrew/ansi-align#readme" target="_blank">ansi-align</a></td><td>3.0.1</td><td>ISC</td><td>align-text with ANSI support for CLIs</tr>
<tr><td>agent-base</td><td>6.0.2</td><td>MIT</td><td>Turn a function into an `http.Agent` instance</tr>
<tr><td><a href="https://github.com/tomgreenfield/adapt-octopus#readme" target="_blank">adapt-octopus</a></td><td>0.1.0</td><td>GPL-3.0</td><td>Convert old Adapt schema into conformant JSON schema</tr>
<tr><td><a href="https://github.com/acornjs/acorn-jsx" target="_blank">acorn-jsx</a></td><td>5.3.2</td><td>MIT</td><td>Modern, fast React.js JSX parser</tr>
<tr><td>adapt-cli</td><td>3.3.0</td><td>GPL-3.0</td><td>Command line tools for Adapt</tr>
<tr><td>accepts</td><td>1.3.8</td><td>MIT</td><td>Higher-level content negotiation</tr>
<tr><td><a href="https://github.com/acornjs/acorn" target="_blank">acorn</a></td><td>8.12.1</td><td>MIT</td><td>ECMAScript parser</tr>
<tr><td>image-size</td><td>0.5.5</td><td>MIT</td><td>get dimensions of any image file</tr>
</table>
</details>

## Commonly asked questions