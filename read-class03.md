## Q1.  The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error
## it allows for cleaner code and makes handling any unexpected errors easier for you.

## Q2. The .read() would treat each character in the file separately, meaning that the iteration would happen for every character.
## The readline() function only reads a single line of the file. This means that if the file file_1 were three lines long,
## the readline() function would only parse (or iterate/operate) on the first line of the file.
### ex
#### 1.file_1 = open('file', 'r')
#### for i in file_1.read():
#### do
#### 2.file1 = open('myfile.txt', 'r')
#### Lines = file1.readlines()
## Q3. when a Python script encounters a situation that it cannot cope with, it raises an exception. An exception is a Python object that represents an error.
## When a Python script raises an exception, it must either handle the exception immediately otherwise it terminates and quits
#### try block: lets you test a block of code for errors.
#### except block: lets you handle the error.
#### finally block: lets you execute code, regardless of the result of the try- and except blocks.
## ex 
### 1.try and except
try:
  print(x)
except NameError:
  print("Variable x is not defined")
except:
  print("Something else went wrong")
### 2.finally
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
 #### from "w3 schools"
