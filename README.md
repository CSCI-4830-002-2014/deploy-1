Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits
maximum value: (2^31)-1
http://arduino.cc/en/Reference/long

## What amount of RAM is embedded on the arduino board? (2 pts)

2 KB (ATmega328)
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

10-bit analog to digital converter
integer values between 0 and 1023
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

maximum reading rate is about 10,000 times a second.
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

Data type sizes could be limited, although this isn't a big issue. The larger problem is learning how to multithread a process, have enough RAM, a fast processor and multiple CPUs, etc.

## What limitations may you run into doing data collection via arduino? (5 pts)

Some issues I've already run into is with the voltage. I think the 9 volt battery has caused some issues when hooked up to the 3V3 pin. You may also want more readings per second, but are limited to 10,000 (as we saw above). The machine can not be left to run on it's own since it will run out of memory space after just a few hours (although this has more to do with the SD card). Data types are more of an issue with the Arduino since it maxes at 32-bit.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)

I tested the noise level in my house over the weekend.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

I would love to see if the noise level got noticably louder during the night, and then quite quiet in the mornings. There was a point where my machine quit collecting "valuable" data, and it would also be neat to find out exactly when it broke.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

```
8.89,281,------324 seconds------

8.89,282

9.17,283

9.64,284

9.80,285

9.59,286

12.33,287

9.11,288

8.72,289

17.06,290

14.21,291,------336 seconds------

13.75,292

10.44,293

11.45,294

8.89,295

9.11,296

8.83,297

8.83,298

8.83,299
```
It seemed like the "average" sound in my living room remained at about 8 when it was mostly silent (i.e. with no people around). The few seconds in here where it jumps above that value indicates that someone was present in the room. Perhaps two people taking or someone washing their hands quickly. The level doesn't seem loud enough compared to other parts of the night, so it couldn't be loud music or shouting, but it's definitely some sort of activity. The recorder then dips back to ~8, perhaps indicating that whatever activity was going on ended and the room was "silent" again.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)

```
8.54,684

8.49,685

11.70,686

8.49,687

11.00,688

14.66,689

8.54,690

8.77,691,------797 seconds------

8.54,692

8.54,693

8.72,694

11.09,695

13.34,696

10.63,697

9.64,698
```
Here the data points seem to be all over the place. This occurs in a few parts of the recording, and it wouldn't make sense that someone was in the room at this time giving off this data. I'm not sure what could be going on here. Perhaps the noise was too far away for the sensor to make anything of it, or maybe a song was playing that had weird beat to it? Haha. It could have also been one of the times when I came close to check on the machince to make sure no one had found/tampered with it.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

I'm thinking that whenever I see high deltas between values over a very short amound of time (~30-60 seconds), it would be safe to assume the data is not what I want. More investigation would need to be done to verify this hypothesis, but it's a safe guess.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Definitely getting valid data. Now that I found a place that could potentially give me far better data than what I have, I would love a chance to let my machine run there. However, and this is also a reason why collecting data is so frustrating, the voltage levels from the batteries aren't playing nice with the Arduino, so that issue has to be fixed before any further collection can take place.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

I noticed that we are using port 3.3V. Looking online, the recommended input voltage is 7-12V. At first, I was using the 9V battery to collect remote data, and this worked fantastically for the first data collection I gathered. But once I tried to collect future sets, a strange pattern started to emerge where the machine would act normally for about 30 minutes, then all of a sudden the voltage would slowly (linearly) increase, without collecting data, go into the 100s, and just keep increasing usually at about 1-2 points at a time until I unplugged it. I tested this out on my computer and it worked properly, so it clearly has to do with the battery.

Once the class received the AA container, I attempted another data run, but the same thing happened. Each of the AA batteries I used are 1.5V, and there are 4 of them. I don't understand the linear increase in sound level over time, and since lowering the voltage by 3V clearly didn't help, I'm not quite sure what to do. I was thinking that I could re-solder the voltage to the 5V input pin, and then test again with the AA battery pack. If that doesn't work, I'm at a loss and would love assistance in getting my machine to collect more data. I have a better spot in the house now, and would love to be able to collect data from that area instead of my current dataset (which is fine, it could just be better).
http://arduino.cc/en/Main/arduinoBoardUno#Summary
