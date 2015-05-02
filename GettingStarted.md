# Getting Started Guide - Introduction and How-To

# Introduction #

html2fb takes in html (ideally clean html but it can handle a lot of real-world html) and converts to fb2 format. html2fb is both a library for developers and a command line tool for end users.


# Requirements #

Main requirement is Python, originally tested with version 2.3 currently testing with 2.5.

Tested under both Linux (Ubuntu) and Windows (XP).

There are some recommened but purely optional requirements:
  * wxPython http://www.wxpython.org/ - an optional GUI front end
  * PIL http://www.pythonware.com/products/pil/ - PIL can be used to convert images to PNG in the result FB2 file. If image conversion is not required PIL is not required, for example if your ebook reader supports JPG and GIF files.
  * PyRtfLib http://sourceforge.net/projects/pyrtflib/ - this is used to convert RTF files into fb2 format (note pictures not currently supported by PyRtfLib)
  * Convert LIT http://www.convertlit.com/ - support for .lit files is possible by making (subprocess) calls to convertlit

# Features #

  * command line
  * GUI
  * supports reading from .zip (and .Z compressed) files
  * supports writing to .zip files to save space
  * .html file input
  * .txt file input
  * .rtf file input
  * .lit file input


# Basic Usage #

```
   html2fb.py -i input.html 
```

This will read in input.html and automatically create a .zip file containing the .fb2 ebook.


See --help (or GUI) for more information and options.