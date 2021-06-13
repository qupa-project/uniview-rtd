Installation
============

There are only three main requirements to install uniview.

#. Clang++ v12 or greater
#. Having NPM installed
#. NodeJS v12 or greater


Checking Prerequisites
**********************

Checking Clang Install
----------------------
To check you have the correct version of clang installed, simply run the command:

.. code-block::bash

  clang++ --version

And check the version number is greater than 12

Checking NPM install
--------------------
Run the command:

.. code-block:: bash

  npm -v

Checking Node install
---------------------
Run the command:

.. code-block:: bash

  node -v


Installing Uniview
******************
Simply run:

.. code-block:: bash

  npm install -g @qupa/uniview

This will install uniview, bind the compile command, and pre-build the standard libraries.

Installing IDE Tools
--------------------
| There is a VSCode extension called ``Uniview Language`` which is the offical VSCode extension for the language.

Checking Installation
---------------------

.. code-block:: bash

  uvc --version