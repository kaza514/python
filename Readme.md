# Python Basics
## Create Input String and Print
  ```sh
 ch=input("ente a char : ")
 print(ch)
 ```

## String Validation in Python
  ```sh
 name = input( "please enter the name")
 print(name)
 name1 = 'you got a nice name' if name == 'kaju' or name == 'khaja mohiddin' or name == 'kaza' else 'you have cool name'
 print(name1)
 ```

##  Diff Between Local and Global Variable in Python
  ```sh
total = 25; # This is global variable.
# Function definition is here
def sum( arg1, arg2 ):
    # Add both the parameters and return them."
    total = arg1 + arg2; # Here total is local variable.
    print("Inside the function local total : ", total)
    return total;
# Now you can call sum function
sum( 10, 20 );
print("Outside the function global total : ", total)
def func():
    global x;
    print(" local value is",x)
    x=2
    print("changed local varialble",x)
x=50
func()
print(" the value of x still is ",x)
 ```



## Creating if and else if statement in Python
  ```sh
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
  ```sh
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
  ```sh
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

## Nested While
  ```sh
 i = 2
 while(i < 100):
     j = 2
     while(j <= (i/j)):
         if not(i%j): 
             break
         j = j + 1
         if (j > i/j) : 
             print(i, " is prime")
     i = i + 1
 print("Good bye!")
 ```

## For loop in Python 
  ```sh
 for letter in 'Python': # First Example
     print('Current Letter :', letter)
 fruits = ['banana', 'apple', 'mango']
 for fruit in fruits: # Second Example
     print('Current fruit :', fruit)
 print("Good bye!")
 ```


## Continue

### First Example
  ```sh
 for letter in 'Python':   
     if letter == 'h':
         continue
     print('Current Letter :', letter)
 ```
### Second Example
  ```sh
 var = 10  
 while var > 0:
     var = var -1
     if var == 5:
         continue
     print('Current variable value :', var)
 print("Good bye!")
 ```



## Python Operators
  ```sh
 import math
 def operation_result(op,var1,var2):
     if op==1:
         sum=var1+var2
         print("Addition of %d and %d is %d"%(var1,var2,sum))
     elif op==2:
         sum=var1-var2
         print("Substraction of %d and %d is %d"%(var1,var2,sum))
     elif op==3:
         sum=var1/var2
         print("division of %d and %d is %d"%(var1,var2,sum))
     elif op==4:
         sum=var1*var2
         print("multiplication of %d and %d is %d"%(var1,var2,sum))
     elif op==5:
         sum=var1%var2
         print("modulus of %d and %d is %d"%(var1,var2,sum))
     else:
         print("please enter a valid operator")
     
 def operation_geometry(op,var1):
     
     if op==6:
         val=math.sin(var1)
         print("the sin of %d is %f"%(var1,val))
     elif op==7:
         val=math.cos(var1)
         print("the cos of %d is %f"%(var1,val))
 
     elif op==8:
         val=math.tan(var1)
         print("the tan of %d is %f"%(var1,val))
 
     else:
         print("please enter a valid oprator")
 
 while True:
     print("-----------1. addition -----------")
     print("-----------2. subtraction -----------")
     print("-----------3. division -----------")
     print("-----------4. multiplication -----------")
     print("-----------5. modulus -----------")
     print("-----------6. sin value -----------")
     print("-----------7. cos value -----------")
     print("-----------8. tan value -----------")
     op=int(input("enter your choice : "))
    
     if (op==1 or op==2 or op==3 or op==4 or op==5):
         var1=int(input("enter first value"))
         var2=int(input("enter second value "))
         operation_result(op,var1,var2);
     elif(op==6 or op==7 or op==8):
         var1=int(input("enter a value"))
         operation_geometry(op,var1)
     else:
         print("Please enter proper value from the menu")
     print("do you want to continue again [y/n]")
     c=input("enter y to continue n to exit  : ")
     if c=='n' or c== 'N':
         break
     
 print("thanks for using this application , visit again")
     
  ```   




## Function and lamdba function

  ```sh

sum = lambda arg1, arg2: arg1 + arg2;

def sum1(arg3,arg4):
    return arg3+arg4
 

# Now you can call sum as a function
print("Value of total : ", sum( 10, 20 ))
print("Value of total : ", sum( 20, 20 ))

print("value of total is : ",sum1(45,45)) 

  ```
