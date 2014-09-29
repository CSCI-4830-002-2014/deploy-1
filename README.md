Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

[32 bits]
[4,294,967,295]
[https://learn.sparkfun.com/tutorials/data-types-in-arduino]

## What amount of RAM is embedded on the arduino board? (2 pts)

[2 KB]
[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[10 bits]
[http://arduino.cc/en/Reference/analogRead]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[10,000 times/second]
[http://arduino.cc/en/Reference/analogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Big Data is just that-- big. By definition, it is data that is nearly impossible to contain in fast access memory. So trying to manage what little (relatively) amount of data is stored on RAM to provide fast analysis is a problem that the various tools we've used throughout the semester try to solve. 


## What limitations may you run into doing data collection via arduino? (5 pts)

Storing the data long term, getting accurate data, getting data that means anything at all, and/or finding a signal through the noise.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
To find out if our dog is barking throughout the day.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

Short, spontaneous spikes in noise level during normally quiet hours.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

8.06,97

7.75,98

7.62,99

11.53,100

8.25,101

8.06,102

7.68,103

8.66,104

7.35,105


You can see that the sensor was sampling quiet air space, but all of a sudden a loud sound was made. It was probably a bark.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

7.28,4

9.22,5

12.57,6

12.33,7

12.92,8

10.54,9

9.90,10

8.43,11

7.42,12

This was probably someone talking, a phone ringing, or something similar that made a sustained, loud noise.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

Finding areas where the sound is steadily quiet for a decent period of time, and then there are SHORT bursts of sound, filtering out, or even re-basing the sound level, for longer periods of loud noise.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Analysis will definitely be the harder problem to tackle, as I have to take into account all the varities of noise that occur in the house, what times are most likely for the dog to bark (when no one is home), and what actually is a bark.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

Some kind of IC that provides a time to the Arduino to more easily correlate data.
[http://playground.arduino.cc/code/time]
