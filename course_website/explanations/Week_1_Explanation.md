# Week 1: Python Data Structures Deep Dive

## Overview
This week focuses on mastering Python's built-in data structures and leveraging their unique features for memory-efficient and expressive data handling.

## Key Concepts
### 1. Lists
- **Dynamic Arrays**: Python lists act as dynamic arrays, offering flexibility in size and content types. Unlike C++, they are heterogeneous.
- **Advanced Slicing**: Using `[start:stop:step]` syntax allows for powerful data extraction and manipulation, such as reversing or sub-sampling.

### 2. List Comprehensions
- **Conciseness and Speed**: They offer a declarative way to create lists, often replacing verbose loops and functional patterns like `map` or `filter`.
- **Performance**: Comprehensions are typically faster than equivalent manual `append` loops due to internal optimization.

### 3. Dictionaries
- **Hash Maps**: Dictionaries are optimized hash tables, providing near O(1) average time complexity for lookups, insertions, and deletions.
- **Safe Access**: The `.get()` method allows for providing default values, avoiding `KeyError` exceptions when keys are missing.

### 4. Sets
- **Unique Collections**: Sets ensure all elements are unique and are optimized for set-theoretic operations like union, intersection, and difference.
- **Membership Testing**: Checking if an element exists in a set is extremely efficient (O(1)).

### 5. Tuples and Unpacking
- **Immutability**: Tuples are immutable, making them safer for fixed datasets and hashable keys in dictionaries.
- **Unpacking**: Powerful syntax allows assigning tuple elements directly to variables. Extended unpacking (using `*`) is useful for handling variable-length data.

### 6. Generators and Lazy Evaluation
- **Memory Efficiency**: Unlike lists, generators do not load the entire sequence into memory at once. They compute values on demand (lazy evaluation), which is crucial for handling large data streams in data science.

### 7. Itertools
- **Combinatorial Iterators**: This library provides high-performance building blocks for complex iteration patterns, essential for data prep and feature engineering workflows.
