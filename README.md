{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Conditional Probability - Lab"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Introduction\n",
    "\n",
    "In order to be ready for real world applications of probability, it is important to understand what happens when probabilities are not independent. Very often, the probability of a certain event depends on other events happening! Let's see how this all works in this lab.\n",
    "\n",
    "## Objectives"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "You will be able to:\n",
    "\n",
    "- Understand and Explain the conditional probability - P(A∩B) = P(A|B) x P(B)\n",
    "- Use the multiplication rule to find the probability of the intersection of two events\n",
    "- Apply the techniques learned in the lesson to simple problems\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 1\n",
    "A coin is tossed and a single 6-sided die is rolled. Find the probability of landing on the head side of the coin and rolling a 3 on the die."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.08333333333333333"
      ]
     },
     "execution_count": 1,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution\n",
    "0.5 * 1./6"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 2\n",
    "A school survey found that 9 out of 10 students like pizza. If three students are chosen at random **with replacement**, what is the probability that all three students like pizza?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.7290000000000001"
      ]
     },
     "execution_count": 2,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your Solution\n",
    ".9**3"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 3\n",
    "70% of your friends like Chocolate flavored ice cream , and 35% like Chocolate AND like Strawberry flavors.\n",
    "\n",
    "What percent of those who like Chocolate also like Strawberry?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.5"
      ]
     },
     "execution_count": 3,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution \n",
    "0.50"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "50% of your friends who like Chocolate also like Strawberry"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 4\n",
    "What is the probability of drawing 2 consecutive Aces from a Deck of cards. "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.004524886877828055"
      ]
     },
     "execution_count": 4,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution\n",
    "4/52 * 3/51"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 5\n",
    "In a manufacturing factory that produces a certain product, there are 100 units of the product, 5 of which are defective. We pick three units from the 100 units at random. \n",
    "\n",
    "What is the probability that none of them are defective?\n",
    "Hint: Use chain rule"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.8559987631416202"
      ]
     },
     "execution_count": 5,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution\n",
    "95/100 * 94/99 * 93/98"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 6"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Let's consider the example where 2 dice are thrown. Given that **at least one** of the dice has come up on a number higher than 4, what is the probability that the sum is 8?\n",
    "\n",
    "Let i,j be the numbers shown on the dice . Denote events as below:\n",
    "\n",
    "* **Event A is when Either i Or j is 5 or 6** (Keep an eye on either - or)\n",
    "* **Event B is when i + j = 8**\n",
    "\n",
    "\n",
    "* What is the size of sample space Ω ?\n",
    "* What is P(A ∩ B) ?\n",
    "* What is P(A) ?\n",
    "* Use above to calculate P(B|A) ."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.16666666666666666"
      ]
     },
     "execution_count": 8,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "(4/36)/(24/36) "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.16666666666666666"
      ]
     },
     "execution_count": 6,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution\n",
    "# question?"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Exercise 7\n",
    "\n",
    "Let's consider a credit card example. At a supermarket, we randomly select customers and make notes of whether a given customer owns a Visa card (event A) or an Amex credit card (event B). Some customers own both cards.\n",
    "You can assume that:\n",
    "\n",
    "- P(A) = 0.5\n",
    "- P(B) = 0.4\n",
    "- both A and B = 0.25.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "With the knowledge we have about conditional probabilities, compute and interpret the following probabilities:\n",
    "\n",
    "- $P(B \\mid A)$\n",
    "- $P(B'\\mid A)$\n",
    "- $P(A\\mid B)$\n",
    "- $P(A'\\mid B)$\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "0.5"
      ]
     },
     "execution_count": 10,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "# Your solution\n",
    "p_B_given_A = 0.25/0.5  \n",
    "p_B_given_A # correct answer: 0.5\n",
    "\n",
    "p_Bcomp_given_A = 1 - 0.5\n",
    "p_Bcomp_given_A # correct answer: 0.5"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Summary \n",
    "\n",
    "In this lab we practiced around conditional probability and its theorem with some simple problems. The key takeaway from this lab is to to be able to identify random events as dependent or independent and calculating the probability of their occurrence using appropriate methods. Next we'll start focusing on the some more conditional probability axioms, building on the knowledge we have thus far. "
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.6.5"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
