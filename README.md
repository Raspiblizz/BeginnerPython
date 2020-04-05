# BeginnerPython
Beginner Python 

# script from Udemy 
print(6*7)
# adding and subtracting etcetera

print("hello world")
# but also 
print(hello world) 
# don't need parentheses 
# tabs and spaces + functions + strings 
# below is a string 
greeting = "Hello"
name= input("Please enter name") 
print(greeting + '' + name) 
# the result is example "Hello Tim" , and the space is ''

# printing tabs 
# tabbedstring= 'Hello\tThe T stands for tabs in between\tAKA spaces in between'
# Splitstring = 'Hello\And N stands for a split to another line\n'
print(Splitstring + tabbedstring) 
Triplequotes= ("""tripe quotes are my best friend, they basically print as is, 
the problem is if you don't want it to run to the next line but you have no more space, but you can solve this by adding a backslash that basically cancels out the spaces like this \
see how it cancels \ """)
print(Triplequotes)
# what if backslash is included in ur text - example below
print("C:Users\tim\newstuff")
# just add a second one (this method is recommended vs other method below)
print("C:Users\\tim\\newstuff")
# or you create a raw string by adding an r 
print(r"C:Users\\tim\\newstuff")
# Python variables can only begin with a letter or _ , can't begin with number
# Classes --> strings example "computers, steve jobs, Microsoft" int examples "1,2,3" ps. u can rebound the label to a new variable
print(type(variableurlookingtodefine))
# don't forget about typeerror -- where concatonating int with string classes doesn't work 
# Python has several built- in data types (numeric, iterator, sequence(also iterator), mapping file, class, exception) 
# Numeric data types ( int (whole numbers), float(decimal point numbers) , complex(imaginary numbers)) 
print(a + b) #15
print(a - b) #9
print (a * b) #36
print(a / b) # 4.0
print(a // b) #4 integer division, rounded down towards minus infinity 
print(a % b) # 0 modulo: the remainder after integer division - so what remains - after diving 
# Operator precedence (order- example: bedmas) 
# usual for programming languages to start counting at 0 and not 1 
parrot = "Norwegian Blue"
print(parrot) 
print(parrot[3])
# number inside brackets are called index, used to index into the string -four uses of square brackets in python, all used to access individual items in something  - you gotta count 0 first 
# you can print the last number by going backwards --> you can print "e" as -1
# dont count zero as negative zero go straight to 1 
# slicing 
print(parrot[-1])
print(parrot[0:6]) 
# answer - Norweg 
print(parrot[:9])
# leaving it blank makes the default here "0" 
# this tells python run the range of numbers no including the last number-very important "final value" "up to but not including" 
print(parrot[10:14]) 
print(parrot[10:])
# 14 is the stop value -
print(parrot[6] + parrot[6:1])
print(parrot[-4:-2]
print(parrot[-4:12]
# can't go back print(parrot[-14:8])
# using a step in a slice 
print(parrot[0:6:3]) #Nre
print(parrot[0:6:3] #NW
# this is because it it takes the range 0:6 and then steps through the sequence in steps of 2 - kinda tricky at first but very simple- just takes every two letters from ranges 0:6
number = "9,223,372,036,854,775,807"
print(number[1::4]) #,,,,,, this prints every fourth character starting from 1 
seperators = number[1::4]
print(seperators) 
values = "".join(char if char not in seperators else " " for char in number).split()
print([int(val) for val in values]) 

letters = "abcdefghijklmnopqrstuvwxyz"
backwards = letters[25::-1)
print(bacwards)
backwards = letters[::-1) #python idiom 
# makesure start value is greater than stop value
# last value not printed 
#random note: spaces count! ex- in 5 in ---> 3:1:5 
print(16:13:-1) #qpo
print(4::-1) #edcba
print(:-9:-1) #last 8 characters in reverse order

Idioms 
# returning last 4 letters of sequence
print(letters[-4:] #wxyz
print(letters[-1:]) #the last item "z"
print(letters[:1])  (because 1 is end value - so you get 0-1 ) 
print(letters[0]) ---problem with this version is that it won't show an output if the sequence is removed , causing it to crash - but the :1 allows it to keep running through a lackless sequence -- even if it is an error technically 

#Python sequence(sequence is a data type) 
The string type
list 
tuple
range
bytes and bytearray 
computer_parts= ["x", "monitor," "y"]
computer_parts[1][0] --> first part of sequence # 1 "m"

string1= "he's"
string2= "probably"
string3= "pining"
string4= "for the"
string5= "fjords"

print(string1 + string2 + string3 + string4 + string5) # plus is not necessary when concatinating in python 
print("he's" "probably" "pining" "for the " "fjords")
print("hello"* 5) # start repeats sequence #hello hello hello hello hello
print("Hello"* (5 + 4)) #prints nine times 
print("hello" 5 * "4") #hello hello hello hello hello 4 

# are you a part of a string?
today = "friday"
print("day" in today) # True 
print("fri" in today) # True 
print("thur" in today) # False 
# replacement fields
# making int into strings - using string function str 
age = 24 
print("My age is" + str(age) + "years")
#replacement fields and dot format method
print("My age is {0} years".format(age))
print("There are {0} days in {1}, {2}, {3} and {7}"
.format(31,"Jan","Mar", "May", "Dec")) 

print("Jan: {2}, Feb: {0}, Mar: {2}, Apri: {1}, May: {2}
  .format(28,30,31)) 
  
print()
print("""Jan: {2}
Feb: {0}
Mar: {2}
Apr: {1}
May: {2}
  """.format(28,30,31))
  
#String formatting 
for i in range (1, 13): 
print("No. {0} squared is {1} and cubed is {2}" .format(i,i ** 2, i ** 3)
#example of output: 
No. 1 squared is 1 and cubed is 1
No. 2 squared is 4 and cubed is 8 
No. 3 squared is 9 and cubed is 27 
 
#add width ---> with colon - example if you add {0:2} it thinks of reserving two spaces o the screen 
print("No. {0:1} squared is {1:4} and cubed is {2:4}" .format(i,i ** 2, i ** 3))
#left align add less thank values 
print("No. {0:1} squared is {1:<4} and cubed is {2:<4}" .format(i,i ** 2, i ** 3))
# center is ^ such as {2:^4)
# precision - decimal point -
# floating point numbers - precision after the decimal point following the width 
print("pi is aprox {0:12}" .format(22/7))
print("pi is aprox {0:12.50f}" .format(22/7)) default is 6 digits
print("pi is aprox {0:12.54f}" .format(22/7))
print("pi is aprox {0:12f}" .format(22/7))

# python ignores width over decimal point, it considers decimal point more important which is why above - the results are interesting lol 

# f-strings
age = 24 
print(name + "is" + age + " years old") 
# the line above will display error due to int mixed with strings 
print(name + f" is {age} years old") 
print(type(age)) #<class 'int'>
print (f"Pi is approximately {22/7:12.50f}")
print(f"Pi is approx {pi:12.50f}

# string interpolation :
print("my age is %d, %s, %d, %s" % (age major, 6 minor) 
print("PI is approximately %60.50f" % (22/7))
print("PI is approximately %60.50f" % (22/7))
