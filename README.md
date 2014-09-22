Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

16 bit

32767

(http://arduino.cc/en/Reference/int)[http://arduino.cc/en/Reference/int]

## What amount of RAM is embedded on the arduino board? (2 pts)

2 kB

(http://arduino.cc/en/Main/arduinoBoardUno)[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]

10 bit

(http://arduino.cc/en/Main/arduinoBoardUno)[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times per second

(http://arduino.cc/en/Reference/analogRead)[http://arduino.cc/en/Reference/analogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

When working with very large samples of data, performing operations on that data could lead slow down a laptop computer that doesn't have the memory to support operating on that scale of data.


## What limitations may you run into doing data collection via arduino? (5 pts)

As discussed in class, the Arduino's bit size limits the maximum size of an integer, which can throw off counts in the code. It's important to keep this in mind when doing math with integers and use long ints as appropriate.

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
How does sound level in the living room vary over the course of a Friday night, after inviting guests.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

A base line can be identified when first setting up the arduino, as the room was quiet. Increases in the value indiciate more people or louder music, so it can be hypothesized that higher values will be observed in the data when people began to come over.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[169.99,2:53:40

170.09,2:53:41

170.20,2:53:42

170.09,2:53:43

170.21,2:53:44

170.13,2:53:45

170.13,2:53:47

170.03,2:53:48

170.03,2:53:49]

[It's difficult to tell as the measurement was only recorded once per second and the sound gradually increased, but the sound levels at 8pm were about 167 while at 11pm when people began to come over, the level had increased to 170.]

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[
181.57,3:44:55

187.81,3:44:56

209.36,3:44:58

200.90,3:44:59

210.30,3:45:0

238.99,3:45:1

261.28,3:45:2

309.30,3:45:3

249.72,3:45:5

234.94,3:45:6

197.79,3:45:7

237.35,3:45:8]

[The values demonstrate a sharp spike at 3:45:3, in contrast to the values of 170-173 that preceded this snippet. The values increased steadily before the spike, however, which may suggest someone turned up the volume on the stereo rather than noise.]

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

[Perhaps alternative averaging methods could better smooth the data. Data analysis could also be performed to remove outliers. ]

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

[For this particular research question, the biggest challenge is the analysis. By simply keeping the arduino in the living room, I've introduced a lot of variability. Proximity to the sensor makes a signficiant difference in the measured values, and with so many people in the room and a variety of different sounds, it is difficult to control outlying events, which in turn makes it hard to identify whether or not outliers in the data were simply noise or a meaningful event.]

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

This data logging shield for Arduino has similar functionality to the microSD shield we used, though one key feature it has is a Real Time Clock. It's possible that I just couldn't figure it out on my own, but I believe the Arduino is unable to maintain accurate time on its own. This shield has a clock onboard that lasts for years. Correct timing of data is vital to data analysis so that specific events can be identified within a dataset. 

(http://www.adafruit.com/products/1141?gclid=COW83Iyb9MACFaQ7Mgod4QMA_w)[http://www.adafruit.com/products/1141?gclid=COW83Iyb9MACFaQ7Mgod4QMA_w]
