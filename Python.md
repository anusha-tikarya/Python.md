###  Printing Strings and Numbers
```python
# Printing Strings and Numbers
print("hello World , I'm Anusha")
print("I am 21")
print(21)
print(21 + 22)
```
### input
name1,name2 = input(f'What is first guy\'s name? '),input(f'What is second guy\'s name? ') # f' string use to print #/ is use to use(')
height1,height2 = int(input(f'What is {name1}\'s height?  ')),int(input(f'what is {name2}\'s height? ')) # {} --> these are use to variable directly without using"+""
if height1 > height2:
  print(f'{name1} is taller than {name2}')
else:
  print(f'{name2} is taller than {name1}')
  
### Variables and Data Types
```python
# Variables and Data Types
name = "shradha"
age = 12
score = 90.9
age2 = age + 3
print("My name is:", name)
print(name, "is", age2, "years old")
print(type(name))
print(type(age2))
print(type(score))
```
### Booleans and None
```python
# Booleans and None
old = True
a = None
print(type(old))
print(type(a))
```
###  Function to Sum Two Numbers
```python
# Function to Sum Two Numbers
def sum(a, b):
    sum = a + b
    return sum

print(sum(1, 2))
```
### String Operations \n , \t
```python
# String Operations
str = "I am happy \n I am healthy \t I am wealthy"    # \n for new line and \t for tab
print(""" allow multiple line
support """)## just paste same as you have as it supports multiple lines
print(str)
```
### Concatenation
```python
# Concatenation
a = "hello"
b = "Indore"
print(a + " " + b)
print(len(a))  # len used for length
ch = a[2]  # Access value of a at the index of 2, similar we cannot assign the value
print(ch)
```
###  Slicing

```python
# Slicing
str = "apple is red"
print(str[1:])
print(str[:6])
print(str[-5:-1])
print(str[:-3])
```
### endswith , capitalize , replace , find , count
```python
str = "apple is red"
print(str.endswith("app"))  # endswith function tells if a function ends with a particular string or not
print(str.capitalize())  # capitalize makes the first letter of the string capital.
print(str.replace("apple", "cherry"))
print(str.find("c"))  # -1 as it doesn't exist
print(str.find("apple"))  # name starts at index _
print(str.count("e"))  # count no. of occurrence of a particular string
```
## Conditional Statement:
```python
if (condition):
elif(condition):
else:
```
## Nesting 
```python
if (condition): 
    if (condition):
    else:
else:
```
## List
```python
marks = [40,20,30,40,"KUMU"]
print(marks[1])#20
marks[1]=45
print(marks[1])#45
```
## List slicing 
```python
# strating_index : ending_index

a=[ 1,2,"abhi","sabhi"]
print(a[2:3])
```
## LIST METHODS:

### list.append
```python
b=[1,2,3,4,5]
b.append(4)
print(b)
```
### list.sort
```python
b=[1,2,3,4,5]
print(b.sort())#None , as it just change 
print(b) #[1, 2, 3, 4, 5] , as sorting is done before
print(b.sort(reverse=True))# now list will print in desc. order
print(b)#[5, 4, 3, 2, 1]
```
### list.reverse
```python
b=[1,2,3,4,5]
b.reverse # this will reverse the final or true list
print(b)
```
### list.insert(index , element)
```python
b=[1,2,3,4,5]
b.insert(0,4)
print(b) #[4,5, 4, 3, 2, 1]
```
### list.remove(element)
```python
b=[1,2,3,4,5]
print(b.remove(1))#None
print(b)#[2, 3, 4, 5]
```
### list.pop(index)
```python
b=[1,2,3,4]
b.pop(1)
print(b)#[1, 3, 4]
```


### TUPLES 

```python
tup=(1,2,3,4,5,6)
print(tup[1])  # Output: 2
print(type(tup))  # Output: <class 'tuple'>
print(tup.count(2))  # Output: 1
tup=(1,2,3,4,5,6)
print(tup.index(3))  # Output: 2
```
### Shallow copy 
The `copy()` method is not available for tuples in Python because tuples are immutable, meaning their elements cannot be modified after creation. However, you can create a shallow copy of a tuple using slicing or the `tuple()` constructor. Here's how you can do it:

```python
# Original tuple
original_tuple = (1, 2, 3)

# Shallow copy using slicing
shallow_copy = original_tuple[:]

# Shallow copy using tuple() constructor
shallow_copy = tuple(original_tuple)

print(shallow_copy)
```

Both methods create a new tuple with the same elements as the original tuple, effectively producing a shallow copy. Remember that if the tuple contains mutable objects (like lists), changes made to those objects will be reflected in both the original and copied tuples because they share references to the same objects.

