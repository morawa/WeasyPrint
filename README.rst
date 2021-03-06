WeasyPrint
##########

.. image:: https://img.shields.io/pypi/l/WeasyPrint.svg?style=flat-square
    :target: https://pypi.python.org/pypi/WeasyPrint/
    :alt: License

.. image:: http://img.shields.io/pypi/v/WeasyPrint.svg?style=flat-square
    :target: https://pypi.python.org/pypi/WeasyPrint/
    :alt: Latest Version

.. image:: http://img.shields.io/pypi/dm/WeasyPrint.svg?style=flat-square
    :target: https://pypi.python.org/pypi/WeasyPrint/
    :alt: Download

.. image:: http://img.shields.io/travis/Kozea/WeasyPrint.svg?style=flat-square
    :target: http://travis-ci.org/Kozea/WeasyPrint
    :alt: Build status

|

WeasyPrint is a visual rendering engine for HTML and CSS that can export
to PDF. It aims to support web standards for printing.
WeasyPrint is free software made available under a BSD license.

It is based on various libraries but *not* on a full rendering engine like
WebKit or Gecko. The CSS layout engine is written in Python, designed for
pagination, and meant to be easy to hack on.

* Free software: BSD licensed
* Python 2.6+ or 3.1+
* Website: http://weasyprint.org/
* Latest documentation: http://weasyprint.org/docs/
* Source code and issue tracker: https://github.com/Kozea/WeasyPrint

Pretty Page Breaking branch
###########################

These non-standard extensions will be added to give better control of page
breaking behavior and other aesthetics:

* Header/footer stack: stack of elements (table/div) which will be rendered
  on top/bottom of the page between <push> and <pop>
* Stickness factor (default 1.0) to decide which elements should be more or less
  "sticked" (hard to break pages between them)
* Compactness factor for whole document which has influence for compromise
  between page count and stickness sum on page breaks
