# I.1 Bitboards and simulation

## What is a Bitboard ?

Bitboard is a **method for representing states** in game engine, and particularly in **2D board games**.

It uses the **bit array data structure** and transform all usual searching/testing methods into **binary** and **logical** operations.

![Banner](img/banner.png)

## What is this good for ?

The **strength** of Bitboards are:
1. using only one bit where common data structure use one byte
2. performing high efficiency operations
3. operating on all squares in parallel using bitwise instructions

This data structure is very often used in famous 2D board games like:
* [Chess](https://en.wikipedia.org/wiki/Chess)
* [Reversi](https://en.wikipedia.org/wiki/Reversi)
* [Connect Four](https://en.wikipedia.org/wiki/Connect_Four)
* [The Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)
* Many word games

## Just give me the code !

If you already know why you are here, you can **go to the first section** and see a short example of bitboard application.

Otherwise, you should probably **read the following** about the importance of making a good game engine in Artificial Intelligence (AI) concern.

# A word about simulation (optional)

## Agent and Environment in AI

When creating some artificial intelligence (AI), we have to carry about two things:
* The **environment**: where the agent will act and evolve. it defines the relation between a state, an action of the agent, and the resulting next state.
* The **agent**: anything that can perceive its environment through sensors and acts upon that

![Agent and environment](http://cs-alb-pc3.massey.ac.nz/notes/59302/fig02.01.gif)

> _That's cool ! Why are we talking about that_ ?

The reason is: most of the algorithms need to **predict the future** (make **simulations**) to be efficient.

With bitboards we're not gonna make an agent, but an **efficient perception of the environment** in order to power up our simulation-based algorithms.

## The relative importance of simulations

As said above, an efficient algorithm will sometimes need a high rate of simulations. The rule is:

**The more states we simulate, the more accurate will be our agent**.

> _So, I will learn to make an AI better than the world chess champion ?_

Don't be on a rush ! For two reasons:

##### 1. You should always **improve the algorithm first**

Improving the number of states simulations is very important, **but not as many as improving the algorithm**.

This tutorial will be useful only once you have had an efficient algorithm.

##### 2. Bitboards are **not the response to everything**

Bitboards cannot be implemented without a **lot of condition**, and is sometimes very fastidious to set up.

However, it remains a powerful tool that you should know about !
