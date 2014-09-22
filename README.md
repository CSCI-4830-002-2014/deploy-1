Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

64,
2^64=18446744073709551616
[source URL](http://www.nongnu.org/avr-libc/user-manual/group__avr__stdint.html)

**Note:** Assuming unsigned integers. Floating point values can be larger. The processor's instruction set only supports 8-bit integers, but larger integer types and floating point types can be emulated by the compiler.

## What amount of RAM is embedded on the arduino board? (2 pts)

2K Bytes (Internal SRAM)
[source URL](http://www.atmel.com/Images/doc8161.pdf)

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[phone?]
The Atmega328's ADC has 10 bit resolution.
[Source URL](http://www.atmel.com/Images/doc8161.pdf)

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

"about 10,000 times a second."
[source URL](http://arduino.cc/en/Reference/analogRead)

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

For storing big data on your laptop, the barrier is the capacity of the harddrive/ssd since this determines how much data you can store.

For processing big data, the memory barrier is the amount of RAM in the computer since this limits the amount of data you can process.


## What limitations may you run into doing data collection via arduino? (5 pts)

* Not enough memory to store all data
* Not being able to store data due to limited data write bandwidth 
* Not enough processing power / RAM to process the data before storing it


--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
[Statement here]

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

[Response]

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

[Insert Data snippet]
[Explanation]

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

[Data snippet]
[Explanation]

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

[Explan your method]

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

[Explanation]

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

[Explain at least one tool]
[Provide URL to it]
