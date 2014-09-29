Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

32 bits,
4294967295,
https://learn.sparkfun.com/tutorials/data-types-in-arduino

## What amount of RAM is embedded on the arduino board? (2 pts)

32 KB Flash Memory and 2KB SRAM
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

0-1023,
10 bits,
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times per second
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

The memory barriers you could run into is your laptop could run out of memory causing your computer to run very slow.


## What limitations may you run into doing data collection via arduino? (5 pts)

Some limitations you could run into are the arduinos battery supply run out, or the drive runs
out of space.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
Using the data collected determine when I am home or when my house is just empty.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

A signal for me would be when the resting level of my house changes to something much higher then what it was.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)
17.66,1125
17.52,1126
32.20,1127
18.89,1128
29.15,1129
24.64,1130
17.80,1131
17.23,1132
15.30,1133
24.94,1134
23.32,1135
22.98,1136
22.74,1137
22.41,1138
22.27,1139
22.07,1140
73.11,1141
85.85,1142
20.22,1143
21.54,1144
21.70,1145
22.11,1146
21.84,1147
21.66,1148
21.77,1149
21.73,1150
21.73,1151
21.56,1152
21.82,1153
21.49,1154
21.59,1155
Compared to the resting level of my house this data reads consistently higher indicating that I am in my house.
## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  
21.26,25
21.45,26
102.35,27
90.70,28
21.54,29
21.40,30
As you can see the indexes of this data is very low so I was probably still moving the arduino into place.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

Data smoothing to smooth out these problems.

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

For my research question it is very easy for me to get data but the analysis is going to be the hard part.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.
I think that an ethernet shield would be very useful so we can connect our data to a server of some sort and provide real time data.
http://arduino.cc/en/Reference/Ethernet
