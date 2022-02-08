---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## Human-assisted Activity Recognition
*Jan 2022 - Present*

Currently researching ways to improve a video-based activity recognition system by incorporating knowledge from human narration under the supervision of Prof. Thomas Ploetz. Ideally, we would have a system that can be trained to recognize activities in a video stream, by using the accompanying human narration, such as a model that recognizes sports events based on the commentary. Right now, I am experimenting with [MMAction2](https://github.com/open-mmlab/mmaction2) and [ActivityNet](http://activity-net.org/index.html).

## Blockboard
_Aug 2021 - Dec 2021_

Blockboard is an interactive visual dashboard that analyzes complex information regarding cryptocurrencies and visualizes it in a simplified manner so that it can be beneficial to general audiences as well as hardcore traders. It collects financial information, on-chain data and sentiment analysis to come up with unique insights that can help you make a more informed and smarter decision regarding your trades. This is a novel platform that combines several different data sources and algorithms for a better understanding of the market.

**Tech stack:** Flask backend with a Javascript frontend (D3.js, Swiper.js) backed by an AzureMySQL database. Sentiment analysis was performed on relevant tweets using Vader.

Here is a brief (_3 min_) video explaining the project with a quick demo:
<p>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/FlJ3E5Omfdg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

## Federated Learning Movie Recommendation System
_Aug 2021 - Dec 2021_

Federated learning is a privacy-by-design machine learning approach where the learning is done by a group of users/nodes who train the algorithm on their own local data. The updated gradients are then encrypted and sent over to the central server which uses it to update its model and then the updated model is sent over to the nodes, who again perform the learning on their own data. This process is repeated a certain number of times until convergence. 

For this project, we simulated Federated Learning on a set of 2000 nodes using the MovieLens dataset. We developed a unique algorithm that uses both user data as well as the movie data to predict ratings that a user might have given to a movie. This was used to train the model by trying to minimize the error in the predictions. For the test set, the algorthm recommended the top N movies based on the ratings it predicted a user to give. This unique approach was developed to ensure we worked within the limitations of federated learning. All the communications with the server were encrypted using gradient pruning.

**Tech stack:** scikit-learn, BERT, Pytorch, Pandas.

## Ageing Prognostics for Engineering Components using ML
_July 2019 – May 2020_

Trained an SVM which learned the conditions for ageing failure in independent parameters of a 2nd-order system. I developed a methodology which used the error response to identify ageing failure in the second-order system. The error response was calculated using the difference between the predicted and actual response. The error response was then used to identify the ageing failure in the second-order system. Built a similarity-based prognostics model using regression analysis on historical data to predict RUL of components.

**Tech stack:** Python, Scikit-learn, Keras, Pandas, Matplotlib.

## Ship Detection using Variational Bayesian Inference
_Aug 2018 - Nov 2018_

Decomposed polarimetric SAR images to separate sea-clutter and establish a probabilistic model of ship detection and then applied variational Bayesian inference to estimate the posterior distributions and obtain the final results.

**Tech stack:** Python, NumPy, Scikit-learn, TensorFlow.