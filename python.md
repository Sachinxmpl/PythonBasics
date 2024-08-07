## What is python

- Python is a dynamically typed, general purpose programming language that supports an object-oriented programming approach as well as a functional programming approach.
- Python is an interpreted and a high-level programming language.
- It was created by Guido Van Rossum in 1989.

## Features and usuage of python

- Possible to integrate other programming lnaguages wihtin python
- Used in data analytics
- Ai and Machine learning as well as web applications

## First program

- print("hello python world")
- print if built in function to display output

### Comments in python

- single line comment ( #this is single line comment )
- multiline line ("""
  This multiline comment in python
  """)

### Escape squence characters

- To insert characters that cannot be directly used in a string , we use an escape sequence character
- An escape seqeunce character is a backslash (\) followed by the character you want to insert

```python

    # Using escape sequence character
    print(" I am a guy \" interesting \"")
    print(" The cow is animal \n And it has four legs")
```

### Print statement

The syntax of print statement looks like this
print(object(s) , sep= , end= , file = )

### Parameters on print statement

- Object(s) anu object and as many as you like . Will be converted to string before printed
- sep ="separator" specify how to separate the object in case of more than one object
- end = "end" specify what to print at the end. The default is "\n"

```python
 print("sacihn", "shamsher" , sep=" and " , end="are good friends")
```

### Variables and Data types in python

Variable is a container

- a = 1
- b = True
- c = "harry"
- d = None

### Datatypes

- Numeric data : int , float , complex
  a = 5
  b = 5.666
- Boolean data
  a = True , b = False
- String
  a = "hello python programming "

```python
a = 5
print(a)
print(type(a))    //<class 'int'>

c = -5.323
print(c)
print(type(c))   //<class 'float'>

d = complex(8,2)
e = 5
print(type(d))   // <class 'complex'>

print(d+e)

b = True
print(b)
print(type(b))  //<class 'bool'>

```

- List
  A list is an ordered collection of data with elements separated by a comma and enclosed within square brackets. Lists are mutable and can be modified after creation.
  Class List

```python
list = [3,4,"this is good"]
print(list)
print(type(list))    //<class 'list'>

//Lists are mutable and hence can be changed
```

- Tuple
  A tuple is an ordered collection of data with elements separated by a comma and enclosed within parentheses. Tuples are immutable and can not be modified after creation.

```python
tuple1 = (("parrot , sparrow") , ("children"))
print(tuple1)
print(tuple1[0][1])
print(type(tuple1))
```

### A dictionary is an unordered collection of data containing a key:value pair. The key:value pairs are enclosed within curly brackets.

```python
person1 = {
    "name" : "sachn" ,
    "age" : 17  ,
    "class" : "bachelor"
}
print(person1)
print(type(person1))
print(person1["name"])
print(person1["age"])
print(person1.get("name"))
```

### Multiple variable assignment in python

```python
the code name = "sachin"
age = 18 ,
class = True ,

is replaced by

name , age , class = "sachin" , 18 , True ;

name = age = cla = True
```

### Operators in python

Arithmetic operators
Operator Operator Name Example

```python
- Addition 15+7

* Subtraction 15-7

- Multiplication 5\*7
** Exponential 5**3
/ Division 5/3
% modulus 15%7
// Floor Division 15//7
```

### Typecasting in python

Explicit type casting of valid datas , done by user

```python
a = "1"
b = "2"
print(int(a) + int(b))
```

Implicit type casting ,by python

```python
c = 1.3
b = 4
a = b + c
print(type(a))
print(type(c))
print(type(b))
```

### Taking input in python

Using input and return value as string/character

```python
a = input("Enter a number")
b = input("Enter a number")

print(a + b)
print(int(a) + int(b))
```

# String

ANything encloded that you enclosed in a double or single quotation mark

```python
name="sachin"
print(type(name))
print("heelo" + name)
print(name[0])

for character in name :
    print(character)
print('he said , "it is raining"')


# multiline stirng
multiline = '''hey
i am multiple
line string
'''
print(multiline)
```

### String handeling functions

```python
#string methods  string are immutable
Name = "sachin"
print(len(Name))  #length of string
print(Name.upper())
print(Name.lower())
print(Name.capitalize())

age = "SACHIN"
classd = "sachin"
print(age.swapcase())
print(classd.swapcase())

str = " Silver spoon "
#strip method is same as trim() in js
print(str.strip())
print(str.replace("Silver" , "khatri"))

str2 = "i am going to get into array , list "
print(str2.split(" "))

str3 = "i am double a aa "
print(str3.count("a"))

#slicing in string
print(Name[0:4]) #prints from index 0 to 3  , 4 is excluded
print(Name[:4])
print(Name[-4 : 3])

str5 = "welcome to the console !!!"
print(str5.endswith("!!!"))
print(str5.find("welcome"))

#istitle() rturns True if first letter of each word is capitalized
a = "Wold Health Organizatoin"
print(a.istitle())

#isalpha() check if alphaumeic
print("sachin".isalpha())
print("sachin khatri".isalpha())

#islower() isupper() check it the case is lower or upper

#.title() converts to title
print("hi i am sachin".title())
```

# Conditional statements

```python
name = "schin"
if(len(name) < 10 ):
    print("short name ")
else :
    print("long name ")
```

## Math Case statement

```python
x = int(input("Enter the number"))

match x :
    case 0 :
        print("YOu types 0 ")
    case 1 :
        print("You types 1 ")
    case _ if x % 2 == 0 :
        print("It is even ")
    case _ :
        print("Default case ")
```

### Loops

```python
#For loop
name = "sachin"
for i in name :
    print(i)

colors = ["red" , "yellow" ,"orange","pink"]
for color in colors :
    for i in color :
        print(i)

#can also define range include 2 excluedes 10
#range parameters range(start , end , range )
for k in range(2,10):
    print(k)
print("brak")
for k in range(1, 12, 3):
  print(k)


#While loop , we can also use else statement
count =5
while(count> 0) :
    print(count)
    count = count -1
else :
    print("Count is 0 ")

```

# Functions

```python
#we can also pass the function
def hi():
  pass


def helper (a , b) :
  if( a == b ) :
    print ("a and b are same")
  elif (a > b) :
    print(" a is greate than b")
  else :
    print("b is greater than a ")

helper(10,10)



#Defual arguments
#We can provide the keyword argument in form key:ValueError
#The order doesnot matter

def greet(name="sachin" , age  = 10 ) :
  print("Hi" , name  , age)
greet(age = 18 , name ="bhim")

#takes input as a tuple
def name(*name) :
    print(name)
    print(type(name))
    print(name[0] , name[1] , name[2])
name ("sachin" , "kahtri" , "lami")

#takes input as a dictionary

def dic(**name) :
  print(name)
  print(type(name))
  information = name["fname"] + " " + name["lname"]
  return information


info = dic(fname ="sachin" , lname="khatri")

```

# Lists in python

lists are mmutable

```python
list = [1,2,3,4,5]
#print(list[start : end : step])  end is exclueed
print(list[0:5:1])

for val in list :
  print(val)

names = ["Milo", "Sarah", "Bruno", "Anastasia", "Rosa"]
namesWith_O = [item for item in names if (len(item) > 4)]
print(namesWith_O)

age = [1 , 20 , 35 , 12, 30]
senior = [ item for item in age if item > 18 ]
print(senior)
```

### Some list methods in python

```python
num = [3,4,2,3,6,45,34,2,4,5,34,23]
num.sort()
print(num)

num.append("sachin")
print(num)


num2=[3,23,2,4,45,324,23,54,34,2,65,3]
num2.sort(reverse=True)
print(num2)

names=["sachin" , "klhatir" , "is" , "laxy"]
names.reverse()
print(names)


sample=["sachin" , "rohan" , "rohan" ,  "shrishti"]
#finds the index of element
print(sample.index("sachin"))
print(sample.count("rohan"))


#copy return the copy of list
real = [1,2,3,4,5,56]
#copy = real  if ( we do so then both copy and real point to the same list )
copy = real.copy()
copy[0]="edited"
print(copy)
print(real)

#insert method()
colors = ["voilet", "indigo", "blue"]
#           [0]        [1]      [2]
colors.insert(1, "green")   #inserts item at index 1
# updated list: colors = ["voilet", "green", "indigo", "blue"]
#       indexs              [0]       [1]       [2]      [3]
print(colors)


#concat two list
colors = ["voilet", "indigo", "blue"]
color2 = ["green", "yellow", "orange", "red"]
concat = colors + color2
print(concat)
```

# Tuples in python

Tuples are immutable and must contain atleast one comma
Least element is (1,)

```python
list = (2,3,4,5,6,7,7)
print(type(list))

a = (1,)
print(type(a))

sample=("hi" , "this" , "is" , "me" , "readinf")
print(sample[0])

#both positive and negetive indexing work same as list

if "this" in sample :
  print("yes")
else :
  print("no")


#tuple_name(start :end : jump)
sample2 = ("hi" , "this" , "is" , "me" , "rading")
print(sample2[0:4:2])
```

### Tuple methods

```python
tuple1 = (0, 1, 2, 3, 2, 31, 1, 3, 2, 3)
print(len(tuple1))
print(tuple1.count(3))
print(tuple1.index(31))  #raises error if not found


#to add something to tuple you need to first convert it to list and then add the value and then convert it back to tuple

countries = ("Spain", "Italy", "India", "England", "Germany")
temp = list(countries)
temp.append("Nepal")
temp[0]="United States of America"
temp.pop(3)
modifiedCountries = tuple(temp)
print(modifiedCountries)

#concatenating two tuples to get a new tuples
countries1 = ("Pakistan", "Afghanistan", "Bangladesh")
countries2 = ("Vietnam", "India", "China")
southEastAsia = countries1 + countries2
print(southEastAsia)
```

#fstrings

```python
#fstrings are similar to template literals in javascript
letter = "Hey my name is {} and I am from {}"
name = "sachin"
country = "nepal"
print(letter.format(name , country))
print(letter.format(country , name ))


test = "hi what is you name {0} i am  {1}"
print(letter.format("alan","jo"))
print(letter.format("jo","alan"))

#the code becomes too long and boring using format method
#to solve this problem we have fstrig in python

val1="rainbow"
val2="pokhara"
print(f"hey i studied at {val1} academic homes located in {val2}")

#try to nulity f-strings using double {{}}
age=17
print(f"hi , i am {{age}} old ")

price=49.0023430
print(f"the fucking price is {price:.4f}")
#:.4f takes up to 4 decimal places

print(f"the product is { 4*2}")
```


# Docstrings and pep8

Python docstrings are the string literals that appear right after the definition of a function, method, class, or module.

### Python Comments vs docstrings
Comments are descriptions that help programmers better understand the intent and functionality of the program. They are completely ignored by the Python interpreter.

As mentioned above, Python docstrings are strings used right after the definition of a function, method, class, or module (like in Example 1). They are used to document our code.

Docstrings must be defines right above the function body 
We can access these docstrings using the doc attribute.

```python
def square(n) : 
  '''Takes in a number n , returns the square of n '''
  print(n**2)

square(5)
print(square.__doc__)
```

## PEP8  
PEP stand for Python Enhancement Proposal 
PEP 8 is a document that provides guidelines and best practices on how to write Python code. 
```python
import this 
print(this)
```

# Recursion in python
```python
def factorial(n) : 
    if(n == 0  or n ==1) : 
        return 1 
    else : 
        return (n*factorial(n-1))
    
print(factorial(5))

#recursion
def helper(n) : 
    if(n == 1 or n == 2 ) : 
        return 1 
    else : 
        return (helper(n-1) + helper(n-2))
    
for i in range(1 , 7) :
    print(helper(i)) 
```


# Sets 
Sets are unordered collecton of data items . They store multiple items in a single variable 
Sets are seperated by commas and enclosed in a curly bracket{}
Sets are unchangeable and cannot contain duplicate items 
- Sets cannot contain duplicate items 

```python
#ordered are just random and hence cannot be accessed by using index 
info ={
12 , 12 ,3
}
print(info)

data = {
    "sachin" , 
    12 , 
    True , 
    4.3
}
for i in data : 
    print(i)
```

```python
sets vs dictionary
ans = {} 
print(type(ans)) #this is an empty dictionary not set 

ans2 = set()
print(type(ans2)) #this is an empty set 
```


## Some sets methods 
```python
#We can perform operations like union , intersecition in sets just like in maths 

#union of sets 
cities = {"tokyo"  , "madrid" , "barlin"}
cities2 = {"tokyo" , "madrid" , "nepal"}
cities3 = cities.union(cities2)
print(cities3)

#update
s1 = {1,2,3,4,5}
s2 = {3,5,6,8,9}
s1.update(s2)
print(s1)

#intersection
cities = {"tokyo"  , "madrid" , "barlin"}
cities2 = {"tokyo" , "madrid" , "nepal"}
cities3 = cities.intersection(cities2)
print(cities2)

#intersection_update updates into existing set(s1) the common element of s1 and s2
a1={2,3,4,5,6,7}
a3={4,3,5,6,7,9,10}
a1.intersection_update(a3)
print(a1)

#symmetic_differecne return the symmetric difference of two sets 
set1 = {3,4,5,6,10}
set2 = {1,10,3,6,10}
set3 =set1.symmetric_difference(set2)
print(set3)

#symmetric_difference_update updates the existing set from another set 
b1 = {"berlin" , "kabul" , "nepal"}
b2 = {"berlin" , "india" , "nepal"}
b1.symmetric_difference_update(b2)
print(b1)

#difference returns the elements that are only present in the original set not in the another set 
age = {1,2,3,4,5}
age2 = {1,3,5}
diff = age.difference(age2)
print(diff)

#difference_update updates the set with the difference with another set 
age3 = {1,2,3,4,5}
age4 = {1,3,5}
age3.difference_update(age4)
print(age3)
print(age4)
```

Some other methos in sets 
```python
#check if item in a set 
info = {"carla" , 10 , False , 5.9}
if "carla" in info : 
    print("yes")

else : 
    print("no")

#isdisjoint() method return true is two sets are disjoint else False 
cities = {"Tokyo", "Madrid", "Berlin", "Delhi"}
cities2 = {"Tokyo", "Seoul", "Kabul", "Madrid"}
print(cities.isdisjoint(cities2))

#SImilarly there are methos like issubset() ans issuperset() to check subsest 

#remove method is used to remove the item form the list 
set = {
  "ram" , "shaym" , "ganshyam"
}
set.remove("ganshyam")
print(set)

#pop method removes the last element of set 
The last element might be random , unordered 


#clear method clears the set 
cities = {"Tokyo", "Madrid", "Berlin", "Delhi"}
cities.clear()
print(cities)


del keyword removes the entire set 
cities = {"Tokyo", "Madrid", "Berlin", "Delhi"}
del cities
print(cities) #cities is not defined 


#cities.add("added_item") to add item to city 

#remove()/discard()
We can use remove() and discard() methods to remove items form list.

Example :
cities = {"Tokyo", "Madrid", "Berlin", "Delhi"}
cities.remove("Tokyo")
print(cities)
Output:
{'Delhi', 'Berlin', 'Madrid'}

The main difference between remove and discard is that, if we try to delete an item which is not present in set, then remove() raises an error, whereas discard() does not raise any error.

```





# Python dictionaries 
Basics of dictionary 
```python
person = {
  "name" : "sachin" , 
  "age" : 20  , 
  "class" : "bachelor"
}

print(person)
print(person["name"])
print(person.get("name"))

#dictionary are ordered unlike sets 

#accesing all values of dictionary 
print(person.keys())
#accessing all values of dictionary 
print(person.values())
#accessing key values pairs 
print(person.items())

for i in person : 
  print(i) 
  print(person[i])


print("break")

sample = {
  1 : 'sachi' , 
  2 : 'ram' , 
  3 : 'shyam' , 
  4 : 'sita' ,
}

for key , values in sample.items() : 
  print(sample[key] == values)
```

### Dictionary methods 
```python
ep1 = {122: 45, 123: 89, 567: 69, 670: 69}
ep2 = {222: 67, 566: 90}

#The update() method updates the value of the key provided to it if the item already exists in the dictionary, else it creates a new key-value pair

ep1.update(ep2)
print(ep1)


#Creating an empty dictionary 
empt = {}



#clear method to clear whole dictionary
ep2.clear()
print(ep2)

#pop() method removes the key-value pair whose key is passed as a parameter

info = {'name':'Karan', 'age':19, 'eligible':True}
info.pop("age")
print(info)

info.popitem() #removes the last key-value pair
print(info)


#del keyword is used to delete the dictionary entirely
person = {
  "age" : 20 
}
del person 
print(person) #person is not defined 
```


# Loops 
```python
i = 0 
while i < 10 : 
  print(i)
  i = i +2 

else : 
  print("number exceeds 10")

print("break")

for  i  in range(0 ,5 ):
  print(i)

else : 
  print("hello mother fucker ")



print("break")
for x in range (5):
  print(f"iteration no {x} in for loop ")

else : 
  print("out of loop ")


#else execution means loop is executed and finishes not breaked 
#if loop is breaked else is also breaked 
```

# try except error in python 
```python
try :  
    a = 10
    b = "sachin" + a 
except : 
  print("what is this ")
```

# Finnary clause in python 
The finally code block is also a part of exception handling. When we handle exception using the try and except block, we can include a finally block at the end. The finally block is always executed, so it is generally used for doing the concluding tasks like closing file resources or closing database connection or may be ending the program execution with a delightful message.

```python
def testingFinally : 
    try : 
      l = [1,2,3,4,5,6]
      i = int(input("Enter the index: "))
      return 0 

    except:
      print("Some error occured")
      return 1 
    finally : 
      print("i am alwats ececuted")

testingFinally()
```


# Raising custom erros 
To raise a custom error we can use raise keyword 
```python
a = int(input("Enter the number"))

try : 
    if (a == 10 ) : 
             raise ValueError ("value should not be 10")
except  : 
    print("ther is a value error ")
```


# Short hande if Else 
```python
a = 1000 ; 
b = 10 
print("A") if a < b else print("=") if a ==b else print("B")

result  = 10 if 5%2 == 1 else 20 
print(result )
```

# Enumerate function in Python while looping 
```python
marks = [12, 56, 32, 98, 12,  45, 1, 4]

# index = 0 
# for mark in marks : 
#   print(mark) 
#   if(index == 3) : 
#     print("Awesome")
#     break ; 
#   index = index + 1 ; 

#To solve this problem of initializing index , increasing it 
# we use enumerate function

for index, mark in enumerate(marks) : 
  print(index)
  print(marks[index])

print("Break")

#we can also definee the starting index by defining start = 
for index , mark in enumerate(marks , start = 4) :
  print(marks[index])
```



# Virtual environment in Python 
A virtual environment is a tool used to isolate specific Python environments on a single machine, allowing you to work on multiple projects with different dependencies and packages without conflicts. This can be especially useful when working on projects that have conflicting package versions or packages that are not compatible with each other.

Virtual enivironment helps you to manage dependencies , version by allowing each project have its own python 


Creating a virtaul enivronment 
- Select a directory to create a virtaul environment 
- To create use command $ python -m venv env
- This will create a new directly ./env


# Using keywords Arguments
The order of arguments doesnot matter unlike positional arguments  
```python

def hello(first  ,middle , last) : 
    print("Hello", first, middle, last, "!")

hello(last="Smith", first="John", middle="Q.")
```

# Nested function calls in python 
```python
num = round(abs(float(input("Enter a whole number positive"))))
print("The number is", num)
```



