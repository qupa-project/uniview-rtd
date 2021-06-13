Declaration
============

When simply declaring a value, the type must be explicitly stated

.. code-block::

	let a: int;

However if a variable is being assigned on declaration the type can be inferred, and thus ommited from the code

.. code-block::

	let a = 1;

Both of these statements define ``a`` as an ``int``, however only the second one defines the value.
Attempting to use an undefined value will result in a crash at compile time.

.. code-block::
	:linenos:
	:emphasize-lines: 2

	let a: int;
	println(a);

This example will not compile, as line 2 attempts to use an undefined value.