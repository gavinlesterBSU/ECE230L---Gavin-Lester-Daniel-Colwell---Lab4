# ECE230L---Gavin-Lester-Daniel-Colwell---Lab4
github repository to submit lab 4, done on Feb 12, 2026
# Lab 04 - SOP/POS and KMaps

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

First, we learned how to create and collaborate on our own github. We then both joined it and did some basic formatting. We then looked at the given table, and made  a K-map for the naive.v, and filled out the "assign Y" statements in it according to the K-map we made. Using that same K-map, we circled the 0's and 1's how you should, and got the expressions for the SOP and POS respectively. We then put those expressions into Vivado, and ran the simulation. After running it, we ran into errors with our minterm, asit said in the console. We then spent some time going over what we did, and trying to fix it. We did eventually figure out that the minterm was formatted wrong, even though our expression was correct. All test cases passed! We then followed the steps to program it onto the Basys 3 board, and showed the successful demonstration to one of our professors. And then of course, we filled out this readme and ported over our code to this github repository.
:)

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?

When K-maps go across edges, only one value changes, because K-maps are technically an infinite grid, and each time we utilize one, we are just looking very closeley at the set of data that matters to us. So, when they wrap values around edges, it is just like they are just going to the next row or collumn over, not flipped to something completely different.

### Why are the names Sum of Products and Products of Sums?

In K-Maps, "Sum of Products", or SOP, represent expressions where multiple AND terms are OR'd together. In "Product of Sums", or POS, they represent expressions where multiple OR terms that are AND'd together. SOP = 1's and POS = 0's. So, Sum of Products emphasize summing product terms, while Product of Sums multiply sum terms.
### Open the test.v file – how are we able to check that the signals match using XOR?
Using XOR, we can enter the signals, and as long as the XOR gate returns false, we know that the signals match. 
