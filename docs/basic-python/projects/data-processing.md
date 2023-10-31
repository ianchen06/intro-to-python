# Simple Data Cleaning and Processing

### Project Description:
In this project, we will be working with a dataset that contains information about a collection of books. The dataset is slightly messy: it contains missing values, inconsistent formatting, and requires some basic transformations. Our goal is to clean and process this dataset using Python's fundamental structures and control flows such as lists, dictionaries, list comprehensions, for-loops, and if-else statements.

By the end of this project, you will have a clean dataset that is ready for further analysis or storage in a more structured format.

### Dataset Overview:
Our dataset is a list of dictionaries. Each dictionary contains information about a single book, with the following keys: 'title', 'author', 'published_year', and 'pages'. Here is a sample of the dataset:

```python
books_data = [
    {'title': 'Python Basics', 'author': 'H. Programmer', 'published_year': '2020', 'pages': '300'},
    {'title': 'Learning Python', 'author': 'Joe Smith', 'published_year': 'None', 'pages': '250'},
    {'title': 'Fluent Python', 'author': 'Luciano Ramalho', 'published_year': '2015', 'pages': 'N/A'},
    {'title': 'Data Science for Dummies', 'author': '', 'published_year': '2016', 'pages': '400'},
    # ... more books
]
```

### Tasks:

#### Task 1: Remove Books with Missing Information
Remove any books from the dataset that have missing information ('None' or empty strings).

#### Task 2: Convert Page Numbers
Ensure that all page numbers are integers. Some page numbers are currently stored as strings.

#### Task 3: Filter Books Published After 2010
Create a new list containing only the books that were published after 2010.

#### Task 4: Generate a Summary Dictionary
Generate a summary dictionary that contains the count of books for each author.

### Detailed Instructions:

#### Task 1: Remove Books with Missing Information
1. Iterate over the `books_data` list.
2. Check if any of the values in the dictionary are 'None' or empty strings.
3. If a book has missing information, remove it from the list.

#### Task 2: Convert Page Numbers
1. Iterate over the `books_data` list.
2. Check if the 'pages' key has a value that is a string.
3. Convert the string to an integer and update the dictionary.

#### Task 3: Filter Books Published After 2010
1. Use a list comprehension to filter out books published after 2010.
2. Store the filtered books in a new list called `recent_books`.

#### Task 4: Generate a Summary Dictionary
1. Create an empty dictionary called `author_summary`.
2. Iterate over the `books_data` list.
3. For each book, check if the author is already a key in the dictionary.
4. If the author is a key, increment the count. If not, add the author to the dictionary with a count of 1.

### Example Code:

```python
# Task 1: Remove Books with Missing Information
cleaned_books = [book for book in books_data if None not in book.values() and '' not in book.values()]

# Task 2: Convert Page Numbers
for book in cleaned_books:
    if isinstance(book['pages'], str):
        book['pages'] = int(book['pages'])

# Task 3: Filter Books Published After 2010
recent_books = [book for book in cleaned_books if int(book['published_year']) > 2010]

# Task 4: Generate a Summary Dictionary
author_summary = {}
for book in cleaned_books:
    author = book['author']
    author_summary[author] = author_summary.get(author, 0) + 1
```

### Test Cases / Test Data:
Make sure that after each task, the dataset is transformed as expected. You can print out the dataset or the results after each task to verify.

1. After Task 1, there should be no books with missing information.
2. After Task 2, all page numbers should be integers.
3. After Task 3, the `recent_books` list should only contain books published after 2010.
4. After Task 4, the `author_summary` dictionary should accurately reflect the count of books for each author.

Good luck, and have fun cleaning and processing this dataset!

## Additional Resources

- [David Beazley | Keynote: Built in Super Heroes](https://www.youtube.com/watch?v=lyDLAutA88s)