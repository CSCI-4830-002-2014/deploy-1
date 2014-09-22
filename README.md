Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

-32256 bytes max in an Arduino Uno.
[http://forum.arduino.cc/index.php/topic,28709.0.html]
-On the Arduino Uno (and other ATMega based boards) an int stores a 16-bit (2-byte) value. This yields a range of -32,768 to 32,767 (minimum value of -2^15 and a maximum value of (2^15) - 1). 
[http://arduino.cc/en/Reference/int]

## What amount of RAM is embedded on the arduino board? (2 pts)

There is 32 KB of RAM, 2 KB of SRAM, and 1 KB of EEPROM. 
[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

The max number representation range is between 0 and 1023, so 10 bits.
[http://arduino.cc/en/Reference/AnalogRead]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

The max sampling of AnalogRead is 10000 times per second.
[http://arduino.cc/en/Reference/AnalogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

One example would be when two laptops share the same program and run them on both laptops. But since both processors are different, each laptop will implement the code in a different order and logically might output different values. Memory barriers are placed at a certain position in code so that both processors output the same values. One example of a memory barrier in the real world:

The full fence implemented in the x86/x64 architecture. A full fence ensures that all load and store operations prior to the fence will have been committed prior to any loads and stores issued following the fence


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

Aside from the NaN at the initial start of my data, the difference of value between the 69th,70th, and 71st datapoints show that the amplitude of the sound waves are dropping. This shows that the sound is decreasing and getting quieter.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

10.63	2425
	
10.95	2426
	
11	2427
	
178.69	2428
	
248.98	2429
	
251.95	2430

It seems that the sound is fairly quiet or constant most of this trial at my work, but then a great adjustment in sound happens and the amplitude hikes up to about 15-20 the value of datapoint 2427. This could either do with my battery malfunctioning, me touching the microphone with my hand (I that a few times), or maybe just lous music being turned on after everything was quiet in the room recorded in. The 11 is either the noise associated with a quiet room or the 100-300 values are outliers and some sort of error.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

First, I would record a bit in a quiet room that is not affected by outside noises. I could then subtract that from my datapoints, plot this into Splunk, and then see how the dataset lines up in a timecount line graph. Then, I could go about finding outlier points and delete them since they might possibly be errors. They would have to be very large outliers and not match the patters obviously. This would help me get rid of the noise associated with the Arduino and quiet static rooms I may have recorded in.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

I think it will be a bit difficult to remove noise from my data and seperate where I actually recorded in my samplings through my noise data. But the noise data will probably prove to be more difficult in my case since I recorded outdoors, inside, and in multiple rooms that may contain more room noise than the other. This data may not come out to be accurate for the test that I am trying to do. 

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

The Analog Shield allows better resolution for smaller and more sensitive signals that cannot reliably be recorded 
or generated using the standard pins on the Arduino. There is a potentiometer that can adjust the amount of voltage being used in our Arduino board. This would prove useful with a voltmeter since there were some wiring issues with using a 3.3V pin with a battery more suited to use the 5 V pin on the board. Also, the Shield provides better measuring and recording information through the analongWrite and analogRead calls in the code.
[https://www.digilentinc.com/Data/Products/TI-ANALOG-SHIELD/AnalogShield_rm_rev3.pdf]
