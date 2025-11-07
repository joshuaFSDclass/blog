# Debugging 
<h2>
  This blog is all about debugging 
</h2>

 Hello this blog is to show some debugging exersises that i have done to sharppen my skill (feel free to try to debug them your self them youslef ).
 
 <img src="/blog/images/ducky.jpg" alt="debugging partner rubber ducky">
 
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



<details>
<summary>
<h2>
	Try it your self or click to see the answer
</h2>
</summary>

	> if we had changed the elif above it we would also have to change the elif to just change
	
<h4>
  The correct thing to do for this code segment:
</h4>

<div markdown="1">

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
</div>
</details>

# Debugging task 2 

  ~ This specific task has to do with for loops.
  
  ~ Common errors that are found when writting loop is using the correct datatype when calling functions . 
<h3>
  The second segment of code 
</h3>

<h4>
	The purpose of the code here is to count the amount of spaces are in a given string
</h4>


```python

text = "Hello, world, my name is"
count = 0

for char in text:
    if char == "":
       count += 1

print(count)

```

~ ERROR:


The issue with this code is that the if statment is meant to check for a space but the quotes have nothing in them so the 
code is actually checking for empty an empty value.





<details>
<summary>
<h2>
	Try it your self or click to see the answer
</h2>
</summary>
<h4>
	The correct veirsion of the code:
</h4>

```python
text = "Hello, world, my name is"
count = 0

for char in text:
    if char == " ":
       count += 1

print(count)
```
	> The code includes the space between the parenthesese

Some of these issues are very hard to notice at first glance me personaly I bearly notied the fact that parentheses are empty.
</details>


# Debugging task 3 

  ~ This specific task has to do with for loops as well.
  
  ~ Common error found is that programmers would use the wrong opperator for some small section of their code. 
<h3>
  The second segment of code 
</h3>

<h4>
	The purpose of the code here is to determinee weather the number enterd by the user is even or odd.
</h4>

```python

print("give me a number")
n = input()

for num in range(1, n):
    if num % 2 < 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")

```

~ ERROR:


The issue with this segment of code is that odd numbers are being shown as even when they aren't.



<details>
<summary>
<h2>
	Try it your self or click to see the answer
</h2>
</summary>
<h4>
	The correct veirsion of the code:
</h4>

```python
print("give me a number")
n = int(input())

for num in range(1, n):
    if num % 2 == 0:
        print(num, "is even.")
    else:
        print(num, "is odd.")
```
	> This corrected versionhas the apropraeate opperator in place.

The solution for this code was easy but often it's hard for biginners to find the mistake deending on the their level of expererience.
The greater than symbal was to be replaced by the doulbe equal sign to compare the result of the oppereation to zero to determine if the number is odd.
</details>

# Debugging task 4 

  ~ This specific task has to do with if statements.
  
  ~ The most common msitekes that are apparent when debugging is sytax error. 
<h3>
  The fourth segment of code 
</h3>

<h4>
  The purpose of the code was to calculate the factrial of any given nunber. 
</h4>

```python
  num = int(input("Enter an integer: "))

if num < -1:
  print("No negative numbers.")
else:
  result = 1
  for i in range(1, num):
    result *= i   

  print("Factorial of " + num + "is" + result)
```
~ ERROR:

The error with this code is that concatination doesn't happen with integers, essentialy a type error.


<h2>
	Try it your self or click to see the answer
</h2>

	> if we had changed the elif above it we would also have to change the elif to just change


<h4>
  The correct thing to do for this code segment:
</h4>



```python
num = int(input("Enter an integer: "))

if num < -1:
  print("No negative numbers.")
else:
  result = 1
  for i in range(1, num + 1):
    result *= i   

  print("Factorial of " + str(num) + "is" + str(result))

attempts = 0
correct_password = "secret"
```

	> This code difines the perameters of moderate.

Of the number of challenges liined up in this blog this one was on of the easiest ones, on to more difficult challenges.
