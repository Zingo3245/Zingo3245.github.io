---
layout: post
title: Markov chains election simulator
---

Awhile back I made a program to simulate elections using Markov chains. It was an interesting subject considering that midterms are now less than a month away. This is a simple program that does not make accurate simulations of the 2018 midterm elections and is actually based on the 2016 elections. I've tried to have the probabilities based on polls and numbers when possible but I did have to guess at points. I've included some examples an introductions so people could review the concepts. I had to import numpy in order to make the random choices, default dictionary to keep track of my counters, and matplotlib for some simple graphs.

The first function was a simple simulator that used np.random.choice to pick between two results, Trump Wins and Hillary Wins. For each choice that was made I used += to add one to each win counter depending on who was picked. This was part of the older code that used if-else statements. I felt this was a good primer not just to make sure I had the simulator down but also because people are not always great with probability. In the aftermath of 2016, people were convinced that Hillary was supposed to win. In this simulation we noticed that Clinton won 66 times and Trump won 34 times.

In the next function, I decided to add an incumbency factor. When running simulations, the simulation would keep track of who won the last election and the probability will be adjusted based on which candidate won the election. I then decided to add primaries to the mix. The total candidate pool was expanded to five people(Hillary Clinton, Bernie Sanders, Donald Trump, Ted Cruz, and John Kasich). The simulator would first run a democratic and republican primary with the winner of those heading to a general election. In the next election, an incumbent would have a 90 percent chance of winning their own primary and face their own general election incumbency factor. I would like to thank Zach Miller for his suggestions to clean up previous if else statements.

![simulate_plot](/images/simulate_plot.png "simulate_plot")
![simulate_bar_graph](/images/simulate_bar_graph.png "simulate_bar_graph")