Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

[32 bits]
[2,147,483,647]
[http://arduino.cc/en/Reference/long]

## What amount of RAM is embedded on the arduino board? (2 pts)

[32 KB and 2 KB of SRAM and 1 KB of EEPROM]
[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone???]
[10 bit]
[http://arduino.cc/en/Reference/analogRead]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[about 10,000 times a second]
[http://arduino.cc/en/Reference/analogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Big data requires lots of memory or RAM and a laptop may not have enough to take on the heavy load. Getting more RAM or turning to the cloud are some options out there to help with memory problems.


## What limitations may you run into doing data collection via arduino? (5 pts)

You might run into the limitations in sampling rate and resolution.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
In the morning, does my bedroom get brighter at a constant rate or is there is spike in sunlight at a certain time?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

The signal I am looking for is a sudden spike in sunlight. I am looking for a time when the amount of sunlight increases faster than at any other time.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

Lost my original data (will do another sampling soon).
I did see the signal that I was looking for though. I graphed my data in a line graph and saw the spike in sunlight. I believe this is when the sun reached a point when my apartment building wasn’t blocking it. It was when the sun directly hit my window.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

My data seemed very clean and I did not notice any “noise”.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

If you know that the noise is not significant or just an “externality”, you can exclude it from the data set.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

My research question was pretty simple and I didn’t see one being more challenging than the other. In general though, I could see cleaning noise out being more challenging because deleting it would leave a gap and can make the analysis much more difficult.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

Arduino VB Lab is a GUI based tool. The nice thing about it is that it is possible to add data from sensors in a SQL Server database.

[http://sourceforge.net/projects/arduinovblab/?source=recommended]
