# f-Strings-examples

f-Strings let you add variables to your string the easy way. It is Literal String Interpolation. You need Python 3.6 or newer to use them. This is a newer way to format strings, that saves you from the unpleasant %-formatting.

## Example

Python supports multiple ways to format text strings. These include %-formatting [1], str.format() [2], and string.
Instead of having to type the %-formatting. First define some variables.

```
>>> name = "Veronica"
>>> age = 25
>>> lastname = "Sofia"
>>> job = "Teacher"
>>> relation = "Single"
```

Then you would traditionally do something like this:

```
>>> "I am %s and I am %i years old." % (name,age)
```

You can use literal string interpolation, or f-strings

```
>>> f"Im {name} {lastname}, Im {age} years old"
```
Then add multiple variables like this:
```
>>> f"Im {name} {lastname}, Im {age} years old and a {job}. Im {relation}"
```

## Why f-Strings

%-formatting can only format ints, strs, and doubles. All other types are not supported, or not converted. For example, it cannot output tuples with the %-formatting.

```
>>> msg = ('hello',13)
>>> "msg %s" % msg
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: not all arguments converted during string formatting
```

But you can output tuples with f-Strings:

```
>>> msg = ('hello',13)
>>> f"msg {msg}"
"msg ('hello', 13)"
>>>
```

You can even use it on datetime

```
>>> import datetime
>>> date = datetime.date(2010, 5, 5)
>>> f'{date} was on a {date:%A}'
'2010-05-05 was on a Wednesday'
>>> 
```
