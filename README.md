<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# AI Battleship

Building AI: course project

## Summary

My project focuses on different approaches to playing Battleship (i.e. searching a grid), based on known information and probability calculations. Specifically, I would like to compare different methods utilising these probabilities, and see the effect of different Artifical Neural Network (ANN) applications.

## Background

Battleship, a game with a long history for being a trivial but challenging game, is centred around searching. You use the knowledge you have obtained so far to try and find ships, weighing up the odds (usually cognitively) of where they might be.

This is, generally speaking, a very impractical problem to solve. However, Bayesian Search is the principle of Battleship, and has been used for finding lost sea vessels and can be applied to many real life search and rescue applications.

My interest lies in the different approaches, because by searching the lower probability areas first we may be able to find a target quickly that would've otherwise taken many turns to reveal, or by traditionally searching highest probability locaions we statistically will narrow down targets quickly. I would like to compare the different approaches, and possible applications for artifical neural networks to decide what to do with the input probabilities.

## How is it used?

The solutions explored may provide insight into the different methods used in search and rescue. This solution is a concept and is used in a demonstration / research context, needs include readability and accessibility. This extends requirements to include thorough visualisation and explanation of the data & information.
Uses may also include being used as reference for material such as infographics to explain different search terms and their uses (using Battleship as a demonstration).


Images will make your README look nice!
Once you upload an image to your repository, you can link link to it like this (replace the URL with file path, if you've uploaded an image to Github.)
![Cat](https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg)

If you need to resize images, you have to use an HTML tag, like this:
<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg" width="300">

This is how you create code examples:
```
def main():
   countries = ['Denmark', 'Finland', 'Iceland', 'Norway', 'Sweden']
   pop = [5615000, 5439000, 324000, 5080000, 9609000]   # not actually needed in this exercise...
   fishers = [1891, 2652, 3800, 11611, 1757]

   totPop = sum(pop)
   totFish = sum(fishers)

   # write your solution here

   for i in range(len(countries)):
      print("%s %.2f%%" % (countries[i], 100.0))    # current just prints 100%

main()
```


## Data sources and AI methods
Where does your data come from? Do you collect it yourself or do you use data collected by someone else?
If you need to use links, here's an example:

Test and training data can both be generated randomly using different ship arrangements. Additional data could also be provided by gathering human data however in the context of searching, rather than just winning battleship (against humans) this data wouldn't prove particularly useful.

[Twitter API](https://developer.twitter.com/en/docs)

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

## Applications & Challenges

The applications of this particular search, using large objects and strictly quantised grids that can only be searched one at a time and in any order, is very far removed from real environments. Rather it provides insights into searching in theory, which may have applications down the line.

Challenges include visualisation, where 3-dimensional (grid-row, grid-column, probability) data plus ship locations, hits and misses all have to be visualised. Additionally, in order to compare ships different numerical summaries must be applied, namely turns taken to win (as a distribution), turns to find each ships and/or all ships (as a distribution or as an average) and explaining how these differences occur, and what might be better.

## What next?

How could your project grow and become something even more? What kind of skills, what kind of assistance would you  need to move on? 


## Acknowledgments

* [Playing Battleship with Bayesian Search Theory, Thompson Sampling, and Approximate Bayesian Computation by Austin Richford](https://austinrochford.com/posts/2021-09-02-battleship-bayes.html) / [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
* [A Bayesian Approach to Finding Lost Objects by Katie Howgate](https://www.lancaster.ac.uk/stor-i-student-sites/katie-howgate/2021/02/08/a-bayesian-approach-to-finding-lost-objects/)
