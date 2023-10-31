# Data Processing with Python

Data cleaning, transformation, and analysis are some of the most common tasks in data science. This section will cover the basics of data processing with Python.

## Example: Reading a CSV File

```python
import csv

with open("data.csv") as file:
    reader = csv.reader(file)
    for row in reader:
        print(row)
```

## Example: Writing a CSV File

```python
import csv

with open("data.csv", "w") as file:
    writer = csv.writer(file)
    writer.writerow(["Name", "Age"])
    writer.writerow(["John", 36])
    writer.writerow(["Jane", 25])
```

## Regular Expressions

Regular expressions are a powerful tool for matching patterns in text. They are used in many programming languages, including Python.

### Example: Matching a Pattern

```python
import re

pattern = r"hello"

if re.match(pattern, "hello world"):
    print("Match")
else:
    print("No match")
```

## Additional Resources

- [David Beazley | Keynote: Built in Super Heroes](https://www.youtube.com/watch?v=lyDLAutA88s)