---
layout: post
title:  "Welcome to Python course"
date:   2025-07-18 11:11:41 +0530
categories: jekyll update
---
# Introduction

Python is a powerful and easy-to-learn language:
## Here are the few concepts we cover during this python course

<!-- # print("Heyyy What is your name?")
# name = input()
# print("Nice to meet you"+ name)
# print("Nice to meet you, " + name + "Do you want to find the letters in your name and other data? ")
# option = input("Type yes or no")
# if option.lower() == 'yes':
#   print("the number os letters in your name is" +" "+ str(len(name.replace(" ", ""))))
#   print ("what is your birth year?")
#   birth_year = input()
#   print ("Current year?")
#   year = input()
#   age = int(year) - int(birth_year)

#   print("Your age is" + str(age))
# else: 
#     print("Ok, have a nice day!") -->




LET US START THE PYTHON BASIC COURSE WITH RESPECTIVE PROGRAMS

1. BASIC PROGRAM WITH PRINT AND INPUT:

print("Hey What is your name?”)
name = input()
print("Nice to meet you"+ name)
print("Nice to meet you, " + name + "Do you want to find the letters in your name 
and other data? ")
option = input("Type yes or no”)

if option.lower() == 'yes':
  print("the number os letters in your name is" +" "+ str(len(name.replace(" ", ""))))
  print ("what is your birth year?")
  birth_year = input()
  print ("Current year?")
  year = input()
  age = int(year) - int(birth_year)

  print("Your age is" + str(age))
else: 
    print("Ok, have a nice day!")


2. OPERATORS:
    These are basic and, or and not operators

if (False and True) == True:
    print("It is an or operator")
else:
    print("It is not an and operator")
elif:
    print("It is an and operator”)


The outputs will print TRUE or FALSE based on the logic provided


3. LOOPS

   a) While Loop

a = int(input("ener a number"))
while a > 0:
    print("The value of a is", a)
    a += 1
    if a == 20:
       break


while(True):
    print("hello")   
    name = input()    
    if name == 'your name':
        break
print (“thanks")

this is an infinite statement so called an infinite loop prints the hello infinitely.
It will stop only if the name is provided as ‘your name’

Continue

a = 0
while a < 5:
#random has so many things like random.choice, random.shuffle, random.sample, etc. so if we do 
    a += 1
    if a == 3:
        Continue       # Skip the rest of the loop when a is 3. means down part will not be executed and again start at the top
                                    
    print("Current value of a:", a)

=> So the output would be 1 2 4 5




b) For Loop

i = 0
for i in range(5):                                 
    print ("Current value of i:", i)           

=> o/p is 0 1 2 3 4 

for i in range(10,20,2):                         # the value will be from 10-20  with a step of 2
    print ("Current value of i:", i)    

=> o/p is 10 12 14 16 18 

BUILT IN FUNCTIONS:

print, len, type, int, str, float, bool, list, dict, set, tuple are the examples which are provided by python and can directly be used.

If we want to use any other functions then we have to import them from the module
EX 1:
import random
print(random.randint(1, 10))                         # This will give a random integer between 1 and 10

=> we are writing random. randint because randint is a function inside the random module
     If we want all the internal functions related to random then we need to import random * then 

randint(1, 10).   # can directly be used

EX 2:
import sys 
sys.exit()                                           # This will exit the program and not allow to continue further
import pyperclip                              # this is used to copy and paste the text from the clipboard
pyperclip.copy("Divya")                   # This will copy the text "Hello" to the clipboard
pyperclip.paste()                              # This will paste the text from the clipboard
print(pyperclip.paste()) 


FUNCTION - is a mini program that can be used to perform a specific task
now we can create our own function and can be called any number of times

Example if we want to do a particular task again and again then no need to write the code several times instead can
Write one function with the task we need and call it again and again

def greet(name):
    print("Hello" + name)
    print(name+ " " + "has "+ " "+ str(len(name)) + " letters in it")
    
greet('dsq')
greet('ravi')    

=> O/p is Hello dsq
                Dsq haș 3 letters in it 


 NONE  datatype is used to represent the absence of a value or a null value
   ex: print('hello')                   # will display hello which means it returns None

print ("hello","world", sep= 'ABC')                # This will print helloABCworld
print ("hello", end = "")
print ("world")                              # now it will print hello world in the same line


GLOBAL AND LOCAL VARIABLES:

Inside the function anything defined like a =5 it is local the same one defined outside the function is global.

eggs = 42        # global
def spam():
    eggs = 99    # local
    print(eggs)

spam()           # o/p is 99
print(eggs)    # o/p is 42
  

ERROR HANDLING:

def x(divide):
    try:
        result = 10 / divide
        print("Result:", result)
    except ZeroDivisionError:
        print("Error: Cannot divide by zero.")

print(x(2))
print(x(0))                        # This will trigger the ZeroDivisionError and execute the except block
                                         thats why we created that try and except block to handle the error gracefully because 
                                         if we don’t handle it it will not execute the next steps

The  same way when we are supposed to provide an input as an int but we have provided as string then also an error 
called value error will come then we can use that try and except as before


LISTS:   is a value which contains multiple values in it, it is mutable, it can be changed, it is ordered,
              it can contain duplicate values, it is defined by square brackets [ ]

b = ['apple', 'banana', 'cherry']           # This is a list of strings , a[0] will give apple, a[1] will give banana, a[2] will give cherry
a = [['apple', 'banana', 'cherry'], [1,2,3], [10, 20, 30]]         #if we want value 2 then 
print(a[1][1])

a[1]= 40                  #then it will change the value of banana of first list to 40
print(a[1:3])             #will give the values from index 1 to 2, a[1:3] will give banana and cherry
del a[2]                    #will delete the value of cherry from the list
print (a)
print(2 in [1,2,3])             #will return True
print(2 not in [1,2,3])       #will return True





LOOPS WITH LISTS:

print(list(range(0,50,5)))     # it will print the numbers fro 0 to 50 with step of 5 in list format [0,5,10,15..45]
a = [1,2,3]
x=  a[0]
y= a[1]
print(x, y)
then x, y, z = absence
so if we ask for x it will give 1, if we ask for y it will give 2, if we ask for z it will give 3 

a, b = b, a means a will take the value of b and b will take the value of a
Augmentation means a+=1 like that

METHODS:
a = [1,2,3]
b = ['APple', 'cHErry', 'baNAna', 'orange', 'dragonfruit']
print(a.index(1))               #answer is 0 can also use append which will add the value to the end of the list, 
print(a.insert(1,7))            # inser will add at the specified index we mentioned
print(a)                             # o/p is [1,7,2,3]
print(a.remove(2))
print(a)                            # o/p [1, 7, 3]
del a[1] 
print(a)                         # o/p [1, 3]
a.sort()
print(a)                         #will sort in ascending order
a.reverse()
print(a)                         # o/p [3, 1]
b.sort(key=str.lower)    
print(b)                        # This will sort the list in ascending order based on the lowercase version of the strings

This is used for list only not normal strings






DIFFERENCE BETWEEN LIST AND STRING:
 List is mutable i.e. the value can be changed or replaced, string is immutable cannot be changed or replaced.
For a string to replace the value needed like

a = "hello"
b = "go "+ "to "+ a[1:2]

In string if a ='hello' and b=a then b is hello but again if a=10 then a= 10
but in list if a=[1,2,3] and b=a then b is [1,2,3] but if b[0]=10 then a will be [10,2,3] and a will also be [10,2,3] because it is mutable (changes)
both the a and b are referring to same list in memory

PASSING LISTS IN FUNCTIONS:

def eggs(x):
    x.append(99)

a= [1,2,3]
eggs(a)
print (a)
x= copy.deepcopy(a)  # This will create a deep copy of the list a, meaning it will create a new list with the same values but not
                                      refer to the same memory location
if we do like this then it will not change the original list a

LINE CONTINUATION: \ if we write this even though it is separate line the output will be shown as a same line.



DICTIONARIES:  collection of many values with key and value pairs

a = {'name': 'John', 'age': 30, 'city': 'tokyo'}
print(a['name']) #will give John, a['age'] will give 30
print(a['age'])
if 2 dictioneries have same values but jumble if it is numbers then it is not equal but they are string then eqal like

a = {'name': 'John', 'age': 30, 'city': 'tokyo'} and b= {'age': 30, 'city': 'tokyo', 'name': 'John'} #both are same
name in a will give True, a.name() will give John

print(list(a.keys()))                    #will give the keys of the dictionary    [‘name’, ‘age’]
print(list(a.values()))                  # will give the values of the dictionary a [‘John’, ’30’]
list(a.items())                            #will give the items of the dictionary a [‘name’, ‘John’] [‘age’, ’30’]

for k in a.keys():
    print (k)                          # will print all the keys one after other in column
for k,v in a.items():
    print(k,v)
    print(i)                            #means both keys and values in single quotes.

a.get('name')                    # will give the value of name, a.get('age') will give the value of age

a.setdefault('name', 'dsq')  # will set the value of name to dsq if it is not already present, if it is present then it will not change the value

CHARACTER COUNTING PROGRAM: 
pprint is used to display in nice format

import pprint
import collections
from collections import Counter
char = "I love to go to gym"
count = {}                                  #this is an empty dictionary

for i in char:
    count.setdefault (i, 0)          # This will set the value of i to 0 if it is not already present
    count[ i ] += 1                     # This will increment the value of i by 1
    print(count)                        # This will print the dictionary with the count of each character like
  O/p  {'I': 1, ' ': 5, 'l': 2, 'o': 3, 'v': 1, 'e': 1, 't': 2, 'g': 1, 'y': 1, 'm': 1}

Counter(char)                     # will give the same output as above but it is from collections module so we have to import it first

pprint.pprint(count)             # will print the dictionary with the count of each character like
                                            {'I': 1, ' ': 5, 'l': 2, 'o': 3, 'v': 1, 'e': 1, 't': 2, 'g': 1, 'y': 1, 'm':1} will display the same data in column




DATA STRUCTURES:  list of dictionaries

a = [{'name': 'John', 'age': 30}, {'name': 'Jane', 'age': 25}, {'name': 'Doe', 'age': 35}]
to have more than one value in dictionary because if same type of date then so many lists or dictionaries are to be created.

ADVANCED STRINGS:
in this we use “ "  instead of ‘ ' as while writing we may have words with '' and it creates confusion.
but you can also write like 'Hi this is Divya\'s mother'
\' - prints as single quote
\" - prints as double quote
\\ - prints as backslash
\n - prints as new line
\t - prints as tab space
print("Hello World. I am Divya\'s mother who is a \"lawyer. \n I love my kid.") 

O/p Hello World. I am Divya's mother who is a “lawyer”.
       I love my kid.

RAW STRING: which starts with r or R before string.

STRING METHODS:  unlike list string will create a new string but not change the original string ex:
a ="Hello World"
b = a.upper()                     # This will create a new string with all the characters in uppercase
c = a.lower()
print(b)
print(c)
print(a.islower())                # O/p is true or false
print(a.istitle())                  # means all the words in a statement starts with a capital letter
print(a.startswith('H'))
print(a.endswith('o'))        #, ','.join[a, b, c] = a,b,c \n\n.join[a, b, c] = print a b and c in different lines

"Hi DSQ".split()                # splits string into list
if mentioned "hello world".split(l) - then ;'he' , 'o' , 'w', 'o', 'r',  ‘d'

ljust()           #- add spaced and move the text towards left, ljust(5,'-') means hello-----
rjust()          #- add spaced and move the text towards right
center()      #same like above
strip(), lstrip(), rstrip()    # opp of just it will remove the extra spaces or anything that gor geneated by ljust or rjust.
a.replace( 'e', 'hel')

"Hello %s. You are invited to %s at %s on %s." %s(name, place, time, day) all these things can be provided 
before only as name =‘Rupa' like that.

FILES:
path() in pathlib module will take care of all the OS. better use /

print("/Users/divyamantha/Documents/python")
print(‘//‘)        o/p is //
print(‘\\')        o/p is \ for windows
to create file path using individual strings we can do like '/'.join(['folder1', 'folder2', 'file.png'])
this will print like 'folder1/folder2/file.png' 
but this cannot be used on other os except windows so thats why few things.we are importing os

import os
print(os.path.join('folder1', 'folder2', 'file.png'))             # works same
print(os.getcwd())                                                           # o/p current working directory
os.chdir(‘/Users/divyamantha/Documents')                  #will change the directory to mentioned

print(os.path.abspath('test.py'))                                   # will give the abs path of test.py 
                                                                                    # isabs() used to check whether that is abs or not
print(os.path.relpath(‘/python/test.py'))                       # if we want only part of the path then
O/p : /Users/divyamantha/Documents/python
              
print(os.path.dirname('/Users/divyamantha/Documents/python/test.py'))             # gives directory path till file
print(os.path.basename(‘/Users/divyamantha/Documents/python/test.py'))         # gives file name
print(os.path.exists('/Users/divyamantha/Documents/python/test.py'))
print(os.path.isfile(‘/Users/divyamantha/Documents/python/test.py'))                   # if its file print TRUE
print(os.path.isdir(‘/Users/divyamantha/Documents/python/test.py'))                   # if its dir print TRUE
print(os.path.isdir('/Users/divyamantha/Documents/python'))
print(os.path.getsize('/Users/divyamantha/Documents/python/test.py'))              #size of the file
print(os.listdir('/Users/divyamantha/Documents')) 

we have abs (full we need to give i.e. root) and relative paths (only from cwd)
. means this directory .. means parent directory 

Program to find all the files or folders in a particular folder

dirSize = 0
fileSize = 0
for dirname in os.listdir('/Users/divyamantha/Documents'):
    if os.path.isdir(os.path.join('/Users/divyamantha/Documents', dirname)):
        print ("Found Dir - ", os.path.join(‘/Users/divyamantha/Documents', dirname))
        dirSize += 1
print(dirSize)         
for filename in os.listdir('/Users/divyamantha/Documents'):
    if not os.path.isdir(os.path.join('/Users/divyamantha/Documents', filename)):
        print("Found File -- ", os.path.join(‘/Users/divyamantha/Documents', filename))
        fileSize += 1
print(fileSize)   

os.makedirs('./Documents/filefolder')
print(os.path.abspath('./Documents/filefolder'))


Plain text files and Binary files:

- the files which have only text and which is .txt
  binary are files which are not at all understanble and have some random symbols

x = open(‘/Users/divyamantha/Documents/file.txt')          # will open the file
print(x.read())
print(x.close())
x = open('/Users/divyamantha/Documents/file.txt', ‘w')   # will open file in write mode
print(x.readlines())
print (x.write("I am feeling good"))
print(x.close())
x = open('/Users/divyamantha/Documents/file.txt', ‘a')   # will open file in append mode i.e. add whatever in the last
print (x.write("\n But will take time to recover"))
print (x.write("\nTime heals everything. So be strong"))
print(x.close())

import shelve                  # instead of normal data if we want to store data like a program which has 
                                          complex data or symbols then use this

sf= shelve.open('mydata')
sf['students'] = ['ram', 'shyam', 'sam']
# sf.close()
print(sf['students'])
print(list(sf.keys()))                  # same like dictionary it will give only keys data
print(list(sf.values()))

import shutil                   # shell util is used for copy, paste kind of functions
shutil.copy('/Users/divyamantha/Documents/file.txt', '/Users/divyamantha/Documents/python/file.txt')
print(os.getcwd())
shutil.copytree('/Users/divyamantha/Documents', '/Users/divyamantha/Documents_backup')         # if to copy all the files and folders
shutil.move()
print(os.getcwd())

os.unlink('/Users/divyamantha/Documents/python/file.txt')            # to delete the file
os. rmdir(‘/Users/divyamantha/Documents_backup')                     # to delete the dir if its empty but if it has files or folders then
shutil.rmtree('/Users/divyamantha/Documents_backup')
os.chdir('/Users/divyamantha/Documents')

for filename in os.listdir():
    if filename.endswith('.rxt'):
        print(filename)

there is also called send2trash first we need to dwnld as pip install and then import here
then it will send that file to trash
send2trash.send2trash(......)]

Normally to find out whether its file or not we need to write big program but if we import walk then 
it will only validate whether it is a folder or a file and segregates accordingly.





for foldername, subfolders, filenames in os.walk('/Users/divyamantha/Desktop'):
    print('the folder is'+ str(foldername)+ "\n")

    print('the subfolders in folder are'+ str(subfolders)+"\n")

    print('the file under sub folder is'+ str(filenames)+"\n")
    


Raise - these are after the output got created then informing the error but try and except are like before giving output only it will say

def boxPrint(symbol, width, height):
    if len(symbol) != 1:
       raise Excpetion ("Should be the symbol with lenght 1") 

    print(symbol * width)
    for i in range (height-2):
        print(symbol+(' ' * (width-2))+symbol) 
    print(symbol * width)
boxPrint('##', 10, 5)



EXCEL, WORD AND PDF:

EXCEL :

openpxl should be imported to work with excel
pip install openpyxl 
import openpyxl
from openpyxl import load_workbook
import os
os.chdir('/Users/divyamantha/Documents/python')

workbook = load_workbook('/Users/divyamantha/Documents/python/example.xlsx') # to open we are using load_workbook
print(type(workbook))
# from workbook we need a worksheet:
sheet = workbook.active                       # if i want to use the first sheet irrespective of its name
print(workbook.sheetnames) 
cell = sheet['C4']
print(cell.value)
print(sheet.cell(row =4, column =4))


EDITING THE EXCEL OR CREATING A NEW EXCEL

wb = openpyxl.Workbook()                 # like creating an workbook object
print(wb)
sheet = wb.active
print(sheet)
sheet.title = "Street food"
sheet['A1'] = "Name"
sheet['B1'] = "Place"
sheet['C1'] = "Rate"
sheet['A2'] = "Idli"
sheet['B2'] = "DLF"
sheet['C2'] = "50"

food = wb.save('/Users/divyamantha/Documents/python/street_food.xlsx')
print(openpyxl.load_workbook('/Users/divyamantha/Documents/python/street_food.xlsx'))


READING
import PyPDF2
os.chdir('/Users/divyamantha/Downloads')
print(a)
pdfFile = open('Samplepdf.pdf')
x = PyPDFF2.PdfFileReader(pdfFile)          # this can read the pdf file
print(x.numPages)                                     # will tell how many pages are there in that pdf





EMAIL:
import smtplib
conn = smtplib.SMTP('smtp.gmail.com', 587)              # this is variable used to connect what kind of server
print(type(conn))
print(conn)
print(conn.ehlo())                      # to start the connection
print(conn.starttls())                  #to start TLS to send the password and it is encypted

need to complete later using some password app or like that as this is not secure


now checking the same mail in the inbox:
IMAP: Internet message access protocol tells or used to how to retrieve emails
just like import stmplib

import imaplib                but instead this we are using imaplib client and pyzmail
pip install imaplib and pyzmail
conn = smtplib.SMTP('imaplib.gmail.com', ssl=True)           # telling like we want to use ssl that's why its mentioned as yes
conn.login('un', 'pwd')
conn.select_folder('INBOX', readonly = True)
UIDs = conn.search(['SINCE 20-AUG-2015'])                      # asking the mails which are from that date provides all the UIDs
rawMessage = conn.fetch([any UID number], ['BODY[]', 'FLAGS'])    # when wanted to check the data in that particulat UID
import pyzmail            - learn again



















































<!-- You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/ -->




