Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits
-3.4028235E+38 to 3.4028235E+38
http://arduino.cc/en/Reference/Float

## What amount of RAM is embedded on the arduino board? (2 pts)

32 KB
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

0->1023
10
http://arduino.cc/en/Reference/AnalogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 reads per second
http://arduino.cc/en/Reference/AnalogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

When dealing with many data points, we will hit problems if our data exceeds the built in data types, and we will also run into problems if we need to process more data than the Arduino can hold in its memory.


## What limitations may you run into doing data collection via arduino? (5 pts)
Your Arduino may not be able to sample fast enough, it vulnerable to environmental factors, and must be plugged in to a power source to be able to run.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
What do the sound levels look like in my room over the weekend?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

I am looking for people talking, and trying to see when the hill gets busy.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

8.43,267

7.81,268

8.12,269

7.55,270

8.77,271

9.43,272

9.17,273

7.42,274

8.06,275

9.38,276

9.33,277

10.05,278

8.94,279

8.77,280

8.19,281

9.17,282

8.31,283

8.89,284

8.94,285

9.17,286

8.77,287

8.94,288

It looks as if there is music playing here, the baseline output is about a 5, this is a significant spike.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

6.08,19245

5.74,19246

5.74,19247

5.74,19248

5.74,19249

10.63,19250

5.66,19251

5.66,19252

5.83,19253

5.83,19254

The 10.63 here happens during a quiet part of the night when nothing is happening. This must be a read error of some sort, it seems unlikely that a loud noise occured without my knowledge.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

Possibly eliminate outliers from subsets of the dataset. This is difficult to do without possibly destroying relevant data though. (What if a spike is because of someone yelping or something dropping? Also, a spike because of noise might not be considered an outlier even if it is noise.) The best way to remove noise is to do it before we have the numerical data by trying to ensure the signal the mocrophone is picking up is the best availiable. Intelligent data gathering.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

I am sure the cleaning will be the hardest part, numbers seem like they will be much harder to clean than words, there is much less data being conveyed.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

The Rugged Audio Shield is a shield that includes a microSD slot, but also includes a microphone in port, a microphone signal amplifier, and its own processor to handle the reads and writes with the SD card.
http://forum.arduino.cc/index.php?topic=104287.0
