Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

-32256 bytes max in an Arduino Uno.
[http://forum.arduino.cc/index.php/topic,28709.0.html]
-On the Arduino Uno (and other ATMega based boards) an int stores a 16-bit (2-byte) value. This yields a range of -32,768 to 32,767 (minimum value of -2^15 and a maximum value of (2^15) - 1). 
[http://arduino.cc/en/Reference/int]

## What amount of RAM is embedded on the arduino board? (2 pts)

[RAM size]
[source URL]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]
[size in bits]
[Source URL]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[sampling rate]
[source URL]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

[Provide Explanation]


## What limitations may you run into doing data collection via arduino? (5 pts)

The battery may die out in the middle of one of your samplings.
Your mic might get messed with by cats or people depending on where you place it.
The amount of voltage used in this experiment might not output what is expected and still contain noise from the Arduino.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
What room is the best atmosphere (lowest sound) for studying in that has been recorded and is the outdoors a better place to study than a room recorded?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

I am looking for the highest wave amplitudes, or the pitch of sounds recorded to find out which room is the quietest and best to study in.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

405.96	21
	
405.96	22
	
405.95	23
	
405.63	24
	
404.25	25
	
403.97	26
	
403.97	27
	
403.96	28
	
403.97	29
	
403.97	30
	
404.94	31
	
404.07	32
	
404.93	33
	
405.35	34
	
405.94	35
	
305.61	36
	
372.75	37
	
390.38	38
	
393.95	39
	
396.92	40
	
399.93	41
	
400.95	42
	
401.94	43
	
401.96	44
	
402.94	45
	
401.7	46
	
400.07	47
	
399.95	48
	
399.89	49
	
399.83	50
	
399.63	51
	
399.56	52
	
398.86	53
	
399.54	54
	
402.21	55
	
352.36	56
	
387	57
	
391.96	58
	
392.92	59
	
392.96	60
	
393.95	61
	
395.93	62
	
396.95	63
	
396.98	64
	
396.97	65
	
397.64	66
	
396.42	67
	
395.01	68
	
396.38	69
	
247.7	70
	
11.96	71

Aside from the NaN at the initial start of my data, the 

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
