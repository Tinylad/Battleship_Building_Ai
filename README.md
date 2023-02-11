<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# AI Battleship

Building AI: course project

## Summary

My project focuses on different approaches to playing Battleship (i.e. searching a grid), based on known information and probability calculations. Specifically, I would like to compare different methods utilising these probabilities, and see the effect of different Artifical Neural Network (ANN) applications.

## Background

Battleship, a game with a long history for being a trivial but challenging game, is centred around searching. You use the knowledge you have obtained so far to try and find ships, weighing up the odds (usually cognitively) of where they might be.

This is, generally speaking, a very impractical problem to solve. However, Bayesian Search is the principle of Battleship, and has been used for finding lost sea vessels and can be applied to many real life search and rescue applications.**

My interest lies in the different approaches, because by searching the lower probability areas first we may be able to find a target quickly that would've otherwise taken many turns to reveal, or by traditionally searching highest probability locaions we statistically will narrow down targets quickly. I would like to compare the different approaches, and possible applications for artifical neural networks to decide what to do with the input probabilities.

## How is it used?

The solutions explored may provide insight into the different methods used in search and rescue. This solution is a concept and is used in a demonstration / research context, needs include readability and accessibility. This extends requirements to include thorough visualisation and explanation of the data & information.

## Data sources and AI methods

Test and training data can both be generated randomly using different ship arrangements. Additional data could also be provided by gathering human data however in the context of searching, rather than just winning battleship (against humans) this data wouldn't prove particularly useful.
So far I've tested my approaches on randomly generated ship placements, testing each approach using 1-3 thousand games. Measuring the number of wins, the table and graph below shows how different base approaches compare.


| Method      | Median turns to win |
| ----------- | ----------- |
| Checkerboard x Probability | 47 |
| Probability & Probability hunt  | 54 |
|  Probability & 4dir hunt | 61 |
|  Checkerboard & 4dir hunt| 68 |
|  Random & 4dir hunt | 71 |
|  Random | 97 |

![image](https://user-images.githubusercontent.com/105332964/218243571-1345031e-21ec-485d-acbc-6e4a77c43930.png)

The actual AI methods that could be used to further investigate search methods most likely include Artifical Neural Networks, or an approach that evolves over the course of the game / search.

## Applications & Challenges

The applications of this particular search, using large objects and strictly quantised grids that can only be searched one at a time and in any order, is very far removed from real environments. Rather it provides insights into searching in theory, which may have applications down the line.

Challenges include visualisation, where 3-dimensional (grid-row, grid-column, probability) data plus ship locations, hits and misses all have to be visualised. Additionally, in order to compare ships different numerical summaries must be applied, namely turns taken to win (as a distribution), turns to find each ships and/or all ships (as a distribution or as an average) and explaining how these differences occur, and what might be better.

## What next?

So far I have only tested and investigated the data from the simpler, non-machine-learning approaches. In order to try out these approaches I need a better skill in coding, and understanding of what approaches might work for this context. Spending more time on machine learning and this project in particular I would be able to continue.

## Acknowledgments

* [Playing Battleship with Bayesian Search Theory, Thompson Sampling, and Approximate Bayesian Computation by Austin Richford](https://austinrochford.com/posts/2021-09-02-battleship-bayes.html) / [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
* [A Bayesian Approach to Finding Lost Objects by Katie Howgate](https://www.lancaster.ac.uk/stor-i-student-sites/katie-howgate/2021/02/08/a-bayesian-approach-to-finding-lost-objects/)
