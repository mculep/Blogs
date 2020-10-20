## DAY 6 OF PROGRAMMING - 10/19/2020

## Python
---

### Things we worked on:
---
- List
1. What are the parts of a list?
2. Creating lists
3. Accessing items from a list

---
- Iterate though Lists
1. Loop through list with while
2. Loop using for

---
- Modifying Lists
1. Appending values
2. Concatenating lists
3. Extending lists
4. Assign value by index
5. Deleting by index
---

- Lists in Lists
1. Accessing nested lists
2. Looping through nested lists

## 1. **Lists**

### Usually is an array. But Python is list

## What are the parts of a list?
```
  [1,2,3] #List of intergers
  ["hi", "my", "name", "is", "Clint"] #List of strings
  [1,"stringy", False] # List of mixed types

```
## Creating lists
```
  # creating a list and assigning it to a variable
  some_numbers = [1,2,3]
  my_children = ["Olivia", "Alle", "Mark"]

  name = "Clint"
  age = 38
  married = True
  my_info = [name, age, married] 
  #Putting the variables in the array

```
## Accessing items from a list
```
  my_children = ["Olivia", "Alle", "Mark"]
  print(my_children[0]) #Olivia
  print(my_children[2]) #Mark
  print(my_children[1]) #Alle
```  

## 2. **Iterate through lists**

## Loop through list with while

```
my_children = ["Olivia", "Alle", "Mark"]
index = 0
#When using a list len() counts the number of items
while index < len(my_children):
print(index+1,my_children[index])
index += 1
```      
##
```
my_children = ["Olivia", "Alle", "Mark"]
#child is the value of the current item in the iteration
for child in my_children:
print(child)
```      

WHILE LOOP
```
my_children = ["Olivia", "Alle", "Mark"]
 
while i < len(my_children):
    print(i+1, my_children[i])
    i += 1
```    
---

FOR LOOP
```
 things = ["lamp", "imac", "keyboard", "iphone"]


 for i in range(len(things)):
    print(i, things[i])
```
---

1. ## **Modifying Lists **

```
Example:

my_pets = ["Daisy", "Molly", "Shadow"]
my_pets.append("Rainbow") #using append method
print(my_pets) #You can simply print an array
```

## Appending Values
```

######
"ONLY CAN ADD ONE TO THE LIST"

my_pets = ["Daisy", "Molly", "Shadow"]
my_pets.append("Rainbow") #using append method
print(my_pets) #You can simply print an array
```
## Concatenating Lists

```
my_dogs = ["Daisy", "Molly"]
my_cats = ["Shadow", "Rainbow"]
my_pets = my_dogs + my_cats
print(my_pets) #combines both
print(my_dogs) #doesn't change the original list

Example

my_dogs = ["Daisy". "Molly"]
my_cats = ["Shadow", "Rainbow"]

my_pets = dogs + cats
my_pets + my_pets + ["George"] 

####
Combined _literal = [1,3,4] + ["A", "b", True]
print (combined_literal) 
###

```
## Extending Lists
```
my_pets = [] #empty list
my_dogs = ["Daisy", "Molly"]
my_cats = ["Shadow", "Rainbow"]
my_pets.extend(my_dogs) 
#extend method modifies the array
print(my_pets)
my_pets.extend(my_cats)
print(my_pets)
```
## Assign Value by index
```
my_pets = ["Daisy", "Molly", "Shader", "Rainbow"]
my_pets[2] = "Shadow"
print(my_pets)#now its Shadow at index 2
```
## Deleting Value by index

```
my_pets = ["Daisy", "Molly", "Shadow", "Rainbow"]
del my_pets[3]
print(my_pets)#now rainbow is gone

```
1. **Lists in Lists**

### Nested list
---
```
 people = [
      ["Clint","Fleetwood", 38], 
      ["Anna", "Fleetwood", 37]
  ]
  print(people[0]) #["Clint","Fleetwood", 38]
  print(people[0][0]) #Clint

  #assigning result of expression to variable
  age = print(people[1][2]) #37

  #You can modify the array in place the same way
  people[0][2] = 39 
  del people[1][2]
  print(people)

  ```
### Loops through nested lists
---
```
people = [
      ["Clint","Fleetwood", 38], 
      ["Anna", "Fleetwood", 37],
      ["Peter", "Hollens", 34],
      ["Lindsey", "Sterling", 35]
  ]

  for person in people:
      print("First, Last, Age")
      for attribute in person:
          print(attribute)

----------------

  coordinates = [[10,10], [20,10],[10,20]]

  for cord in coordinates:
      idx = 0
      print("Position:")
      for position in cord:
          p = "X"
          if idx == 1:
              p = "Y"
          print(f"{p}-{position}")
          idx += 1

```
----

## DAY 7 OF PROGRAMMING 10/20/20

## Python
---

### Things we worked on:

---






## DAY 8 OF PROGRAMMING 10/21/20

## Python
---

### Things we worked on:

---






## DAY 9 OF PROGRAMMING 10/22/20

## Python
---

### Things we worked on:


---






## DAY 10 OF PROGRAMMING 10/23/20

## Python
---

### Things we worked on: