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
