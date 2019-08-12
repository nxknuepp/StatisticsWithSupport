# Statistics Packet

This repository contains the files necessary to generate the Math 110 Packet, Fall 2019, from Los Medanos College.

The sections in the packet have been written in both Word and Latex, with the packet itself generated with the Latex typesetting engine XeLatex. To make this possible, the original Word files have been converted to pdfs, and imported into Latex using the Latex package **pdfpages**. The packet contained in this repository was generated on a MacBook Air, using TexShop with MacTex as the underlying typesetting engine.

After downloading this repository you can generate the package itself using a computer running either OS X, Windows, or Linux. Instructions for building the packet on each of these operating systems appear below.

## The Files

* Math110Packet.tex	This is the main Latex file that you typeset. It assembles all the remaining files to produce the packet. **Note**: To ensure that the table of contents is populated you must run the typesetting engine at least two times. Running it *four times* guarantees all the cross references populate.
* mystyle.sty    This file contains the Latex macros for correct formatting of the table of contents, as well as those for wrapping the pdf files into Latex.
* img     This directory contains two images that are imported into two Latex sections of the packet.
* tex     This directory contains the Latex sections of the packet. Most of these assemble the pdf versions of the Word files.
* pdfs    These directory contains the pdf files that comprise the bulk of the packet.

## Font Issues

The default font for the packet is Cambria, available in both Windows and Mac. Provided you have a version of Microsoft Office installed, XeLatex will find the font and use it.

Because Cambria is not readily available on Linux, you should replace the Cambria font in the Math110Packet.tex file with Caladea font. The two fonts are essentially the same. It's obvious where to make the change in the file.

## How to Typeset the Package

### Linux

1. Download and extract the repository, preserving the directory hierarchy.
2. Install your Latex typesetting engine. Recommended: TexLive distribution.
3. If you want to use a typesetting editor to generate the package, download one. Recommended: TexMaker. Otherwise, it's fine to generate the packet from the command line.
4. Generate the packet itself, remembering to run the typesetting engine at least *two* times (four times to be sure). **Note** Because of the font choice, be sure to set the typesetting engine to use XeLatex. If you are using the command line, the command is
    xelatex Math110Packet.tex

### Windows

Same as Linux (TexLive and TexMaker).

### Mac OS X

Same as Linux, except use MacTex as the typesetting engine, and TexShop as the editor; be sure to set TexShop to use XeLatex because of the font choice.