# Reading and writing files

* Absolute vs relative paths
* linux and mac use / for folder delineation
* windows uses \
* `..` represents one folder level higher
* `.` represents this folder
* end of line in windows is lf+cr
* end of line in linux and max is just lf
* character encoding standards
  * unicode (UTF-8) vs ascii
  * ASCII is a subset of unicode

## Reading a file

Python has a built in open() function wuich takes a filepath as a parameter, and returns a file object.

Whenever you open a file, you should also close it when you are done.

There are two methods to opening and closing a file:

```py
reader = open('somefile.txt')
try:
  # do the file stuff with reader
finally:
  reader.close()
```

OR

```py
with open('somefile.txt') as reader:
  # do the file stuff with reader
```

The 2nd method is cleaner and preferred.

open() takes an optional 2nd argument as a flag for read/write/append + byte data. **If you open a file with `w` as a parameter, the original file will be deleted!**

Once a file is opened you can `read()`, ` readline()` or `readlines()` depending on your needs.

You can also `write()` and `writelines()`

Sometimes you'll want to read from one file and write to a different file at the same time, which is totally possible:

```py
with open('reading_from.txt', 'r') as reader, open('writing_to.txt', 'w') as writer:
    stuff = reader.readlines()
    writer.writelines(stuff)
```

Finally, there's lots of existing modules for reading and writing files. Use those when you can!

[<-- Back](../README.md)
