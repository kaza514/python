## Create Input String and Print
```
ch=input("ente a char : ")
print(ch)
```

## String Validation in Python
```
name = input( "please enter the name")
print(name)
name1 = 'you got a nice name' if name == 'kaju' or name == 'khaja mohiddin' or name == 'kaza' else 'you have cool name'
print(name1)
```

## Creating if and else if statement in Python
```
var = 100
if var == 200:
    print("1 - Got a true expression value")
    print(var)
elif var == 150:
    print("2 - Got a true expression value")
    print(var)
elif var == 100:
    print("3 - Got a true expression value")
    print(var)
else:
    print("4 - Got a false expression value")
    print(var)
print("Good bye!")
```

## Nested If
```
var = 100
if var < 200:
    print("Expression value is less than 200")
    if var == 150:
        print("Which is 150")
    elif var == 100:
        print("Which is 100")
    elif var == 50:
        print("Which is 50")
elif var < 50:
    print("Expression value is less than 50")
else:
    print("Could not find true expression")
print("Good bye!")
```

## While loop using if Condition
```
var = 1
num=1;
while num: # This constructs an infinite loop
    num = input("Enter a number :")
    num=int(num)
    if num == 200:
        break
    print("You entered: ", num)
    
print("Good bye!")
```

## For loop in Python 
```
for letter in 'Python': # First Example
    print('Current Letter :', letter)
fruits = ['banana', 'apple', 'mango']
for fruit in fruits: # Second Example
    print('Current fruit :', fruit)
print("Good bye!")
```





