# Monkey Programming Language Basics

## Binding Values

```
let age = 1;
let name = "Monkey";
let result = 5 * (10 / 2);
```

## Arrays and Hash

```
let myArray = [1, 2, 3, 4, 5];
let myHash = {"course": "Interpreter in Go", "pages": 200};

myArray[0] // => 1
myHash["course"] // => "Interpreter in Go"
```

## Functions

```
let add = fn(a, b) { return a + b; };

let add = fn(a, b) { a + b; }

// calling function
add(1, 4);

// fibonacci
let fibonacci = fn(x) {
    if (x == 0) {
        0
    } else {
        if (x == 1) {
            1
        } else {
            fibonacci(x - 1) + fibonacci(x - 2);
        }
    }
};
```

## Higher Order Functions

```
let twice = fn(f, x) {
    return f(f(x));
};

let addTwo = fn(x) {
    return x + 2;
};

twice(addTwo, 2); // => 6
```

## First Program

```
let five = 5;
let ten = 10;

let add = fn(x, y) {
    x + y;
};

let result = add(five, ten);

// 5, 10
// five, ten, add, x, y, result
// let, fn
// =, ;, (,), {,}
```
# interpreter-in-Go-
# interpreter-in-Go-
