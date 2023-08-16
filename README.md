# Rec+
This is basically a derivative of my previous language, [Rec](https://github.com/jfioasd/rec), which (I hope) is easier to program in.

You can compile `rec_p.c` with a compiler that supports C99.

The language has the following commands:

|Command|Behavior|
|:--:| :--:|
|`123`| Push number.|
|`+`| Addition. |
|`*`| Multiplication. |
|`_`| Negative; Push `-x`. |
|`=`| Pushes whether `x == 0`. |
|`:`| Load; Pops `x`, pushes `x`th-to-top item on stack. |
|`;`| Store; Pops `v` and `x`. Assigns `x`th-to-top item on stack to `v`.|
|`[ ... ]`| Infinite loop; executes <code>...</code> forever. |
|`^`| Pops `x`. If `x != 0`, break out of the innermost `[ ... ]` loop. |
