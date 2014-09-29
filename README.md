Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

16-bit (2 byte)
32,767
http://arduino.cc/en/Reference/int

## What amount of RAM is embedded on the arduino board? (2 pts)

2 KB
http://arduino.cc/en/Main/ArduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

1023 maximim 
10-bits
http://arduino.cc/en/Reference/AnalogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times per second
http://arduino.cc/en/Reference/AnalogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

If the data is very large, there is a limitation in the disk storage space available, especially with the prevalence of SSD drives of smaller capacity. There is also an issue of limited RAM if a lot of data is being processed at the same time. 


## What limitations may you run into doing data collection via arduino? (5 pts)

The processor isn't very powerful, so processing several signals at once (if that's your goal) might not be possible without some issues. Collecting a large amount of data is impossible without an external memory source. Some data collection (for example, video) is impossible with arduino's limited RAM.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
I wanted to measure the highway road noise outside my window to determine when there is the most traffic and when the roads are most quiet.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

The signal of my data is one or more ranges of particularly high/low noise readings. This would signify high or low traffic patterns. 

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[Snippet 1](snippet1.txt)
This is a small snippet of code where there is a noticable spike in the sound data for a brief period of time. I think this is a good example of some significant road noise. In this case, I would guess that only 1 car passed by and that is why the spike was short lived. Heavy traffic would lead to a longer sustained spike.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Snippet 2](snippet2.txt)
Throughout the data there's many snipets where the baseline rests at either 9 or 10. This makes things hard to follow because normally you'd want complete silence to be 0, but here it seems to be 9 or 10. 

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

The sound sensor can be moved closer to the sound source to get a better sound reading. The data might also be easier to read if was normalized, that way the peaks and troughs are more definitive. 

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Sampling. Because the arduino is decently far away from the sound source, it's not picking up strong noise patterns like those I hear when I sit in my room. This is a problem because the data poorly reflects the dramatic changes in road noise levels. In my orignal data set I also didn't time stamp my data, so there is no way to understand what the data points really mean. This was more of a preliminary test to see if the sensor detected peaks in sound.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

A temperature sensor could be used to see if there is any variance in driving volume/traffic levels with the temperature, especially as the weather gets worse this semseter. 
https://www.sparkfun.com/products/11050
