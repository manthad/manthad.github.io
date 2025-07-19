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





# if (False and True) == True:
#     print("It is an or operator")
# else:
#     print("It is not an and operator")
# elif:
#     print("It is an and operator")

# WHILE LOOP

# a = int(input("ener a number"))
# while a > 0:
#     print("The value of a is", a)
#     a += 1
#     if a == 20:
#        break

# Loops
# while(True):
#     print("hello") #- this is an infintie statement so called an infinite loop prints the hello infinitely
#     name = input()    
#     if name == 'your name':
#         break
# print ("thanks")

# CONTINUE

# a = 0
# while a < 5:
# #random has so many things like random.choice, random.shuffle, random.sample, etc. so if we do 
#     a += 1
#     if a == 3:
#         continue  # Skip the rest of the loop when a is 3. means down part will not be executed and again start at the top
#         #this will never happen
#     print("Current value of a:", a)

# FOR LOOP

# i = 0
# for i in range(5): # also can write (10,15) (2,10,2): #it starts from 0 and goes to 4
#     print ("Current value of i:", i) # the value will be from 10-14, values from 2 to 10 with a step of 2

# for i in range(10,20,2): # also can write (10,15) (2,10,2): #it starts from 0 and goes to 4
#     print ("Current value of i:", i)    

# BUILT IN FUNCTIONS:

# print, len, type, int, str, float, bool, list, dict, set, tuple
# now if we want to use any other functions then we have to import them from the module
# ex: 
# import random
# print(random.randint(1, 10)) # This will give a random integer between 1 and 10
# we are writing random. randint because randint is a function inside the random module
# from random * all the functions will be imported and we can use them directly without random.
# randint(1, 10)

# same way import sys 
# # sys.exit() # This will exit the program and not allow to continue further
# import pyperclip # this is used to copy and paste the text from the clipboard
# pyperclip.copy("Divya") # This will copy the text "Hello" to the clipboard
# pyperclip.paste() # This will paste the text from the clipboard
# print(pyperclip.paste()) 

# FUNCTION - is a mini program that can be used to perform a specific task
# now we can create our own function and can be called any number of times
# def greet(name):
#     print("Hello" + name)
#     print(name+ " " + "has "+ " "+ str(len(name)) + " letters in it")
    
# greet('dsq')
# greet('ravi')    



#  NONE datatype is used to represent the absence of a value or a null value
#    ex: print('hello') will display hello which means it returns None

# print ("hello","world", sep= 'ABC') # This will print helloABCworld
# print ("hello", end = "")
# print ("world") # now it will print hello world in the same line


# Function points:
# 1. these are like mini programs, dev statement defines a function, duplication of code is less,the parameters inside function are variables.return value can br done. if nothing is ther then it return none.
# print has end and sep arguments in it.

# Global and local variables
# inside the function anythibg defined like a =5 it is local the same one defined outside the function is global.

# eggs = 42
# def spam():
#     eggs = 99
#     print(eggs)

# spam()
# print(eggs)
  

# Error handling:
# def x(divide):
#     try:
#         result = 10 / divide
#         print("Result:", result)
#     except ZeroDivisionError:
#         print("Error: Cannot divide by zero.")

# print(x(2))
# print(x(0))  # This will trigger the ZeroDivisionError and execute the except block
# thats why we created that try and except block to handle the error gracefully because if we dont handle it it will not execte the next steps

# The  same way when we are supposed to provide an input as an int but we have provided as string then also an error called value erro will come then we can use that try and except as before


# LISTS: is a value which contains multiple values in it, it is mutable, it can be changed, it is ordered, it can contain duplicate values, it is defined by square brackets []

# b = ['apple', 'banana', 'cherry']  # This is a list of strings , a[0] will give apple, a[1] will give banana, a[2] will give cherry
# a = [['apple', 'banana', 'cherry'], [1,2,3], [10, 20, 30]] #if we want 2 then 
# print(a[1][1])
# a[1]= 40 #then it will change the value of banana of first list to 40
# print(a[1:3]) #will give the values from index 1 to 2, a[1:3] will give banana and cherry
# del a[2] #will delete the value of cherry from the list
# print (a)
# print(2 in [1,2,3]) #will return True
# print(2 not in [1,2,3]) #will return True

# LOOPS WITH LISTS::

# print(list(range(0,50,5)))
# a = [1,2,3]
# x= a[0]
# y=a[1]
# print(x, y)
# then x,y,z= absence
# so if we ask for x it will give 1, if we ask for y it will give 2, if we ask for z it will give 3 

# a,b=b,a means a will take the value of b and b will take the value of a
# Augumentation means a+=1 like that

# METHODS:
# a = [1,2,3]
# b = ['APple', 'cHErry', 'baNAna', 'orange', 'dragonfruit']
# print(a.index(1)) #answer is 0 can also use append which will add the value to the end of the list, inser will add at the specified index we mentioned 
# print(a.insert(1,7)) 
# print(a)# then i will show [1,7,2,3]
# print(a.remove(2))
# print(a) # will remove 2 only
# # del a[1] 
# print(a) #will remove 7
# a.sort()
# print(a) #will sort in ascending order
# a.reverse()
# print(a)
# b.sort(key=str.lower)
# print(b)  # This will sort the list in ascending order based on the lowercase version of the strings

# This is used for list only not normal strings

# DIFFERENCE BETWEEN LIST AND STRING:
# # list is mutable i.e. the value can be changed or replaced, string is immutable cannot be changed or replaced.
# For a string to replace the value needed like
# a = "hello"
# b = "go "+ "to "+ a[1:2]

