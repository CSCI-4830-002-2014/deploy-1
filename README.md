Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

Float - 32 Bits
3.4028235E+38
http://arduino.cc/en/Reference/Float

## What amount of RAM is embedded on the arduino board? (2 pts)

32 KB
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

0 to 1023
10 bits
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 reads / 1 sec
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Not having enough RAM on your laptop, and it would make your laptop run exceptionally slow.


## What limitations may you run into doing data collection via arduino? (5 pts)

The speed of reading would definitely be a big problem. This is very similar to the previous question where not having enough memory really slows it down.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
My research statement is how loud a room can get in a fraternity house room on a weekend (Thursday-Sunday morning).

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

The louder the levels get, the louder the room was at that time usually between 10:30-1am.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

148.99	75696
	
235.37	75697
	
329.15	75698
	
310.86	75699
	
343.32	75700
	
308.63	75701
	
320.06	75702
	
331.39	75703
	
296.46	75704
	
340.34	75705
	
314.76	75706
	
316.08	75707
	
366.51	75708
	
420.71	75709
	
159.93	75710
	
158.46	75711
	
157.12	75712

When the code reads in the 300's or above that usually shows that there was an event in that room.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

380.54	75865
	
356.56	75866
	
354.48	75867
	
336.26	75868
	
300.09	75869
	
230.95	75870
	
180.96	75871
	
323.41	75872
	
331.72	75873
	
298.72	75874
	
338.41	75875
	
316.54	75876

Where there is a noise level of 180.96 it is unusually low for the data at that time so there is the possibility that either the noise level was lower or someone fiddled with the noise sensor.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

I would just have to go through the data and figure out when weird data sets like this appear in weird times and remove them.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Definitely the analysis because their will definitely be weird sample points like this throughout the data sampling time.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

I would have to say the time function because it would have been nice to be able to determine an easier way too look at time for my data.
http://playground.arduino.cc/code/time
