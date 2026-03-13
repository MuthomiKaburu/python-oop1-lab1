# Python OOP Lab: Book and Coffee Classes

## Overview

This project demonstrates basic **Object-Oriented Programming (OOP)** concepts in Python by implementing two classes: **Book** and **Coffee**. The lab focuses on creating classes, defining attributes and methods, and validating data using Python properties.

## Book Class

### Attributes

* **title** – the title of the book
* **page_count** – the number of pages in the book

### Validation

The `page_count` property ensures that the value assigned is an integer.
If a non-integer value is provided, the program prints:

```
page_count must be an integer
```

### Method

`turn_page()`

This method prints:

```
Flipping the page...wow, you read fast!
```

Example:

```python
book = Book("Atomic Habits", 320)
book.turn_page()
```

---

## Coffee Class

### Attributes

* **size** – the size of the coffee
* **price** – the price of the coffee

### Validation

The `size` attribute must be one of the following values:

```
Small
Medium
Large
```

If an invalid size is entered, the program prints:

```
size must be Small, Medium, or Large
```

### Method

`tip()`

This method:

1. Prints a message
2. Increases the coffee price by **1**

Output:

```
This coffee is great, here’s a tip!
```

Example:

```python
coffee = Coffee("Medium", 4)
coffee.tip()
print(coffee.price)
```

---

## Testing

The project uses **pytest** to confirm that the classes work correctly and that attribute validation behaves as expected.

Run tests with:

```
pytest
```

---

## Author

Muthomi Kaburu
