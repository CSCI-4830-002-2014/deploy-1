Deploy and Learn (50 pts)
========

For each question in this section, please provide where you got your information via a URL in the [source URL] placeholder.  

## What maximum bit size does an Arduino Uno use and what's the largest number it can represent? (3 pts)

16 bit
32,767 (int)
http://arduino.cc/en/Reference/int

## What amount of RAM is embedded on the arduino board? (2 pts)

2 KB
http://arduino.cc/en/Main/arduinoBoardUno

## What is the maximum bit representation you can get from data using analogRead()?   (2 pts)

[10 bits]
http://arduino.cc/en/Reference/analogRead

## What is the maximum sampling rate of an analogRead() in arduino? (3 pts)

10,000 times/second
http://arduino.cc/en/Reference/analogRead

## When working with "Big Data" on your own laptop, what memory barriers might you run into?  Explain your answer. [5 pts]

[The ability to perform operations on big data is limited by the RAM of the laptop, which could be to low if the volume and velocity of the data is high enough. The storage of the laptop could be too small as well if the volume is large enough.]


## What limitations may you run into doing data collection via arduino? (5 pts)

Arduino's sampling rate may be too slow for certain measurements. Arduino can only store 8gb of data, which is approximately 7 - 8 million lines of data assuming 1024 bytes per line in .csv format

--------------------

For the next part of the assignment, you will look at your sample data.

## State the research question of your mini-project. (1 point)
Is there a time of night that I am particularly louder/in a louder surrounding?

## What would you define as your 'signal' you are looking for in your data?  That is, what might constitute as finding something of interest to your question? (5 pts)

I am looking for a specific period of heightened noise levels that is consistent across days of the week.

## Insert a small sample of your data where you notice something that might be a signal and explain why you think so. (5 pts)

44.97	6850	16975	Friday
43.83	6851	16976	Friday
44.46	6852	16977	Friday
43.84	6853	16978	Friday
43.78	6854	16979	Friday
43.69	6855	16980	Friday
43.62	6856	16981	Friday
43.71	6857	16982	Friday
44.01	6858	16983	Friday
43.84	6859	16984	Friday
43.66	6860	16985	Friday
44.36	6861	16986	Friday
45.96	6862	16987	Friday
45.84	6863	16988	Friday
43.7	6864	16989	Friday
43.61	6865	16990	Friday
43.7	6866	16991	Friday
43.69	6867	16992	Friday
43.73	6868	16993	Friday
43.67	6869	16994	Friday
43.66	6870	16995	Friday
43.65	6871	16996	Friday
43.67	6872	16997	Friday
43.6	6873	16998	Friday
46.02	6874	16999	Friday
45.23	6875	17000	Friday
44.4	6876	17001	Friday
44.2	6877	17002	Friday
43.6	6878	17003	Friday
43.78	6879	17004	Friday
43.77	6880	17005	Friday
44.2	6881	17006	Friday
43.69	6882	17007	Friday
43.6	6883	17008	Friday

The average volume levels here were higher. It could have been that music was playing or I was talking.

## Provide a data snippet of some noise you've encountered in your data collection, then try to explain it. (5 pts)  

43.37	6927	17052	Friday
43.43	6928	17053	Friday
43.41	6929	17054	Friday
47.52	6930	17055	Friday
46.01	6931	17056	Friday
45.83	6932	17057	Friday
47.27	6933	17058	Friday
45.88	6934	17059	Friday
167.03	6935	17060	Friday
85.49	6936	17061	Friday
52.49	6937	17062	Friday
49.22	6938	17063	Friday
257.11	6939	17064	Friday
43.76	6940	17065	Friday
46.02	6941	17066	Friday
156.76	6942	17067	Friday
87.42	6943	17068	Friday
43.22	6944	17069	Friday
47.21	6945	17070	Friday
73.57	6946	17071	Friday
283.8	6947	17072	Friday
45.81	6948	17073	Friday
55.41	6949	17074	Friday
43.62	6950	17075	Friday
43.47	6951	17076	Friday

The rows with 167.03, 257.11 and 156.76 volume levels are abnormally high.

## How might you go about getting rid of the noise? (Don't worry, we'll learn more about this, but try to think of a first method) (5 pt)

I'd find the standard deviation of the data and use it to find and remove the outliers

## For your research question, do you think your biggest challenge is in the sampling (i.e., getting valid data) or the analysis (i.e., cleaning noise out of your data)?  Explain (4 pts)

Sampling the data. It's important to make sure that data doesn't vary simply because at a certain point of time I put the microphone closer to sound/myself.

## In thinking ahead about the big project, what additional Arduino tools may be helpful for getting higher fidelity data?  Do a bit of your own research here.

In terms of the big project, I feel that a motion sensor would be helpful as we could use it to identify incoming data from when people actively near our project.
https://www.sparkfun.com/products/8630
