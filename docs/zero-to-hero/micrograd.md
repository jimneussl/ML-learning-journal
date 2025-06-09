---
title: Micrograd
parent: Zero to Hero
nav_order: 1
---

# Building Micrograd

## What does micrograd do on a conceptual level?

### It builds a computational graph of all values and operations
Micrograd takes numbers as input and keeps track of the various operations (e.g., addition, multiplication) that are done on them and any of the intermediate and final results. It builds out a graph of how the various elements or nodes are connected and how they lead to the final result.

For example, let's say we have variables a, b, and c.
Let's say that:
a + b = d
c * d = e

Micrograd will now keep track of how 
1) d is a result of an addition of a and b
2) e is a result of a multiplication of c and d

We know which other values a given value stems from and through what operation is was created.

### Backpropagation




## What does micrograd do on a code level?

Overview:
- we create a Value class
- this class initialises the Value object and contains a number of things
- it handles the operations of Values, such as addition, multiplication, division, etc.
