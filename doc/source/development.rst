*********** 
Development
***********
.. _github: http://github.com/alisaifee/holmium.core/
.. _issue tracker: http://github.com/alisaifee/holmium.core/issues
.. _travis: https:/travis-ci.org/#!/alisaifee/holmium.core 
.. _develop: http://pythonhosted.org/distribute/setuptools.html#development-mode
.. _phantomjs download page: http://phantomjs.org/download.html 
.. _freenode irc channel: irc://irc.freenode.net/#holmium

Contributors
============
.. include:: ../../CONTRIBUTORS.rst

Project Resources
=================
Continuous Integration
    The project is being continuously built with `travis`_ against python 2.6 & 2.7 & 3.3. 

Code
    The code is hosted on `github`_.

Bugs, Feature Requests
    Tracked at the `issue tracker`_.

Questions
    `freenode irc channel`_ 

Installation
============

.. note:: 
   
   Holmium is tested and supported on pythons version 2.6, 2.7 & 3.3.

The stable version can be installed either via ``pip`` or ``easy_install``.

.. code-block:: bash

    pip install holmium.core 
    # or 
    easy_install holmium.core 


To use holmium.core directly from source the preferred method is to use the
`develop`_ mode. This will make :mod:`holmium.core` available on your `PATH`, 
but will point to the checkout. Any updates made in the checkout will be available 
in the *installed* version.

.. code-block:: bash 

    git clone git@github.com:alisaifee/holmium.core 
    cd holmium.core 
    sudo python setup.py develop 

Tests
=====
:mod:`holmium.core` uses ``nosetests`` for running its tests. You will also
need ``phantomjs`` installed to run certain tests that make more sense without 
mocking. For instructions on installing ``phantomjs`` go to the `phantomjs download page`_.

.. code-block:: bash 

    cd holmium.core 
    nosetests --with-coverage --cover-html --cover-erase --cover-package=holmium.core 


