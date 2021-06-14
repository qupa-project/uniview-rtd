If statements
=============

Based on a boolean opperator, then executes a certain branch of code

.. code-block::
	:linenos:

	if (a > b) {
		println("Greater");
	} else {
		println("Less than or equal to")
	}

Extra conditions can also be chained on failure of proceeding cases

.. code-block::
	:linenos:

	if (a % 5 == 0) {
		println ("Multiple of 5");
	} elif (a % 3 == 0) {
		println ("Multiple of 3");
	} elif (a % 2 == 0) {
		println ("Even number)
	}

The ``elif`` statement must always proceed either an ``if`` statement or another ``elif`` statement.
The ``else`` statement may only follow an ``if`` statement.
However neither ``elif``, nor ``else`` is required for a valid ``if`` statement.