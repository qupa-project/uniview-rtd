Lending
#######

Values of any type can also be lent to function calls (but only in function calls).
This may appear as reusing a value, but instead is actually a contraction of a reassignment.
Any value that is lent, is actually parsed forward,
then the function returns an extra result which is then reassigned to the same name.

Here is an example of adding integers not using lending.

.. code-block::
	:linenos:

	fn main() {
	  let value = 3;
	  value = add(value, 3);
	  println(value); // 9
	}

	fn add(a: int, b: int) {
	  return a + b;
	}


Here is an example of adding integers not using lending.

.. code-block::
	:linenos:

	fn main() {
	  let value = 3;
	  add(@value, 3);
	  println(value); // 9
	}

	fn add(a: @int, b: int) {
	  a = a + b;
	}

Why using lending? The two examples are the same length.
	In this example we were using ``int`` which is a primative type, hence there is no real advantage.
	However later when we introduce classes, this method can have minor improvements
	due to the compiler being able to easily determine more information about the program.

	When classes are introduced later, the benfits will become more obvious of the reduce code needed,
	and the increased clarity.

When should I use lending?
	If the primary goal of your function is to alter some value then return it,
	it is generally better to use lending for any none ``normal`` type values.