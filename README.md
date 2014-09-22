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

Depending on the scale of the data (much larger than this sample data), the files may be too large to store in cache or even RAM and thus be slow to access because so much is off disk.  The files may be too big to fit on my hard drive and could require a cloud based solution.


## What limitations may you run into doing data collection via arduino? (5 pts)

Read speed and write speed could be too slow to properly collect data, and additionally the low memory can handicap any real mathematical functionality. The data has to be collected and processed later because 32 KB of ram is not nearly enough for most functionality of data processing on the fly.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
This has changed since Make 1A since my data was kind of a mess.  I now put my arduino by my TV to determine how the volume of a TV broadcast of a football game (Broncos vs. Seahawks) varies with the events occuring in the game.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

If I found consistent correlations of higher volumes with interesting events (touchdowns, sacks, etc.), I would be satisfied.  Although I do know that TV broadcasts are both limited and compressed so these may or may not occur.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)



83953,16.49,11690668


83954,15.62,11690807


83955,17.64,11690946


83956,16.31,11691085


83957,20.07,11691224


83958,31.69,11691369


83959,24.35,11691507


83960,18.00,11691657


83961,16.43,11691796


83962,16.52,11691947


83963,14.53,11692085

Since these unusually large voltage values are grouped together, I am hoping they correspond to an event in the football game.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

85909,35.55,11964039

85910,18.19,11964178

85911,16.06,11964317

85912,15.26,11964455

85913,129.82,11964605

85914,183.47,11964744

85915,127.40,11964883

85916,26.74,11965022

85917,14.56,11965161

85918,13.08,11965305

85919,15.62,11965445

85920,17.46,11965583

We see completely ridiculous voltages - up to 183.47.  These outliers suggest that possibly the microphone was touched or something weird happened electrically.



## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

I would do statistical analysis and weed out any complete outliers, or it would be fairly simple to lay down a threshold and remove (or smoothen) points that are out of the trend and out of question.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

It'll be an interesting challenge to eliminate the commercial data, as well as finding the exact times touchdowns were scored, etc. to compare with. 

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

One place I took the easy way out was timing.  I used arduino's millis() function to get milliseconds from startup.  To make something more functional and long lasting, I think it would be beneficial to use Ardunio's Time Library.  This will not get off over time and has more powerful output functionality. The library's documentation can be found at:
http://playground.arduino.cc/code/time
[Provide URL to it]
