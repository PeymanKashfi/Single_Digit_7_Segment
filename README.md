# Single_Digit_7_Segment
This is a simple project for STM32L476 NUCLEO board to work with a single digit 7-segment LED.  
  
First, I setup the clock to the maximum 80MHz.  
Then, I configure the corresponding GPIO pins as GPIO output in .ioc file.  
  
Each segment connected to a GPIO port as folows:  
a --> PB9  
b --> PB8  
c --> PB5  
d --> PB4  
e --> PB3  
f --> PA5  
g --> PA6  
DP --> PB6  
  
To display each number we should setup the following segments:  
0 : a, b, c, d, e, f --> 1  g --> 0  

