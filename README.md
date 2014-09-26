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
To figure out at what time my living room is loudest. 

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

My theory is that the ambient noise level of ambient noise is directly tied to when my roommates and I get back to the house. 

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

time    noise       index	
1		25.9		1	
		
3		31.43		2
		
4		20.57		3
		
5		20.9		4	
		
6		20.98		5
		
7		21.42		6
		
8		23.32		7
		
9		23.75		8
		
11		21.7		9	
			
12		22.11		10
		
13		19.67		11
		
14		19.77		12
		
15		24.06		13
		
16		22.16		14
		
17		41.95		15
		
19		22.56		16

Here is our noise levels after various times. We can see  clearly modulation during a normal conversation around a dinner table

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

time 	noise 	index

15837	176.79	13637
		
15838	178.57	13638
		
1		163.42	1
		
1		163.38	1
		
1		163.38	1

Here we see that the arduino must have somehow reset itself. 15,838 seconds after the experiment began. 

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

My first method would simply be adding the time of when the device shut off, to when it reset. Although this might not be accurate because I have no idea how long it was off for. 

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

I think the most difficult challenge with this assignment is cleaning out the noise because I don't know if I can even find any useful data from this project. 

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

We can attach this antenna to the arduino and have it uplaoding its data in real time so we can know if/when it shuts down and have easier access to quick data analysis. 

[http://ebay.to/1qAtMoz]
