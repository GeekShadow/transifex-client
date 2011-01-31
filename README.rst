
=============================
 Transifex Command-Line Tool
=============================

Check the full documentation at http://help.transifex.net/user-guide/client/client-0.4.html


Installing
==========

You can install the latest version of transifex-client running 
``pip install transifex-client`` or ``easy_install transifex-client``
You can also install the `in-development version`_ of transifex-client with
``pip install transifex-client==dev`` or ``easy_install transifex-client==dev``.

.. _in-development version: http://code.indifex.com/transifex-client/get/tip.gz#egg=transifex-client-dev


Releasing
=========

To create a new release:

1. Update local rep and update the version in ``setup.py``::

    $ hg pull -u
    $ vim setup.py

2. Test::

    $ python setup.py clean sdist
    $ cd dist
    $ tar zxf ...
    $ cd transifex-client
    ...test

3. Package and upload on PyPI::

    $ python setup.py clean sdist bdist_egg upload