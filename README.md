# ColorDetection
I am building an application through which you can automatically get the name of the color by clicking on them.


## List of libraries used:
* numpy
* pandas
* OpenCV
* argparse


## Reason/inpiration behind this project:
I am learning about OpenCV library and I wanted to do something with the library.


## DataSets -
colors.csv - Details of color name and three primary colors Red, Green and Blue and hex number.


## About OpenCV - It is also known as Compuer Vision 
* I OpenCV library we can show image, brur it, make it black and white image with simple coding.
* cv2.imshow("original image",img) - To show the image.
* img = cv2.blur(img, ksize = (5, 5)) - To blur the image.
* I have drawn a rectangle and to get the color name to draw text on the window using cv2.rectangle and cv2.putText() function.


## Brief - 
* I am using argparse library to create an argument parser. So I can directly give an image path from the command prompt.
* I am using pandas library to read colors.csv file to load the data in the DataFrame.
* Calculate distance to get color name - I have the r,g and b values. Now, I have another function which will return us the color name     from RGB values. To get the color name, we calculate a distance(d) which tells us how close we are to color and choose the one having   minimum distance.
* To calculate distance d I used this Formulae - (d) = abs(Red – ithRedColor) + (Green – ithGreenColor) + (Blue – ithBlueColor)
* To run this program from command prompt - python color_detection.py -i <add your image path here>
* We can find the colors of any pictures by giving the image path and name.
