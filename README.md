Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits
3.4028235E+38
http://arduino.cc/en/Reference/Float

## What amount of RAM is embedded on the arduino board? (2 pts)

32 KB
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]
0-1023
10-bit
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 sample/second
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Well, there are many ways including but not limited to caching that can help with performance. They will be useless as the size of data grows. As a result, we have to read the data from the disk which is approximately 100,000 times slower. 

## What limitations may you run into doing data collection via arduino? (5 pts)

(1) It may not read samples often enough. (2) it's also vulnerable to power and volt changes like the battery issue we all faced in the first phase (anomaly in data because of battery).

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)

How does the amount light change during day and night in a living room.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

That sometimes when the lights are off (at night), there still might be a considerable amount of light because of moon light.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

9.49,3828

9.49,3829

9.49,3830

9.49,3831

9.49,3832

9.49,3833

9.49,3834

9.49,3835

9.49,3836

9.49,3837

9.49,3838

9.49,3839

9.49,3840

9.49,3841

9.49,3842

9.49,3843

9.49,3844

9.49,3845

9.49,3846

9.49,3847

9.49,3848

9.49,3849

9.33,3850

9.54,3851

7.21,3852

2.00,3853

2.00,3854

1.41,3855

1.41,3856

I frankly cannot say anything about this part of data but it seems like that lights went off at the end. it's not a signal but I couldn't find anything interesting.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

9.49,3843

9.49,3844

9.49,3845

9.49,3846

9.49,3847

9.49,3848

9.49,3849

9.33,3850

9.54,3851

7.21,3852

2.00,3853

2.00,3854

1.41,3855

1.41,3856

It's because the lights went off I assume.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

It may not be the best option but one is to visualize data, find the anomaly/noise and try to remove it using tools like splunk, excel or google refine.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Cleaning. We may have a lot of tools for cleaning but the challenge is to recognize anomaly. How to know when a noise in data is real or as a result of bad sampling.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.
