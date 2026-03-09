# Task 2

## `undefined.c`

1. Compile  `undefined.c` without any special compiler options:

       gcc undefined.c

2. Run the compiled program to see what it does:

       ./a.out

   **Then remove `a.out`**.

3. Recompile `undefined.c`, this time using the `-Wall` option:

       gcc -Wall undefined.c

   What do you see in the terminal?
   Comes up with a warning that 'i' was not declared when first used

4. Run the program to verify that behaviour is unchanged,
   **then remove `a.out` once again**.

5. Recompile `undefined.c` using the `-Wall` and `-Werror` options. Does the
   compiler output change in any way? Is an executable generated?
   No, compilation was terminated

## `double_free.c`

1. Compile `double_free.c` using the `-Wall`, `-Wextra` and `-Werror`
   compiler options. Do you see any messages from the compiler?
   Does compilation succeed?
   Only Wall works, but comes with a warning

2. Run the compiled program. What happens? Do you get any clues about what
   has gone wrong?
   There are 2 free(a), which can't possible

3. Repeat Step 1 for `crash.c` from Task 1. What can you conclude from these
   experiments about the compiler options that you have used?
