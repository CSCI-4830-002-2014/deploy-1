Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

64 (with `uint64_t`),
2^64=18446744073709551616
[source URL](http://www.nongnu.org/avr-libc/user-manual/group__avr__stdint.html)

**Note:** Assuming unsigned integers. Floating point values can be larger. The processor's instruction set only supports 8-bit integers, but larger integer types and floating point types can be emulated by the compiler.

## What amount of RAM is embedded on the arduino board? (2 pts)

2K Bytes (Internal SRAM)
[source URL](http://www.atmel.com/Images/doc8161.pdf)

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone?]
The Atmega328's ADC has 10 bit resolution. The maximum value you can get from `analogRead()` is 2^10-1=1023.
[Source URL](http://www.atmel.com/Images/doc8161.pdf)

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

"about 10,000 times a second."
[source URL](http://arduino.cc/en/Reference/analogRead)

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

For storing big data on your laptop, the barrier is the capacity of the harddrive/ssd since this determines how much data you can store.

For processing big data, the memory barrier is the amount of RAM in the computer since this limits the amount of data you can process.


## What limitations may you run into doing data collection via arduino? (5 pts)

* Not enough memory to store all data
* Not being able to store data due to limited data write bandwidth 
* Not enough processing power / RAM to process the data before storing it


--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
The data is the measured noise level from the parking lot outside my window, which I will try to use to determine at what time of the day the parking lot is the most active and thus when it is better to study in school vs at home.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

Finding some specific time range of the day (only looking at weekdays or weekends) when the noise level is the highest. It would also be interesting to see if weekends in general are higher in noise level, and whether there is any significant difference between the average signal for weekdays and weekends.

The signal could either be seen as the average noise level for the hours of the day, or the number of high-noise events during the day.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

![image](dataplot.png?raw=true)
In the image the x-axis is the number of days since Thursday 11 September 00:01am. Between 1.6 and 1.8 there is a "noise peak" that is going on for about 20 minutes.
This can be seen as a signal, since it indicates that I have had something loud outside my window. 

For the whole dataset the signal is clearly 24-hour cyclic, and some days appear to be "louder" than others.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

![image](dataplot2.png?raw=true)
There is one peak at about 9.5 that is much larger than any other data point. Why it is there is unclear, but it could be the wind or something physically touching the sound sensor.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

Outliers (data points with values far from the average) could be removed. Several data points could be combined by averaging the noise over e.g. a 5 minute window,
so that the noise level plot gets smoother.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)
Since the research question is about measuring noise, the noise in the data could be data as well. The data noise is likely only present for a few seconds at a time, so 
the number of data noise values should be small. Thus analysing the data should be the biggest challenge.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

A good way to get better fidelity data would be to use multiple audio sensors / arduino devices and measure data at nearby locations. Then if the data differs
much it is likely that one of them is noisy.
