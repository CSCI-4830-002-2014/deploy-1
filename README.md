Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits,
4,294,967,295,
https://learn.sparkfun.com/tutorials/data-types-in-arduino

## What amount of RAM is embedded on the arduino board? (2 pts)

RAM = 32 KB with 2 KB of SRAM and 1 KB of EEPROM,
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

1023,
10 bits,
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times per second,
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

A possible memory barrier issue that you can run into might have to do when trying to analyze or index a lot of data in splunk. You might not be able to store it properly in memory for proper speed or timely results.


## What limitations may you run into doing data collection via arduino? (5 pts)

With the Arduino, we are limited by two main things: 
1. Power, we might not have batteries at hand keep the device going for truly sustained observation. 
2. Storage, we might fill up our SD card and be unable to take any further measurments without overwriting important data. 

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
[Statement here]

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

[Response]

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
