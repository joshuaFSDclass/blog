# Debugging 
<h2 style= "color:red, blod">
  This blog is all about debugging 
</h2>

 Hello this blog is to show some debugging exersises that i have done to sharppen my skill (feel free to try them youslef ).
  
# Debugging task 1 

  ~ This specific task has to do with if statements.
  
  ~ The most common msitekes that are apparent when debugging is sytax error. 
<h3>
  The first segment of code 
</h3>

<h4>
  The purpose of the code was to determine wheather the temperature was hot or cold. 
</h4>

```python
  temperature = 75
  
  if temperature > 80:
      print("It's hot")
  elif temperature > 50 :
      print("It's temperate")
  elif temperature < 0:
      print("It's cold")
```
~ ERROR:

The main issue with this code is that the perameters for beign hot and cold aren't propperly defined 
the probem with the code is that the code does not account for number between 0 and 50 
 
						(if we had changed the elif above it we would also have to change the elif to just change)


<h4>
  The correct thing to do for this code segment:
</h4>



```python
temperature = 75

if temperature > 80:
  print("It's hot")
if temperature > 50 and temperature < 80:
  print("It's temperate")
if temperature < 0:
  print("It's cold")
```

	> This code difines the perameters of moderate.

Of the number of challenges liined up in this blog this one was on of the easiest ones, on to more difficult challenges.

# Debugging task 2 

  ~ This specific task has to do with for loops.
  
  ~ Common errors that are found when writting loop is using the correct datatype when calling functions . 
<h3>
  The first segment of code 
</h3>


```python

text = "Hello, world, my name is"
count = 0

for char in text:
    if char == "":
       count += 1

print(count)

```
