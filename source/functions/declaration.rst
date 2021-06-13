Declaration
###########

All functions must have three main elements
	#. Name
	#. Signature
	#. Return type

The combination of a name, and signature must also make any function unique.
Hence you cannot have two instances of the same function.

All types within a function header must be explicit as they cannot be efficiently infered.


Examples
--------

This function takes no inputs, but outputs one int

.. code-block::
	:linenos:

	fn main(): int {
	  // body
	  return 0;
	}

This function takes two input ints, but returns no output

.. code-block::
	:linenos:

	fn main(a: int, b: int): void {
	  // body
	  return;
	}