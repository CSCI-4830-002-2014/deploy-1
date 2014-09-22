Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32-bit
3.4028235E+38
https://learn.sparkfun.com/tutorials/data-types-in-arduino

## What amount of RAM is embedded on the arduino board? (2 pts)

Flash  32k bytes (of which .5k is used for the bootloader)
SRAM   2k bytes
EEPROM 1k byte
http://arduino.cc/en/Tutorial/Memory

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

int
1023
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times a second
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

My laptop would probably not have enough space to store too much data (without some sort of cloud or external drive(s)).  Additionally, processing the data can boost up the CPU and RAM usage to an almost unusable point.


## What limitations may you run into doing data collection via arduino? (5 pts)

The card on the arduino is limited in size.  Additionally, the 10,000 sampling-per-second may not be enough for some advanced frequency/graphical analysis (although my personal project should be fine).  I ran some Arduino code that I found on the internet and discovered that it instantly crashed my computer, so I suppose that it also a risk somehow.  Lastly, there is always a risk of excessively “noisy” data or dying batteries, which require a lot of cleaning and calibration to be used accurately.


--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
How can we identify frequency of an input and, if within a reasonable scope, how can we use pitch analysis to “guess” the particular key of a song?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

Correctly identifying a pitch would be most interesting to me because that can contribute to the bigger idea of making a reasonable guess of the key.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[B-flat played on accordion](DATALOG_accordBflat.CSV) and
[E played on accordion](DATALOG_accordE.CSV)
These are snippets of a B-flat and an E being played on an accordion.  I chose an accordion because it sustains better than, say, a piano or guitar.  I’d like to say that I can see some wave-like readings, but it’s really hard to tell at this stage.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Noise on accordion](DATALOG_noisy.CSV)
I’m not sure how to identify noise quite yet, so I made a recording of myself snapping to see extreme variations in volume.  The reason I did this is because I’m assuming volume will be an unwanted variable in this analysis.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

Look for outliers and long-term trends (in the case that there is a Arduino issue that is causing an unrepresentational long-term change in the data).

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

In the initial stages, I think the biggest difficulty will be the analysis.  However, once trends are identified, I hope to take more complex samples. Multi-frequency samples may be quite difficult to both sample and analyze since more variables will probably be introduced (combined volume, overtones, etc.).

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

Using the tone() function, you can generate square waves to be played out of a pin.  It would be neat to be able to “hear” what the our code is interpreting, rather than just reading graphs, etc.  I think this concept would be similar to MIDI, but I don’t know too much about that.
http://arduino.cc/en/reference/tone
