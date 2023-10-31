# Write and Run Python Code

In this section, we'll explore the various ways you can write and execute Python code, including using the REPL (Read-Eval-Print Loop), writing .py files with a text editor, and utilizing Jupyter Notebooks. We'll compare and contrast these methods, list their advantages and disadvantages, and provide examples and exercises.

## 1. Interactively with REPL

### Use Case:
The Python REPL is often used for quick tests, learning, and small experiments. It's excellent for beginners to understand how Python syntax and commands work.

### Advantages:
- **Immediate Feedback**: Executes your Python code line by line and gives instant results.
- **No Setup Required**: Comes pre-installed with Python, no need to install anything extra.
- **Great for Learning**: Perfect for experimenting with new concepts and debugging.

### Disadvantages:
- **Not Suitable for Large Projects**: It's not practical for writing long or complex programs.
- **No Code Persistence**: Once the REPL is closed, the code is lost unless it's manually saved elsewhere.
- **Lack of Advanced Features**: Doesn't have features like syntax highlighting, debugging tools, or code completion that are available in text editors or IDEs.

### Example:
```python
>>> print("Hello, World!")
Hello, World!
```

### Exercise:
1. Open your Python REPL by typing `python` in your terminal or command prompt.
2. Try executing a simple calculation, like `8 * 7`.
3. Print your name using the `print()` function, e.g., `print("Your Name")`.

## 2. Using a Text Editor to Write .py Files

### Use Case:
Text editors are used for developing longer scripts and full applications. They are suitable for all levels of Python development.

### Advantages:
- **Code Persistence**: Your code is saved in files that can be reopened and edited anytime.
- **Advanced Features**: Most text editors come with syntax highlighting, code completion, and other helpful features.
- **Flexibility**: Can be used for projects of any size, from small scripts to large applications.

### Disadvantages:
- **Setup Required**: Requires installation and setup of a text editor suitable for coding.
- **No Immediate Feedback**: You need to run your script each time to see the output.
- **Learning Curve**: Some features of text editors (like Git integration, debugging, etc.) might have a learning curve for beginners.

### Example:
A simple Python script saved as `hello.py`:
```python
print("Hello, World!")
```

To run this script, you'd type `python hello.py` in your terminal or command prompt.

### Exercise:
1. Install a text editor (e.g., VS Code).
2. Create a new file called `greetings.py`.
3. Write a script that prints "Hello, Python!" and save the file.
4. Run your script from the terminal or command prompt.

## 3. Using Jupyter Notebook

### Use Case:
Jupyter Notebooks combines the interactivity of the REPL with the persistence of text editors. It's great for data analysis and exploratory programming.

### Advantages:
- **Interactive Development**: Allows you to run code cells individually and see their output immediately below the cell.
- **Documentation and Visualization**: Supports markdown for documentation and can display charts, images, and other media inline with the code.
- **Great for Data Science**: Especially useful for exploratory data analysis and iterative coding.

### Disadvantages:
- **Not Ideal for Software Development**: While great for experimentation, notebooks are not as convenient for developing production-level code.
- **Learning Curve**: New users might need some time to get used to the interface and concepts of notebooks.
- **Browser-Based**: Generally requires a browser to use, which might not be preferred by all developers.

### Example:
A cell in a Jupyter Notebook:
```python
print("Hello, Jupyter!")
```

After running the cell, the output "Hello, Jupyter!" is displayed immediately below.

### Exercise:
1. Start [Google Colab](https://colab.research.google.com) and create a new notebook.
2. In the first cell, type `print("Exploring Jupyter Notebook!")` and run the cell.
3. Try creating a new Markdown cell and write a brief introduction about yourself.

## Conclusion

Each method of writing and executing Python code has its advantages and disadvantages. The REPL is great for quick tests and learning, text editors are versatile for all kinds of projects, and Jupyter Notebooks are excellent for interactive development and data analysis.