Paylogic developer portal
=========================

This repository contains the sources for the Paylogic developer portal hosted
at developer.paylogic.com_. We use the static site generator Pelican_ to
generate the web pages from content written in the reStructuredText_ format.

The git repository is hosted on our GitHub_ account and we use `GitHub Pages`_
with a custom DNS name for hosting.


.. image:: https://travis-ci.org/paylogic/developer.paylogic.com.svg?branch=master
    :target: https://travis-ci.org/paylogic/developer.paylogic.com
    

Running it locally
------------------

To run the developer portal locally (e.g. to easily preview changes) the
following steps should help you get started::

  # Clone the git repository.
  git clone git@github.com:paylogic/developer.paylogic.com.git

  # Run Pelican and view the result in a web browser.
  cd developer.paylogic.com
  make devserver [DEVSERVER_PORT=<port>]
  gnome-open http://127.0.0.1:8000  # DEVSERVER_PORT is 8000 by default


Publishing changes
------------------

This repo is set up the way travis will build the static content automatically on every push
to ``master`` branch, and then will push the build result to ``gh-pages`` branch, which is then
served by `GitHub Pages`_.


License
-------

This work is licensed under the `Creative Commons Attribution-ShareAlike 3.0
Unported License`_.

.. External references:
.. _Creative Commons Attribution-ShareAlike 3.0 Unported License: http://creativecommons.org/licenses/by-sa/3.0/
.. _developer.paylogic.com: http://developer.paylogic.com/
.. _GitHub Pages: http://pages.github.com/
.. _GitHub: https://github.com/paylogic
.. _Pelican: http://docs.getpelican.com/en/3.2/getting_started.html
.. _reStructuredText: http://docutils.sourceforge.net/rst.html
