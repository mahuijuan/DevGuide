This is the last version of the 1.1.1 tree, that is showing the 

## History

This is the abandoned 2.0 alpha XML branch. Do not use this version.

* 2.0 alpha - never published

## Building this edition

Building a document out of this requires considerable effort. This version of the Guide is in DocBook format, so generating a copy on anything other than Linux is non-trivial.

The root document keeps its entity declarations local to this repository. If you attempt an archival build, install local DocBook XSL and FOP packages, then keep the XML processor offline:

```sh
xsltproc --nonet --output guide.fo /absolute/path/to/local/docbook-xsl/fo/docbook.xsl guide_components.xml
```

Do not remove `--nonet` or use a stylesheet URL. Pass `guide.fo` to the locally installed FOP PDF tool.

## Contact

Please contact Andrew van der Stock vanderaj@owasp.org for any queries about this edition.
