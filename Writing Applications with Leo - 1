 

### Data types and variables:

Leo supports various data types that can be used to store and manipulate data in your programs. Some of the basic data types are:

- **Integers**: Integers are whole numbers that can be positive, negative, or zero. Leo supports different sizes of integers, such as `u8`, `u16`, `u32`, `u64`, `u128`, `i8`, `i16`, `i32`, `i64`, and `i128`. The prefix `u` stands for unsigned, which means the integer can only be positive or zero. The prefix `i` stands for signed, which means the integer can be positive, negative, or zero. The suffix indicates the number of bits used to store the integer. For example, `u8` can store values from 0 to 255, while `i8` can store values from -128 to 127.
- **Booleans**: Booleans are logical values that can be either true or false. Leo uses the keywords `true` and `false` to represent boolean values. Booleans can be used for conditional statements, logical operations, or assertions.
- **Strings**: Strings are sequences of characters that can be used to store text or messages. Leo uses double quotes (`"`) to enclose string literals. Strings can be concatenated using the `+` operator, or interpolated using the `{}` syntax. For example, `"Hello" + " World"` is equivalent to `"Hello World"`, and `"The answer is {42}"` is equivalent to `"The answer is 42"`.
- **Characters**: Characters are single characters that can be used to store symbols or letters. Leo uses single quotes (`'`) to enclose character literals. Characters can be converted to integers using the `to_int` method, or vice versa using the `from_int` method. For example, `'A'.to_int()` returns 65, and `char::from_int(66)` returns `'B'`.

To declare a variable in Leo, you need to use the keyword `let` followed by the variable name and an optional type annotation. You can also assign a value to the variable using the `=` operator. For example, you can declare an integer variable named `x` with a value of 10 like this:

```leo
let x: u8 = 10;
```

You can also omit the type annotation and let Leo infer the type from the value. For example, you can declare a boolean variable named `y` with a value of true like this:

```leo
let y = true;
```

To access or modify the value of a variable, you can use its name in an expression or a statement. For example, you can print the value of `x` using the `console.log` function like this:

```leo
console.log(x);
```

You can also change the value of `x` by assigning a new value to it like this:

```leo
x = 20;
```

Note that Leo variables are immutable by default, which means they cannot be changed after they are declared. To make a variable mutable, you need to use the keyword `mut` after the keyword `let`. For example, you can declare a mutable string variable named `z` like this:

```leo
let mut z = "Hello";
```

Now you can change the value of `z` by assigning a new value to it like this:

```leo
z = "World";
```

### Control structures and loops:

Leo supports various control structures and loops that can be used to control the flow of your program based on conditions or iterations. Some of the common control structures and loops are:

- **If-else statements**: If-else statements are used to execute different blocks of code based on a boolean condition. Leo uses the keywords `if`, `else if`, and `else` to construct if-else statements. For example, you can write an if-else statement that checks if a number is even or odd like this:

```leo
let x = 10;
if x % 2 == 0 {
    console.log("x is even");
} else {
    console.log("x is odd");
}
```

The condition after the keyword `if` is evaluated as a boolean expression. If it is true, the block of code inside the curly braces (`{}`) is executed. If it is false, the block of code after the keyword `else` is executed. You can also use multiple conditions with the keyword `else if`. For example, you can write an if-else statement that checks if a number is positive, negative, or zero like this:

```leo
let x = -5;
if x > 0 {
    console.log("x is positive");
} else if x < 0 {
    console.log("x is negative");
} else {
    console.log("x is zero");
}
```

- **For loops**: For loops are used to iterate over a range of values or a collection of elements. Leo uses the keyword `for` followed by a loop variable, the keyword `in`, and an iterable expression to construct for loops. For example, you can write a for loop that prints the numbers from 1 to 10 like this:

```leo
for i in 1..=10 {
    console.log(i);
}
```

The expression `1..=10` is a range that includes both the start and the end values. You can also use `1..10` to exclude the end value. The loop variable `i` takes each value in the range and executes the block of code inside the curly braces (`{}`). You can also use arrays or tuples as iterable expressions. For example, you can write a for loop that prints the elements of an array like this:

```leo
let arr = [1, 2, 3, 4, 5];
for x in arr {
    console.log(x);
}
```

- **While loops**: While loops are used to execute a block of code repeatedly while a boolean condition is true. Leo uses the keyword `while` followed by a condition and a block of code to construct while loops. For example, you can write a while loop that prints the numbers from 1 to 10 like this:

```leo
let i = 1;
while i <= 10 {
    console.log(i);
    i = i + 1;
}
```

The condition after the keyword `while` is evaluated as a boolean expression. If it is true, the block of code inside the curly braces (`{}`) is executed. If it is false, the loop terminates. You need to make sure that the condition eventually becomes false, otherwise the loop will run forever. You can also use the keyword `break` to exit the loop prematurely, or the keyword `continue` to skip the current iteration.

These are some of the basic data types, variables, control structures, and loops in Leo. You can use them to write simple programs that perform calculations, logic, or input/output operations. In the next section, I will show you how to write functions and recursion in Leo.
