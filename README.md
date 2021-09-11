Python-Generators
U-Tech Advance Python with Data Science

# What are Generators?
Python generators are a simple way of creating iterators. All the work we mentioned above are automatically handled by generators in Python.

Simply speaking, 
## A generator is a function that returns an object (iterator) which we can iterate over (one value at a time).

Generator is as easy as defining a normal function, but with a yield statement instead of a return statement.

If a function contains at least one yield statement (it may contain other yield or return statements), it becomes a generator function. Both yield and return will return some value from a function.

The difference is that while a return statement terminates a function entirely, yield statement pauses the function saving all its states and later continues from there on successive calls.

# Use of Python Generators
There are several reasons that make generators a powerful implementation.

## 1. Easy to Implement
Generators can be implemented in a clear and concise way as compared to their iterator class counterpart. Following is an example to implement a sequence of power of 2 using an iterator class.

## 2. Memory Efficient
A normal function to return a sequence will create the entire sequence in memory before returning the result. This is an overkill, if the number of items in the sequence is very large.

Generator implementation of such sequences is memory friendly and is preferred since it only produces one item at a time.

## 3. Represent Infinite Stream
Generators are excellent mediums to represent an infinite stream of data. Infinite streams cannot be stored in memory, and since generators produce only one item at a time, they can represent an infinite stream of data.

# Differences between Generator function and Normal function
Here is how a generator function differs from a normal function.

1) Generator function contains one or more yield statements.
2) When called, it returns an object (iterator) but does not start execution immediately.
3) Methods like __iter__() and __next__() are implemented automatically. So we can iterate through the items using next().
4) Once the function yields, the function is paused and the control is transferred to the caller.
5) Local variables and their states are remembered between successive calls.
6) Finally, when the function terminates, StopIteration is raised automatically on further calls.
