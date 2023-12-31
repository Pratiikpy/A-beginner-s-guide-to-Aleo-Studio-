 

### Functions and recursion:

Functions are blocks of code that can be defined once and called multiple times with different arguments. Functions can return values or perform side effects, such as printing to the console or modifying global variables. Leo uses the keyword `function` followed by the function name, a list of parameters, an optional return type, and a block of code to define functions. For example, you can write a function that adds two numbers and returns the result like this:

```leo
function add(x: u8, y: u8) -> u8 {
    return x + y;
}
```

This function takes two parameters of type `u8`, which are unsigned 8-bit integers. It also specifies that it returns a value of type `u8`. The function body consists of a single statement that returns the sum of the two parameters using the `+` operator.

To call a function, you need to use its name followed by a list of arguments enclosed in parentheses. The arguments must match the types and order of the parameters. For example, you can call the `add` function with two arguments like this:

```leo
let z = add(3, 4);
```

This statement assigns the value returned by the `add` function to a variable named `z`. The value of `z` is 7.

Functions can also be recursive, which means they can call themselves within their own body. Recursion is a powerful technique that can be used to solve problems that have a recursive structure, such as factorial, Fibonacci, or binary search. However, recursion can also cause stack overflow errors if the function does not have a base case or a termination condition. For example, you can write a recursive function that calculates the factorial of a number like this:

```leo
function factorial(n: u32) -> u32 {
    // base case: if n is zero, return 1
    if n == 0 {
        return 1;
    }
    // recursive case: if n is positive, return n times the factorial of n - 1
    else {
        return n * factorial(n - 1);
    }
}
```

This function takes a parameter of type `u32`, which is an unsigned 32-bit integer. It also specifies that it returns a value of type `u32`. The function body consists of an if-else statement that checks if the parameter is zero or not. If it is zero, it returns 1 as the base case. If it is positive, it returns the product of the parameter and the factorial of the parameter minus one as the recursive case. The function calls itself with a smaller argument until it reaches the base case.

To call a recursive function, you need to use its name followed by an argument enclosed in parentheses. The argument must match the type of the parameter. For example, you can call the `factorial` function with an argument like this:

```leo
let x = factorial(5);
```

This statement assigns the value returned by the `factorial` function to a variable named `x`. The value of `x` is 120.

### Arrays and tuples:

Arrays and tuples are data structures that can store multiple values of the same or different types. Arrays are ordered collections of values that have a fixed length and are indexed by numbers. Tuples are ordered collections of values that have a variable length and are indexed by names.

To declare an array in Leo, you need to use square brackets (`[]`) to enclose a list of values separated by commas. You can also specify the type and size of the array using the syntax `[type; size]`. For example, you can declare an array of five integers like this:

```leo
let arr: [u8; 5] = [1, 2, 3, 4, 5];
```

This statement declares an array named `arr` with a type annotation `[u8; 5]`, which means it is an array of five unsigned 8-bit integers. It also assigns an initial value to the array using a list of five integers enclosed in square brackets.

To access or modify an element of an array, you need to use its name followed by an index enclosed in square brackets. The index must be an integer between zero and one less than the size of the array. For example, you can access or modify the first element of `arr` like this:

```leo
let x = arr[0]; // get the first element
arr[0] = 10; // set the first element to 10
```

These statements assign the value of the first element of `arr` to a variable named `x`, and change the value of the first element of `arr` to 10. The value of `x` is 1, and the value of `arr` is [10, 2, 3, 4, 5].

To declare a tuple in Leo, you need to use parentheses (`()`) to enclose a list of values separated by commas. You can also specify the type and name of each element using the syntax `(name: type)`. For example, you can declare a tuple of three values like this:

```leo
let tup: (a: u8, b: bool, c: char) = (1, true, 'A');
```

This statement declares a tuple named `tup` with a type annotation `(a: u8, b: bool, c: char)`, which means it is a tuple of three elements with names `a`, `b`, and `c`, and types `u8`, `bool`, and `char`. It also assigns an initial value to the tuple using a list of three values enclosed in parentheses.

To access or modify an element of a tuple, you need to use its name followed by a dot (`.`) and the name of the element. For example, you can access or modify the second element of `tup` like this:

```leo
let y = tup.b; // get the second element
tup.b = false; // set the second element to false
```

These statements assign the value of the second element of `tup` to a variable named `y`, and change the value of the second element of `tup` to false. The value of `y` is true, and the value of `tup` is (1, false, 'A').

These are some of the basic functions, recursion, arrays, and tuples in Leo. You can use them to write programs that perform calculations, logic, or data manipulation. In the next section, I will show you how to write circuits and traits in Leo.
