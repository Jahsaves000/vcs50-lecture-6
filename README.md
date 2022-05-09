# vcs50-lecture-6
cs50 lecture 6 notes
// rewatch first 25 mins

//picking up at 25 mins into lecture
// in order to repetively repeat hello world using a for loop in python
for i in range(50):
    print("hello, world")
//how to import entire library
    import cs50
    
// how to import specific functions
    from cs50 import get_string, get_float, ect.

//blurring an image
from PIL inport Image, ImagFilter

before = Image.open("bridge.bmp")
after = before.filter(ImageFilter.BoxBlur(10))
after.save("out.bmp")

//dictionary.py

words = set()

def check(word):
    if word.lower in words:
        return True
    else:
        return False


def load(dictionary):
    file = open(dictionary, "r")
    for line in file:
        words.add(line.rstrip())
    file.close(file)
    return True
    
    
//back to hello.c
// instead of using (get_string) or (get__) as an operator use (input)

answer = input("What's your name? ")
print(f"hello, {answer}")

//addition.py
from cs50 import get_int

# Prompt user for x 
x = get_int("x: ")

# Prompt user for y
y = get_int("y: ")

# Perform addition
print(x + y)

//new syntax for addition.py
//have to cast from str to int because (+) operator will always concatenate as strings

# Prompt user for x 
x = int(input("x: "))

# Prompt user for y
y = int(input("y: "))

# Perform addition
print(x + y)

//division.py

#Prompt user for x
x = int(input("x: "))

#prompt user for y
y = int(input("y: "))

#perform division
print(x / y)


//conditions.py

from cs50 import

x = cs50.get_int("x: ")
y = cs50.get_int("y: ")

if x < y:
    print("x is greater than y")
elif x > y:
    print("x is less than y")
else:
    print("x is equal to y")
    
    
agree.py

from cs50 import get_string

s = get_string("Do you agree? ")

if s == "Y" or s == "y":
    print ("Agreed")
elif s == "N" or s == "n":
    print("Not agreed")
    
//another variation

from cs50 import get_string

s = get_string("Do you agree? ")

if s.lower() in ["y", "yes"]:
    print("Agreed.")
elif s.lower() in ["n", "no"]:
    print("Not agreed.")
    
    
//meow.py
//print meow 3 times

for i in range(3):
    print("meow")
    
//another variation

def main():
    for i in range(3):
        meow()

def meow(n):
    for i in range(n):
        print("meow")

main()



//positive.py

from cs50 import get_int


def main():
    i = get_positive_int()
    print(i)


    def get_positive_int():
        while True:
            n = get_int("Positive Integer: ")
            if n > 0:
                break
        return n
        
        
        
//mario.py

for i in range(3):
    print("#")
    
    
 /*print can take multiple arguments
 there is an understood (\n) at the end of each line in python
 inorder to remove it we must use the second argument in print end=""*/
 
 for i in range(4):
    print("?", end="\n") // this prints horizontally insead if vertically
 print()
 
 //another way to print is 
 
 print("?" * 4)
 
 
 //scores.py
 
 scores = [72, 73, 33]

print("Average: " + str(sum(scores) / len(scores)))


//another variation

scores = [72, 73, 33]

print(f"Average: {str(sum(scores) / len(scores))}


//another variation

scores = [72, 73, 33]

average = sum(scores) / len(scores)
print(f"Average: {average}")


//another variation

from cs50 import get_int

scores = []
for i in range(3):
    scores.append(get_int("Score: "))

average = sum(scores) / len(scores)
print(f"Average: {average}")






















 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
    
    
    
    
    
    
    
