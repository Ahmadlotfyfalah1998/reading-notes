# Q1.
List comprehension is a powerful and concise method for creating lists in Python that becomes essential the more you work with lists, and lists of lists.<br>
 three ingredients are necessary for a python list comprehension to work.<br>
1.First is the expression we’d like to carry out. expression inside the square brackets.<br>
2.Second is the object that the expression will work on. item inside the square brackets.<br>
3.Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.<br>
### Notes about Lists Comprehensions
1. List comprehension methods are an elegant way to create and manage lists. <br>
2. In Python, list comprehensions are a more compact way of creating lists. <br>
3. More flexible than for loops, list comprehension is usually faster than other methods<br>
```python
# create a list using a for loop
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

print(squares)
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```
# Q2.
a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure
# Q3.
When working on code, whether we know it or not, we often come across the decorator design pattern. This is a programming technique to extend the functionality of classes or functions without modifying them.<br> The decorator design pattern allows us to mix and match extensions easily. Python has a decorator syntax rooted in the decorator design pattern. Knowing how to make and use a decorator can help you write more powerful code.<br>
def make_pretty(func):<br>
    def inner():<br>
        print("I got decorated")<br>
        func()<br>
    return inner<br>


def ordinary():<br>
    print("I am ordinary")<br>

# Output: I am ordinary
## Things I want to know more about:
1.decorator in Python?<br>
2.list comprehension<br>
[readme](https://github.com/Ahmadlotfyfalah1998/reading-notes/blob/main/notes/read08-class.md)
