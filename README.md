Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

[size]
32
[number]
2^31 - 1
[source URL]
http://arduino.cc/en/Reference/long

## What amount of RAM is embedded on the arduino board? (2 pts)

[RAM size]
32KB
[source URL]
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]
[size in bits]
10-bit
[Source URL]
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[sampling rate]
10,000 samples / second
[source URL]
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

[Provide Explanation]
With big data (especially with data insertion), memory can be a big bottleck. Essentially,
it is always useful to give your database/program a hunk of ram. Also, you want to make sure
you avoid performance bottle necks like thrashing (evicting your cache constantly). On my laptop,
I have 16GB of memory so I should be fine. That is about equal to an m3.medium on AWS EC2.


## What limitations may you run into doing data collection via arduino? (5 pts)

[Provide Explanation]
- The voltage of the battery dropping
- Too loud of a noisefloor
- Weather conditions preventing outside usage, etc.
- Lack of computation power, limited amount of memory

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)

[Statement here]
Can you predict traffic patterns in the CSEL using noise levels.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

[Response]
A higher level of ambient/crowd noise might dictate that more people were in the building.
Lower levels of of variance in sound amplitude levels would mean less peeople are there.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[Insert Data snippet]
7.14,2195

6.32,2196

6.78,2197

6.00,2198

9.43,2199

6.56,2200

5.29,2201

6.63,2202

5.57,2203

5.00,2204

5.00,2205

4.69,2206

4.80,2207

5.10,2208

5.10,2209

5.83,2210

4.90,2211

5.48,2212

5.92,2213

5.39,2214

[Explanation]
During this period, it seems like I was talking to someone in the CSEL.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Data snippet]

7.14,2195

6.32,2196

6.78,2197

6.00,2198

9.43,2199

6.56,2200

5.29,2201

6.63,2202

5.57,2203

5.00,2204

5.00,2205

4.69,2206

4.80,2207

5.10,2208

5.10,2209

5.83,2210

4.90,2211

5.48,2212

5.92,2213

5.39,2214
[Explanation]
This is when I whistled into the microphone to test it :)

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

[Explan your method]

- You can set a threshold which will turn the volume down whenever noise goes below that level.
- You can filter out frequencies known to be useless (low rumbles, etc)

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

[Explanation]

Definitely getting the signal. I have more failed attempts than I can count, and am still not fully satisfied
with my signal. The first time, my 9-volt battery created a linear increase in noise. On my second attempt with AA
batteries, no data was picked up after a few hundred samples.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

[Explain at least one tool]
- A good power supply to get a steady signal. Possibly even a USB recharger would do!
- A case!

[Provide URL to it]
Recharger: http://www.amazon.com/Duracell-Instant-Charger-Includes-Universal/dp/B002FU6KF2
Case: http://www.adafruit.com/products/337
