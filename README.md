Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits
4,294,967,295
https://learn.sparkfun.com/tutorials/data-types-in-arduino

## What amount of RAM is embedded on the arduino board? (2 pts)
The ATmega328 has 32 KB (with 0.5 KB used for the bootloader). 
It also has 2 KB of SRAM and 1 KB of EEPROM
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)
10 bits
0 -> 1023
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)
10,000 times/second
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]
We can hit a limit quickly with RAM because that is where our data recorded will be written to. In addition, we can easily reach the limits on the size for data types. 


## What limitations may you run into doing data collection via arduino? (5 pts)
I noticed the silent reading changed over time when the Arduino was being battery powered. This is a big issue because now are values are inconsistent for the same sounds and volume level.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
When throwing a party, what time does it get the loudest?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)
I want to take the total lenth of the party (in seconds). And determine as a ratio, when was it the loudest, and when did it start to get quieter (when did people leave).

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[Insert Data snippet]
[Explanation]

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Data snippet]
[Explanation]

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

[Explan your method]

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

[Explanation]

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

[Explain at least one tool]
[Provide URL to it]
