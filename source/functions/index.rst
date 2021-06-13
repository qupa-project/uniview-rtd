Functions
=========

.. toctree::
	:maxdepth: 1
	:caption: Contents:
	:glob:

	declaration
	calling
	lending

There are three main rules applied to functions to ensure the safety of code within Uniview.
	#. A child function can never outlive it's parent
	#. Any function must have ownership over all values it touches through it's entire life time
	#. All functions must return a value