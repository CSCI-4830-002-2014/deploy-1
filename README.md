Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

[16 bit]
[32,767]
[http://arduino.cc/en/Reference/int]

## What amount of RAM is embedded on the arduino board? (2 pts)

[32k bytes]
[http://arduino.cc/en/Tutorial/Memory]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]
[1023]
[http://arduino.cc/en/Reference/analogRead]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[10,000 a second]
[http://arduino.cc/en/Reference/analogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

[My laptop only has 80 gigabytes of hard disk space, so I could easily see that filling up if i was doing the full 10,000 readings a second over a long period of time. Also if we are editing large amounts of data my processsor would take forever.]


## What limitations may you run into doing data collection via arduino? (5 pts)

[Running out of battery, small RAM so data points can't be that big, can't do real time processing. ]

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
[To research how loud my room can get and when it gets the loudest throughout a 3 year period]

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

[Finding to find if theres any pattern of noise in my room, (while music was playing if it was louder)]

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[16.43,5470
19.92,5471
16.22,5472
16.76,5473
20.83,5474
13.45,5475
12.96,5476
13.19,5477
18.22,5478
15.78,5479
33.54,5480
50.44,5481
23.64,5482
30.25,5483
21.10,5484
49.38,5485
30.25,5486
14.90,5487
31.58,5488
34.25,5489
25.51,5490
24.21,5491
24.43,5492
15.87,5493]
[The sound gets averagd over a second, so we can see it spike up from its usual(15), because I believe someone was in my room talking at that point.]

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[12.73,5449
13.27,5450
12.85,5451
19.49,5452
13.42,5453
25.04,5454
13.67,5455
12.37,5456
12.53,5457
12.53,5458
14.97,5459
13.15,5460
12.57,5461
12.57,5462
12.53,5463
12.96,5464
15.65,5465
134.93,5466
321.63,5467
27.86,5468
20.57,5469]
[We can see a huge spike, possibly because the window was open and wind blew into the sensor.]

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

[Just have a cut off of if over 100 then remove the data.]

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

[I'd say the sampling, because it is tough to test whether or not you're getting good data bu]

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

[ Arduino Dashboard is an application for monitoring in real-time the analog and digital pin sensors values interfaced with an Arduino]
[http://www.lvl1.org/2011/07/04/arduino-dashboard-app/]
