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






