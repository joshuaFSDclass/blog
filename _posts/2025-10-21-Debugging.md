# Debugging 
<h2 style= "color:red, blod">
  This blog is all about debugging 
</h2>

 hello this blog is to show some debugging exersises that i have done to sharppen my skill (feel free to try them youslef ).
  
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
  elif temperature > 50:
      print("It's temperate")
  elif temperature < 0:
      print("It's cold")
```
~ ERROR:
The main issue with this code is that the perameters for beign hot and cold aren't propperly defined 
the probem with the code is that the code does not account for number between 0 and 50 
