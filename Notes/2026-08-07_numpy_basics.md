# Day 1 - NumPy Basics

## Date
07 August 2026

## Topics Covered
- Introduction to NumPy
- Arrays
- Matrices
- Shape
- Indexing
- Basic Operations
- Statistics
- Random Numbers

## What I Learned

- NumPy is a Python library for numerical computing.
- ndarray is the main data structure.
- Arrays are faster than Python lists.
- Images can be represented as matrices.

## Research Connection

Image processing uses NumPy arrays to represent pixels.
Almost every Deep Learning framework uses arrays or tensors.

## Difficulties

- Installing NumPy
- Understanding indexing

## Questions

- Why is NumPy faster than Python lists?
An array is a collection of homogeneous data-types that are stored in contiguous memory locations. On the other hand, a list in Python is a collection of heterogeneous data types stored in non-contiguous memory locations. The NumPy package breaks down a task into multiple fragments and then processes all the fragments parallelly.
- What is vectorization?
Vectorization is a technique used to perform operations on entire arrays at once instead of iterating through elements using Python loops. It improves performance by using optimised implementations provided by libraries such as NumPy.

import numpy as np
arr = np.array([1, 2, 3, 4, 5])

# Vectorized operation
result = arr * 2
print(result)

## Next Goal

Learn Pandas and visualize datasets.