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

1. Key Value Pairs
2. Functions
3. Functions with arguements/parameters
4. Function return value
5. Function Scope

---

---
Other types of functions that we use a lot!:
- print()
- input()
- type ()
- float ()
- int()
- len()
---

1. **Key Values**
---
**** keys can have lists ******
**** Use strings in keys ******

 ***************
```
movie = {
  "name":"Star Wars",
  "episode":4,
  "year":1977,
  "villains":["Vader", "Tarkin"],
  "heros":["Luke","Leia", "Han", "Obi-Won"]
   [KEY] [VALUE]
}


print(movie)
print(movie["year"])
print(movie["villains"])


bad_guys = movie["villains"]
or 
- use a set function
bad_guys = list(set(movie["villains"]))

print(bad_guys)
print(bad_guys[1])
bad_guys.append("Jabba")

you can add list by doing the following:

movie["ships"] = ["Falcon", "Star Destroyer", "Death Star"]
print([movie])

movie["heros"].append("Chewbacca")


**
 #print from dictionary
  print(move["name"]) 

  #assign to variable
  episode_num = movie["episode"]
  
  

   #accessing a value from an array in the dictionary
  print(movie["heros"][1]) #Leia

  # the key can be a variable
  search = "villans"
  print(movie[search])

  **
  Call out the keys and values in a for loop

  for key in movie:
    print(key, movies[key])

```

---

---
```
*** Make sure to indent print or anything
else that is within the function and when calling
it def needs to be lined up with def. 
                      ***************

def my_func():
    print('I am function. Hear me roar!')

def add_numbers():
    number_1 = 10
    number_2 = 20
    number_3 = number_1 + number_2
    print(number_3)

my_func()
add_numbers()





  # can call over and over again if you want
  my_func()
  my_func()
  my_func()

  add_numbers()

```

3. 
**Functions using parameters and arguments**
---
print("this is the argument", "hello")
len([1,2,3])

you can add multiple arguments in a function
by seperating them by commas.

```
```
def add_two_num(a,b): <------ these are parameters/treated like a variable inside the function
    print(a+b)
    
add_two_num(1,2) <---supplying the arguements
add_two_num(7,5)


IT HAS TO BE THE SAME DATA TYPE
add_two_num (1, "c")<----- since a + b (it can't be a str and a int)

```
def stuff(first, age):
  print(f"Hello {first} you are {age} year old")

stuff("Samson", "12")  <---- Has to be in order

```
```
it can be anything: string, number, list

def any_print(any):
    print(any)

any_print(2)
any_print(True)
any_print([3,4,5])
any_print("Hello")
```
**Function Return Value**

```
def movie(movie_item):
    Title = movie_item[0]
    Genre = movie_item[1]
    Year = movie_item[2]

    print(f"1. Title: {Title}")
    print(f"2. Genre: {Genre}")
    print(f"3. Year: {Year}")

movie("Star Wars - A new hope", "Sci-Fi", "1977")    

### Another way of doing it is:

def movie(movie_item):
  idx = 1
  for item in movie_item
    print(f"{idx}, {tem} : {movie_item[item]}")
    idx += 1 
 movie({"Genre"} " "Horror", "Title": "I am at beach", "year" : 2020)
```

**Function Scope**


## DAY 8 OF PROGRAMMING 10/21/20
---
### Things we worked on:

1. Classes
2. Class Methods
3. Class Inheritance
---



1. **Classes**

```
class person:
  def __init__(self, name, age):
    print(self)
    print("You created a new instance of a person")
    self.name = "samson"
    self.age = 12

samson = person()
fuzzy = person()

print(samson.age)
print(fuzzy.name)



print(samson)

```

2. **Classes Methods**

```
class mob:
  def __init__ (self, name, health = 10)
    self.name = name
    self.health = health

  def get_hit(self,power):
    self.health = self.health - power
    print(f"I {self.name} was hit for {power} points")


hero = mob("sir barksalot")
print(hero.health)
hero.get_hit(6)
print(hero.health)



```

3. **Classes Inheritance**

```
  # Previous class lesson without print text
  class Mob:
      def __init__(self, name, health = 10, attack_power = 2):
          self.name = name
          self.health = health
          self.attack_power = attack_power 

      def get_hit(self, power):
          self.health = self.health - power            

      def attack(self, enemy):           
          enemy.get_hit(self.attack_power)
  
  #not very useful but valid
  class Hero(Mob):#Hero class is a sublclass of Mob
      pass
  
  hero = Hero("Sir Galahand")
  print(hero.name)

```
## Overiding class methods

  class Hero(Mob):
      #overriding __init__
      def __init__(self):
          #Can repeate for every item
          self.name = "Sir Galahand"
          self.health = 22
          self.attack_power = 3
          self.defence = 1

      #overriding get_hit
      def get_hit(self, power):
          self.health = self.health - (power-self.defence)
      
      ...#yell method
  
  hero = Hero()#all arguments default
  bad_guy = Mob('Evil McEvil', 10)
  print(hero.name)#added automatically 
  bad_guy.attack(hero)
  print(hero.health)#health only went down by one because of defence

 ---
## DAY 9 OF PROGRAMMING 10/22/20

## Python
---

### Things we worked on:
---
 Worked on Python game project, talked about Agile developments.


Menu for user input




## DAY 10 OF PROGRAMMING 10/23/20

## Python
---

### Things we worked on: