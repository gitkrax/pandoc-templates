Templates for [pandoc](http://github.com/jgm/pandoc).

If you use custom templates, we recommend forking this repository,
so that you can integrate changes to the default templates in future
pandoc releases.

All of the templates in this repository are dual licensed, under both
the GPL (v2 or higher, same as pandoc) and the BSD 3-clause license
(included below).

----

Copyright (c) 2014, John MacFarlane

All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.

    * Redistributions in binary form must reproduce the above
      copyright notice, this list of conditions and the following
      disclaimer in the documentation and/or other materials provided
      with the distribution.

    * Neither the name of John MacFarlane nor the names of other
      contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

----

This personal fork of Pandoc Templates contains additional templates,
mostly for academic writing.

* `article.latex` is a nice looking template for articles that doesn't
  follow any particular journal conventions, but looks decent enough to
  show your work. There are several YAML-settings that the template uses.
    - Supports authorblocks, meaning that you define `author.name`
      and `author.affiliation` for one or more authors and see them 
      set properly in the beginning of the text.
    - Adding `abstract` into the YAML-section adds an abstract to the
      beginning of the text.
    - If `numbersections` is set to true, sections are numbered.
    - If `twocolumn` is set true, the text is set in two columns.
    - As usual, you can use pandocs native support for citations to 
      generate a bibliography.
* `cv.latex` is a decent looking cv meant mostly for boring academic cvs
  that need to follow the guidelines of Finnish Advisory Board on Research
  Integrity. It needs to be run with xelatex.
* `aka.latex` is a tightly set template for writing Academy of Finland
  applications. Use level 1 headings for the main headings and level 2 headings
  for inline headings. You need to define fonts, papersize and margins in the
  YAML-sections. Also set `numberedsections: true` for numbered sections. Uses the `datetime2` package, so you can add the current date by writing `\today`.
