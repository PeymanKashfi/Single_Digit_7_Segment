# Single_Digit_7_Segment
This is a simple project for STM32L476 NUCLEO board to work with a single digit 7-segment LED.  
  
First, I setup the clock to the maximum 80MHz.  
Then, I configure the corresponding GPIO pins as GPIO output in .ioc file.  
  
Each segment connected to a GPIO port as folows:  
a --> PC0  
b --> PC1  
c --> PC2  
d --> PC3  
e --> PC4  
f --> PC5  
g --> PC6  
DP --> PC7  
  
To display each number we should setup the following segments:  
0: a, b, c, d, e, f --> 1  g --> 0  
1: b, c --> 1  a, d, e, f, g --> 0  
2: a, b, g, e, d --> 1  f, c --> 0  
3: a, b, c, d, g --> 1  f, e --> 0  
4: f, g, b, c --> 1  a, e, d --> 0  
5: a, f, g, c, d --> 1  b, e --> 0  
