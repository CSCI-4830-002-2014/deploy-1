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
8.12	1869
8.19	1870
8.54	1871
8.60	1872
7.62	1873
8.37	1874
13.64	1875
11.70	1876
8.37	1877
7.68	1878
8.60	1879
21.84	1880
17.44	1881
13.82	1882
9.33	1883
11.05	1884
9.11	1885
10.44	1886
9.95	1887
9.75	1888
14.59	1889
10.54	1890

The voltage reading was at a constant libration around 8 volts until this point in the code when it consistently rose. I think this is when the first visitors arrived.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  
8.60	15520
22.02	15521
43.35	15522
14.25	15523
15.46	15524
7.55	15525
At the very end of the collection, I got this huge spikes. It may have been a battery issue.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)
I could always perform a floor function to tone down the extremely loud values received, or if I were to conclude they are error points I can simply remove all points with values above a threshold number.


## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)
Cleaning. There is not much I can change with the sampling, so making a useful visualization will be most dificult.


## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

Even the wires of the arduino pick up noise because they can act as antennas. This user found a way to hack a medium pass filter to get only the values of interest http://www.elcojacobs.com/eleminating-noise-from-sensor-readings-on-arduino-with-digital-filtering/
