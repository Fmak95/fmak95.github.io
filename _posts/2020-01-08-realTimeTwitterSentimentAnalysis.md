---
title: "Real Time Sentiment Tracking with Twitter"
date: 2020-01-08
excerpt: "A real-time web app based on data pipelines using streaming Twitter data, automated sentiment analysis, and MySQL database."
---

Code for the project can be found <a href="https://github.com/Fmak95/real-time-sentiment-tracking-with-twitter">here.</a>
![alt](/assets/gifs/twitter-example.gif)

## Inspiration
Twitter is a social media platform where everyone posts their opinion on certain topics. Using sentiment analysis one can get a general idea of how the overall population is feeling towards a brand, company, political leader or anything else. By monitoring this information, companies can make more informed decisions that would improve customer satisfaction.

## The Approach
The main two components of this web application are the ```streamer.py``` and ```app.py``` files respectively. In the ```streamer.py``` program, I make use of <a href="https://www.tweepy.org/">Tweepy</a>, a simple Python library that uses the Twitter API to collect tweet data. Then, the sentiment of the tweets are extracted using VaderSentiment, a lexicon rule-based sentiment analysis tool, which is specifically tuned to perform well social media texts (i.e. Tweets from Twitter). All of this information is then stored into a local mySQL database.

The ```app.py``` program is in charge of data visualization. I use <a href = "https://plot.ly/">plotly</a> and <a href = "https://plot.ly/dash/">dash</a> to create an interactive dashboard that presents all of the information. This program connects to the same mySQL database and processes the data in real-time.

