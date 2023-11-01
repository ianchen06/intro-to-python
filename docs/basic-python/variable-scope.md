# Variable Scope

## Introduction to Variable Scope

In programming, the scope of a variable refers to the region in a program where that variable is accessible. Python supports different types of variable scopes. Understanding variable scope is crucial for managing and utilizing variables efficiently in a program.

## Types of Variable Scopes in Python

Python has two primary variable scopes:

1. **Local Scope**: Variables defined inside a function are in the local scope of that function. They are only accessible within that function.
2. **Global Scope**: Variables defined at the top-level of a script or outside of any function have a global scope. They are accessible throughout the file.

## Use Cases

- **Local Variables**: Useful for temporary storage of information that is only needed within a function.
- **Global Variables**: Useful for storing information that needs to be accessed by multiple functions.

## Examples

### Example 1: Local Scope

```python
def greet():
    message = "Hello, World!"  # local variable
    print(message)

greet()  # Output: Hello, World!
print(message)  # This will cause an error because 'message' is not accessible here.
```

### Example 2: Global Scope

```python
message = "Hello, Python!"  # global variable

def greet():
    print(message)

greet()  # Output: Hello, Python!
print(message)  # Output: Hello, Python!
```

### Example 3: Modifying Global Variable inside a Function

```python
counter = 0  # global variable

def increment():
    global counter  # Tell Python that we want to use the global 'counter'
    counter += 1

increment()
print(counter)  # Output: 1
```

## Exercises

1. **Local Variable Usage**:
   Write a function `calculate_sum` that accepts two parameters, adds them, and prints the result. Test the function by calling it with two numbers.
   
2. **Global and Local Scope Interaction**:
   Create a global variable `name` with your name. Write a function `greet` that prints "Hello" followed by the global `name` variable, and then changes `name` to a local variable by assigning a different name to it. What happens when you print `name` after calling the function?
   
3. **Modifying a Global Variable**:
   Define a global variable `count` set to 0. Write a function `increment_count` that increases the value of `count` by 1 each time it's called. Demonstrate this by calling the function multiple times and printing the value of `count` after each call.

Remember, understanding variable scope will greatly enhance your ability to structure and debug your code effectively. Happy coding!