Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

[10]
[1023]
[http://arduino.cc/en/Main/arduinoBoardUno]

## What amount of RAM is embedded on the arduino board? (2 pts)

[2 KB]
[http://arduino.cc/en/Main/arduinoBoardUno]

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone]
[10 bits]
[http://arduino.cc/en/Reference/analogRead]

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

[10,000 times per second]
[http://arduino.cc/en/Reference/analogRead]

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

The memory barriers that I might run into when working with Big Data is that I will not be able to store a massive databse on my laptop. Thus, I would not be able to do a true "Big Data" project if I only had by laptop to host it; chances are I would have to access the data from an outside server. Even then, I would have to be careful how I query and access the data becuase a bad query can make the process run very slowly; when I worked at a company called Genscape, I had to run a query on a laptop that took 20 minutes to run. 

## What limitations may you run into doing data collection via arduino? (5 pts)

With arduino, I can only work with 2KB of RAM. Also, the data that arduino provides me is very basic and will require more analysis on my part to get something out of it. Also, arduino does not do timestamps, which is a particular issue for me since my data is time-based. This means I will have to do extra work by approximating the time I spent in the UMC and adding an x-axis to my data, which will probably be done in Numbers. In retrospect, I probably should have printed the index along with my data points. 

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)

I am trying to find the optimal time to study at the UMC based on noise levels; the less noise, the better.

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

I am looking at volumes of ambient noise. Something of interest to me would be pro-longed spikes and pro-longed decreases in noise as those would give indicators of bad and good times to study at the UMC respectively.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

16.82

16.03

18.30

17.03

This is a signal because there is a noticeable spike in the data. This probably happened when some people walked passed me having a loud conversation.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

15.97

15.56

16.12

74.15

15.56

15.46

16.16

This rather extreme spike may have happened with I moved my computer and disrupted my arduino by accident. I beleive this happend a few more times in my data.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

One method I would look at is to get rid of outliers. One way of doing this is comparing the max and min values of the data with the median. If the difference between the median and the max and/or min values is significant enough, then the max or min is an outlier and needs to be deleted. Repeat until you are satisfied with the range of data.  

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

The analysis. To my knowledge, arduino does not do timestamps. This is an issue becuase my study is time-based and I may need to approximate the time for each of my data points, which were printed once a second. There are a couple extreme spikes in my data, and I will have to sort out whether those spikes were actual noises or just mistakes when I disrupted my arduino.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

The MatLab interface allows you to control the arduino using MatLab, which is a great programming language when it comes to processing data.

http://playground.arduino.cc/Interfacing/Matlab

Apparently, arduino does have a time library. This will be much more useful if the bigger project I do is similar to my mini-project.

http://playground.arduino.cc/Code/Time
