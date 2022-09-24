---
title: "Space Invaders AI"
date: 2022-09-23T22:24:46-03:00
draft: false
---

I was about 16 when a friend showed me a video of an [AI playing Super Mario](https://www.youtube.com/watch?v=qv6UVOQ0F44). This had a great influence on my decision to learn how to code. To this day, reinforcement learning is my favorite area of machine learning and I find genetic computing very intriguing.

Recently I had the chance to try something like that by myself in a class I took about Machine Learning (although in much smaller scale). I used the [Arcade Learning Enviroment](https://github.com/mgbellemare/Arcade-Learning-Environment) to simulate Space Invaders as my enviroment for a neural network agent to play.

Initially, my team and I wanted to implement the [Rainbow Deep Learning](https://arxiv.org/abs/1710.02298) algorithm to train our model. We soon found out that we did not have the hardware necessary to run it. So we split tasks. 

They were responsible for tuning down the algorithm so we could run something like it. I became responsible for trying to use an evolutionary algorithm to solve our problem. That makes sense when you consider that evolutionary algorithms tend to converge very fast towards a local optimum (you get a solution, but it's not the best solution).

The video below shows how my evolutionary algorithm solved the problem. It found a local optimum where it just tries to shoot a bonus enemy.

{{< youtube id=S1KU7yZpV7g >}}