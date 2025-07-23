---
layout: page
title: ""
permalink: /basics-of-python/
---

LET US START THE PYTHON BASIC COURSE WITH RESPECTIVE PROGRAMS

**1. BASIC PROGRAM WITH PRINT AND INPUT:**
<pre>
<i> print("Hey What is your name?”)
name = input()
print("Nice to meet you"+ name)
print("Nice to meet you, " + name + "Do you want to find the letters in your name 
and other data? ")
option = input("Type yes or no”) </i></pre>

<pre><i> if option.lower() == 'yes':
  print("the number os letters in your name is" +" "+ str(len(name.replace(" ", ""))))
  print ("what is your birth year?")
  birth_year = input()
  print ("Current year?")
  year = input()
  age = int(year) - int(birth_year)

  print("Your age is" + str(age))
else: 
    print("Ok, have a nice day!") </i></pre>


    