# In string if a ='hello' and b=a then b is hello but again if a=10 then a= 10
# but in list if a=[1,2,3] and b=a then b is [1,2,3] but if b[0]=10 then a will be [10,2,3] and a will also be [10,2,3] because it is mutable (changes)
# both the a and ba re referring to same list in memory

# PASSING LISTS IN FUNCTIONS:
# def eggs(x):
#     x.append(99)

# a= [1,2,3]
# eggs(a)
# print (a)
# x= copy.deepcopy(a)  # This will create a deep copy of the list a, meaning it will create a new list with the same values but not refer to the same memory location
# if we do like this then it will not change the original list a

# LINE CONTINUATION: \ if we write this even though it is seperate line the output will be shown as a same line.



# DICTIONRIES: collection of many values with key and value pairs
# a = {'name': 'John', 'age': 30, 'city': 'tokyo'}
# print(a['name']) #will give John, a['age'] will give 30
# print(a['age'])
# if 2 dictioneries have same values but jumble if it is numbers then it is not equal but they are string then eqal like

# a = {'name': 'John', 'age': 30, 'city': 'tokyo'} and b= {'age': 30, 'city': 'tokyo', 'name': 'John'} #both are same
# name in a will give True, a.name() will give John

# print(list(a.keys())) #will give the keys of the dictionary, list(a.values()) will give the values of the dictionary a
# print(list(a.values())) # will give the values of the dictionary a (like john in one age and 30 in one bracket like that) 
# list(a.items()) #will give the items of the dictionary a (like a pair name and john in one age and 30 in one bracket like that)

# for k in a.keys():
#     print (k) # will print all the keys one after other in column
# for k,v in a.items():
#     print(k,v)
    # print(i) #means both keys and vlaues in single quotes.

# a.get('name') will give the value of name, a.get('age') will give the value of age

# a.setdefault('name', 'dsq') will set the value of name to dsq if it is not already present, if it is present then it will not change the value

# CHARACTER COUNTING PROGRAM:
# import pprint
# import collections
# from collections import Counter
# char = "I love to go to gym"
# count = {} #this is an empty dictionary

# for i in char:
#     count.setdefault(i, 0)  # This will set the value of i to 0 if it is not already present
#     count[i] += 1  # This will increment the value of i by 1
#     print(count) # This will print the dictionary with the count of each character like {'I': 1, ' ': 5, 'l': 2, 'o': 3, 'v': 1, 'e': 1, 't': 2, 'g': 1, 'y': 1, 'm': 1}

# Counter(char) # will give the same output as above but it is from collections module so we have to import it first

# pprint.pprint(count) # will print the dictionary with the count of each character like {'I': 1, ' ': 5, 'l': 2, 'o': 3, 'v': 1, 'e': 1, 't': 2, 'g': 1, 'y': 1, 'm': 1} will display the same data in column

# DATA STRUCTURES: list of dictionories
# a = [{'name': 'John', 'age': 30}, {'name': 'Jane', 'age': 25}, {'name': 'Doe', 'age': 35}]
# to have more than one value in dictionary because if same type of date then so many lists or dictionaries are to be created.

# ADVANCED STRINGS:
# in this we use "" instead of '' as while writing we may have words with '' and it creates confusion.
# but u can also write like 'Hi this is Divya\'s mother'
# \' - prints as single quote
# \" - prints as double quote
# \\ - prints as backslash
# \n - prints as new line
# \t - prints as tab space
# print("Hello World. I am Divya\'s mother who is a \"lawyer. \n I love my kid.") 

# RAW STRING: which starts with r or R before string.

#STRING METHODS:  unlike list string will create a new string but not change the original string ex:
# a ="Hello World"
# b = a.upper() # This will create a new string with all the characters in uppercase
# c = a.lower()
# print(b)
# print(c)
# print(a.islower())
# print(a.istitle()) #means all the words in a statement starts with a capital letter
# print(a.startswith('H'))
# print(a.endswith('o')) #, ','.join[a, b, c] = a,b,c \n\n.join[a, b, c] = print a b and c in different lines
#"Hi DSQ".split() # splits string into list
# if mentioned "hello world".split(l) - then ;'he' , 'o' , 'w', 'o', 'r',  'd'
# ljust() #- add spaced and move the text towards left, ljust(5,'-') means hello-----
# rjust() #- add spaced and move the text towards right
# center() #same like above
# strip(), lstrip(), rstrip() - opp of just it will remove the extra spaces or anything that gor geneated by ljust or rjust.
# a.replace( 'e', 'hel')

# "Hello %s. You are invited to %s at %s on %s." %s(name, place, time, day) all these things can be provided before only as name ='Rupa'like that.

# FILES:
# path() in pathlib module will take care of all the OS. better use /

from pathlib import Path 
import os

Path('a','b', 'c') # o/p a/b/c
str(Path('a','b', 'c')) # will give output as a\\b\\c
from pathlib import Path
my_files = ['accounts.txt', 'details.csv', 'invite.docx']
for filename in my_files:
    print(Path(r'C:\Users\Al', filename)) # willprint all the files one after other with the mentioned path

Path.cwd() #prints cwd
os.chdir('/Users/divyamantha/Documents/python')


# EXCEL:

# openpxl should be imported to work with excel
# pip install openpyxl
# import openpyxl
# import os
# os.chdir('/Users/divyamantha/Documents/python')

# workbook =openpyxl.load_workbook('example.xlx')
































































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




