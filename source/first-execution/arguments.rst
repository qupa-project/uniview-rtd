UVC Arguments
=============

Arguments are any statements after a given command.
For UVC (Uniview Compiler) the first argument must always be the entry file.
UVC only ever takes on file, any extra files must be included within the code itself.

By default UVC will compile your code to binary, then immediately execute it -
however there are command lines to change this behaviour.
Please note that any argument which includes a space, must be surrounded by ``"``.
(i.e. ``-o "./hello world.exe"``)


.. csv-table:: Arguments
	:file: listings/arguments.csv
	:header-rows: 1