# reading and writing files in python

![reading](data:image/png;base64,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)

A file is a container in a computer system for storing information

**files main part**

1. Header: metadata about the contents of the file (file name, size, type,...)
2. Data: contents of the file
3. End of file : special character that indicates the end of the file

**to open a file in python**

`file = open('file_name.extension, mode')`

**mode** can hold one on this values:
1. 'r'---> means open it in read mode
2. 'w'---> means open it in write mode
3. 'b'---> means open it in binary mode 


         with open('file_name.extension', 'r') as reader:
         print(reader.readline(5))
         # to read 5 lines from the file
         reader.write('massege') # to write on the file


--------------------------------


# Python Exceptions:
exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions

*Exceptions types*:

1. ImportError: an import fails
2. IndexError: a list is indexed with an out-of-range number
3. NameError: an unknown variable is used
4. SyntaxError: the code can't be parsed properly
5. TypeError: a function is called on a value of an inappropriate type
6. ValueError: a function is called on a value of the correct type, but with an inappropriate value


**notes**
- If you want to throw an error when a certain condition occurs using raise
  `raise Exception('Msg')`
- To handle exceptions, and to call code when an exception occurs, you can use a try/except statement.
- The finally statement is placed at the bottom of a try/except statement. Code inside a finally statement always runs after execution of the code in the try, and possibly in the except.
- An assertion is a sanity-check that you can turn on or turn off when you have finished testing the program.

Ex from W3school:

      x = "hello"

      #if condition returns True, then nothing happens:
      assert x == "hello"

      #if condition returns False, AssertionError is raised:
      assert x == "goodbye"


