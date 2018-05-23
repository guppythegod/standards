# Python Style Guide and Standard

## Resources

- [Python Code Style](http://docs.python-guide.org/en/latest/writing/style/)
- [Docstring Conventions](https://www.python.org/dev/peps/pep-0257/)
- [Chromium Style Guide](https://www.chromium.org/chromium-os/python-style-guidelines)

Version: 3.6.5
Package Manager: pip

---

### Variables

- All variable names have to be lowercase
- Lists must contain the same type, unless there is a really good reason

```
# Bad
list = [0, 0, [0.0], 4, "hey"]

# Good
list = [0, 7, 87, 2, 4, 0 5]
```
* when dealing with data structures where you don't need to attack the data itself, use a reference

```
# Bad
list = [0, 0, 0]
print(list[2])

# Good
list = [0, 0 ,0]
workable = list
print(workable[2])
```

- Dictionaries should use `0` and `1` instead of `True` and `False`

### Functions

- All functions must be named undercase with underscores

```
# Bad
def DoSomething():
  ...

# Good
def do_something():
  ...
```
- All functions should have a docstring following this format

```
def do_something(arg1. arg2):
  """
  
  """
  ...
```
