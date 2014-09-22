Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

This is vauge, but I assume you mean what the largest interger value possible on Ardino is, which would probably be an unsigned Long

- 2 Bytes (16 bits)
- 65535
- http://arduino.cc/en/Reference/UnsignedInt

## What amount of RAM is embedded on the arduino board? (2 pts)

- 2 KB
- http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

- AnalogRead returns an int for 0 to 1024
- 2^8
- http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

- around 10000 times a second
- http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Assuming my laptop is now the limiter: One I have already run into is my C drive has less than a gig of space on it. Many programs let 
you decide where you would like to install, but use a temp file buffer on C regardless. This leads to me constantly fighting with
my Windows installation to free up a couple of gigs of space when need be. Another problem I might run into is the need to store
massive arrays/buffers/strings in memory. I could easiy exceed the 4GB RAM allocation if I'm not careful.

## What limitations may you run into doing data collection via arduino? (5 pts)

Already fought with this quite a bit. I am trying to write a script that stores as many values as possible in concated strings/ a string
array before the very, very slow operation of opening the SD card and writing to it. This leads to needing to figure out the max string/array
I can store before needing to reset. I also have a hunch that my code currently has a memeory leak, I need to learn a bit about garbage collection
in Aurdino.
--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
Is it possible to get high enough fidelity data from our Sound Sensor such that one can recognize musical frequencies?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

The "Signal" I am lookin for is a sequence of voltages that looks like a sine wave when plotted against time. This needs to be high enough
fidelity that I can run it through FFT or another wave-collapse function to analyze the sample against known musical frequencies

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[Insert Data snippet] Still Playing
[Explanation] Still Playing

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Data snippet] Still Playing

My code is set up to listen for a "loud (intial)" noise, and then sample at close to the maximum rate for around a second afteword. This was likely
from when I made a loud sound while not playing a note, leading to the next second fo "garbage" being collected.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

I can safely throw out all data that doesn't have the sine wave pattern I am looking for. The easiest way to do this may be to conduct anlysis against
all data I have, and then throw out all values that are "too far" from a goal value.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Gathering the data seems like it will be the larger challange. I spent ~5 hours fighting with aurdinos memory restrictions, but now that I have data it, easiy seperated by sample index, it seems like it will be somewhat straight forward to throw out nonsense data.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

"Higher Fidelity" data is a big vauge. I assume you mean for sound/light! Sparkfun seems ot have a ton of cool addons. We could pick up a more sensitive microphone [https://www.sparkfun.com/products/12656]. Personally I think the biometrics look like a ton of fun [https://www.sparkfun.com/categories/146]. I have a vision for an "accidently interactive" display in the ATLAS lobby, and I think we could do some fun things with biometrics. 
