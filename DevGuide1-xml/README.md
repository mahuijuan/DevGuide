This is the last version of the 1.1.1 tree, that is showing the thinking of the original founders of OWASP. 

As you can see, it's in XML format, which basically killed the project. There was a restart prior to my taking over the project in 2003, and this text is that restart. 

## History

This is the abandoned 2.0 alpha XML branch. Do not use this version.

* 2.0 alpha - never published DO NOT USE

## Building this edition

This version of the Guide is written in an old DocBook format, so generating a copy on anything other than Linux is non-trivial. And on Linux, it's basically not possible in 2013 without porting the Guide to modern DocBook or DAPS.

The root document keeps its entity declarations local to this repository. If you attempt an archival build, use a locally installed DocBook XSL stylesheet and keep the XML processor offline:

```sh
xsltproc --nonet --output guide.fo /absolute/path/to/local/docbook-xsl/fo/docbook.xsl book.xml
```

Do not remove `--nonet` or use a stylesheet URL. It should then be possible to pass `guide.fo` to a locally installed FOP PDF tool.

If you can help build this version, please let us know.

## Contact

Please contact Andrew van der Stock vanderaj@owasp.org for any queries about this edition.
