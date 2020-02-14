# f-Strings-examples

f-Strings let you add variables to your string the easy way. It is Literal String Interpolation. You need Python 3.6 or newer to 
use them.

## Example

Python supports multiple ways to format text strings. These include %-formatting [1], str.format() [2], and string.
Instead of having to type the %-formatting like this:

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
