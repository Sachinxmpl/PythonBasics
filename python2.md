# Variable scoping in python 
Variables declared within a function have a local scope
Python follows LGED rule of least privilege


# *args parameter in python 
parameter that will pack all arguments into a tuple useful so that a function can accept a varying amount of arguments 


```python
def add(*numbers) : 
    print(type(numbers)) #tuple and hence immutable 
    sum = 0 
    for i in numbers : 
        sum += i
    return sum 
print(add(1,2,3,4,4,5,6,7,5))
```


# **kwargs in python 
Parameter that will pack all arguments into a dictionary 
useful so that a function can accept a varyginh amount of keyword arguments 

```python
def hello(**details) : 
    print(type(details)) #dictionary 
    for key , value in details.items() :
        print(key, value)

hello(first="sachin" , middle="kumar", last="kumar")
```

# Format method in python 
```python

```