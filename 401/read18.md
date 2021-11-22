# regular expression
sequence of characters used to check whether a pattern exists in a given text (string) or not.

you can use it by import `re` library

simple ex: 

    import re
    pattern = r"Cookie" # which has the word/char i will search for it
    sequence = "Cookie" # string that will search on
    if re.match(pattern, sequence):
        print("Match!")
    else: print("Not a match!")

**notes**

- The `match()` function returns a match object if the text matches the pattern. Otherwise, it returns None
- `r` at the start of the pattern, called a raw string literal
- [abc] - Matches a or b or c.
- [a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).
- \w - Lowercase 'w'. Matches any single letter, digit, or underscore.
- \W - Uppercase 'W'. Matches any character not part of \w (lowercase w).
- \s - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.
- \S - Uppercase 'S'. Matches any character not part of \s (lowercase s).
- \d - Lowercase d. Matches decimal digit 0-9.
- \D - Uppercase d. Matches any character that is not a decimal digit.
- \t - Lowercase t. Matches tab.
- \n - Lowercase n. Matches newline.
- \r - Lowercase r. Matches return.
- \A - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.
- \Z - Uppercase z. Matches only at the end of the string.


----------------------------


# shutil — High-level File Operations

**notes**

- `copyfile()` copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
- The `copy()` function interprets the output name like the Unix command line tool cp.
- To copy the permissions from one file to another, use `copymode()` 
- To copy other metadata about the file use `copystat()`
- To copy a directory from one place to another, use `copytree()`
- 



***resources***

[python-regular-expression](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

[shutil](https://pymotw.com/3/shutil/)