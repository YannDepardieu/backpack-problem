# Backpack Problem

<https://brilliant.org/wiki/backpack-problem/>

The backpack problem (also known as the "Knapsack problem") is a widely known combinatorial optimization problem in computer science. In this wiki, you will learn how to solve the knapsack problem using dynamic programming.

## Introduction

The backpack problem can be stated as follows:

Given a set of different items, each one with an associated value and weight, determine which items you should pick in order to maximize the value of the items without surpassing the capacity of your backpack.

Concretely, imagine we have the following set of valued items and the given backpack.

Suppose you have a set of 5 items:

|         | First Item | Second Item | Third Item | Fourth Item | Fifth Item |
|---------|------------|-------------|------------|-------------|------------|
| Value:  | $5         | $10         | $3         | $2          | $3         |
| Weight: | 4 kg       | 8 kg        | 3 kg       | 5 kg        | 2 kg       |
|         |            |             |            |             |            |

If your backpack's weight limit is 10 kg, what is the optimal solution? That is, which items should you take with you?

In this case, the solution is clear. One would take the second and the last items, obtaining a value of $13 while meeting the weight limit exactly. We achieve the maximum possible value without violating the problem's constraint.
​
However, evaluating all possibilities is very unpractical in general, so we would like to know if there is a better way to approach this problem. In fact, there is, and we will see an algorithm in the next section.
