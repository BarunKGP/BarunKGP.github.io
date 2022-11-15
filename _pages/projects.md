---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## DoGE: Domain Generalization beyond distribution shifts
*Sept 2022 - Present*

Domain generalization algorithms suffer from distribution shifts when faced with different target domains. This is a problem because performance of models degrades in the presence of different kinds of shiftsl. [Ye et al., CVPR 2022](https://arxiv.org/pdf/2106.03721.pdf) found that most state-of-the-art domain generalization (DG) algorithms fail to beat the simple supervised baseline (ERM) on two major kinds of distribution shifts that seem to affect models the most: *correlation shift* and *diversity shift*. Even though certain algorithms outperform ERM on one of the shifts, their average performance across both kinds of shifts is worse than ERM, which makes these models useful only in a highly specialized setting. Ye et al. argues that this means domain generalization performances have been  overstated and actual progress is comparatively low. 

DoGE solves this problem by implementing a novel algorithm that combines gradient muting and a penalty term that punishes the model when its predictions are wrong after a certain number of annealing iterations. We also implemented a scheduling function that controls the influence the penalty and gradient muting functions have at different part of the training stage, depending on whether we are working on a dataset that is more prone to correlation shift or diversity shift. So far, we have managed to beat several benchmarks mentioned in the OOD-Bench paper across both correlation shift and diversity shift, outperforming the previous state-of-the-art models. We are in the process of testing our model on different datasets and expect to get our final results by December 2022.

## Human-assisted Activity Recognition
*Jan 2022 - Present* 

Currently researching ways to improve a video-based activity recognition system by incorporating knowledge from human narration under the supervision of Prof. Thomas Ploetz. Ideally, we would have a system that can be trained to recognize activities in a video stream, by using the accompanying human narration, such as a model that recognizes sports events based on the commentary. Our current approach is to compute the multimodal attention between the narration verbs and nouns and the frame features as a signal for the action boundaries. This is important because we formulate this as a weakly supervised problem and do not use exact action timestamps. This is in line with the [EPIC Kitchens 100](https://epic-kitchens.github.io/2022#challenge-action-recognition) action recognition challenge, which serves as an inspiration for this task. However, we will take this one step further and formulate this problem in a completely semi-supervised setting, where we aim to formulate action boundaries without using any timestamps.

We estimate this project to have publishable results by the end of this year.

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