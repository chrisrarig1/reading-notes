# File IO & Exceptions

## Reading and Writing in Python

- **What is a file composed of?**
  - Header: metadata about the file
  - Data: contents of file
  - End of File
- **File Path:**
  - Folder Path: File folder location on the system
  - File Name
  - Extension: indicates file type
- **File Methods**
  - *Characters:*
    - `r`: open for reading
    - `w`: open for writing
    - `rb` or `wb`: Open  in binary mode
  - *Opening:*
    - `open('filename', character)`
  - *Closing:*
    - `.close()`
  - *Reading:*
    - `.read(size=-1)`: reads entire file
    - `.readlines(size=-1)`: reads entire line based on size
    - `.readlines()`: returns all lines from file as a list
  - *Writing:*
    - `.write(string)`: writes given string to file
    - `.writelines(seq)`: writes the sequence given to the file

## Python Exceptions

- **Exceptions vs Syntax errors**
  - *Syntax Errors:*
    - These occur when an incorrect statement is detected
  - *Exceptions*
    - This occurs when a syntactically correct piece of python code results in an error
- **Raising an Exception**
  - This allows us to raise an error when a certain condition is met through code like:
    - `raise Exception('statement of why')` 
- **Assertion Error**
  - Implying a assertion at the beginning of the code is an easy to ensure the code runs with no issues. this is a true/false statement 
- **Try Statement**
  - This allows the code to run until an exception pops up
- **Except Statement**
  - This catches and handles the exceptions in the try statement
- **Else Statement**
  - This is the code that will run if no exceptions are encountered
- **Finally Statement**
  - This code will run whether or not exceptions are encountered 

# Useful Links

- [Python Exceptions](https://realpython.com/python-exceptions/)
- [Reading and Writing Files](https://realpython.com/read-write-files-python/)
