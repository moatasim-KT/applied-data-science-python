# Week 5: NumPy: Memory-Efficient Computing

## Overview
NumPy is the foundation of high-performance numerical computing in Python, providing efficient, dense, and homogeneous array structures that allow for vectorized operations.

## Key Concepts
### 1. ndarray Memory Layout
- **Dense Storage**: Unlike Python lists, NumPy arrays store data in contiguous blocks of memory, significantly reducing overhead and improving cache locality.
- **Strides**: Understanding strides (the number of bytes to skip in memory to get to the next element) is essential for grasping how NumPy manipulates multi-dimensional arrays without physical data movement (e.g., transposing, slicing).

### 2. Advanced Indexing
- **Boolean Masking**: Creating a mask (e.g., `arr > threshold`) allows for highly efficient filtering of data without explicit loops.
- **Fancy Indexing**: Using arrays of integers to index into another array enables powerful, non-sequential data selection.

### 3. Broadcasting
- **Implicit Expansion**: Broadcasting allows operations between arrays of different shapes by implicitly expanding the smaller array to match the larger one’s shape, without copying data, ensuring operations are both fast and memory-efficient.
