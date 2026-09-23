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
In this lab, we learned how to turn a truth table into different logic equations using minterms, maxterms, and KMaps. We also learned how KMaps can simplify a logic equation while still giving the same output as the original truth table.
## Lab Questions
### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
The groups can go across the edges because the KMap wraps around. For example, the cell on opposite edges are considered adjacent and can be grouped together to simplify the logic equation.
### Why are the names Sum of Products and Products of Sums?
Because it literally describes what they are
SOP  
(A . B) + (C . D)
In logic gates a product is the result of two ANDs. while a Sum is the result of two ORs. We are getting products (AB) (CD), then looking at the sum of those products
For product of sums its flipped.
POS
(A + B) . (C + D)
We get the sums with (A + B) also (C + D) then the product of all those sums.
### Open the test.v file – how are we able to check that the signals match using XOR?
XOR outputs 0 when two inputs are the same and 1 when they differ. So, led[0] ^ led[1] checks if the signals are matching (each LED is an output and ^ is a XOR gate). If the output isn't 0 it means the outputs differ.
