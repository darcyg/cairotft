cairotft
========

.. image:: https://readthedocs.org/projects/cairotft/badge/?version=latest
   :target: http://cairotft.readthedocs.org

.. image:: https://img.shields.io/badge/github-forkme-lightgrey.svg
    :target: https://github.com/LinkCareServices/cairotft

.. image:: https://img.shields.io/pypi/l/cairotft.svg?style=flat

.. image:: https://img.shields.io/pypi/v/cairotft.svg?style=flat
    :target: https://pypi.python.org/pypi/cairotft

cairotft is a small module for Python (3.4+) used to draw interface on
tft screen using the framebuffer interface.

It's first designed for tft screens, but cairotft can draw
interface on any framebuffer interface;
like the default /dev/fb0 on linux consoles.

Licence
-------

cairotft is free software made available under a BSD license.
See LICENSE.txt

Fonctionnalities
----------------

* support python 3.4 (only tested on python 3.4 for now)
* support double-buffering
* included with widgets:

  * blick icon
  * text marquee
* included animation transitions formulas like mootools.Fx.Transitions
* uses asyncio event loop
* ... (more in the future)

Documentation
-------------

See the full documentation on readthedocs: http://cairotft.readthedocs.org


Installation
------------

from pypi
*********

* create a virtualenv::

    pyvenv-3.4 ~/.virtualenvs/cairotft
    source ~/.virtualenvs/cairotft/bin/activate

* install the package::

    pip install cairotft

from sources
************

* clone the repo::

    git clone https://github.com/LinkCareServices/cairotft.git
    cd cairotft

* create a virtualenv::

    pyvenv-3.4 ~/.virtualenvs/cairotft
    source ~/.virtualenvs/cairotft/bin/activate

* install::

    python setup.py install

* and for development::

    python setup.py develop

* and (eventually) development dependencies::

    pip install --upgrade -r dev-requirements.txt

Running tests
-------------

tests
*****

install tests and developpement requirements::

    pip install -r dev-requirements.txt

on the main cairotft directory run the tests::

    nosetests

or with verbosity::

    nosetests -v
