---
title: "Anime Recommendation System"
date: 2020-01-15
excerpt: "A recommendation system that suggests anime shows to watch based on your myanimelist profile."
---

The code related to this article can be found <a href="https://github.com/Fmak95/recsys-collaborative-filtering">here.</a> I provide a quick tutorial of performing collaborative filtering with a well known recommendation system library called <a href="https://surprise.readthedocs.io/en/stable/">scikit-surprise</a>, as well as my very own implementation using Keras.

## Anime Recommendation System
Have you ever faced the problem of trying to discover a new television series to watch? Trust me, we have all been there. If you are going to invest your precious time and emotional energy to connect with a tv show character, then it better be a good show! 

Enter recommendation systems, which are programs that suggests you tv shows you might enjoy watching. So how does this recommendation system know what I would like to watch? The simple answer is data. The more complicated answer is through a technique called collaborative filtering. In simple terms, collaborative filtering suggests you shows based on your recent watch history and compares that to data on other users who have similar watch histories.

I've written a short program that suggests people a new anime series to watch based on their past scoring metrics from the popular anime site: <a href="https://myanimelist.net/">myanimelist.</a>