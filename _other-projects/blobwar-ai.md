---
project_id: Blobwar-AI
---
	
#### Context

This was a project I made with a classmate in my last year of engineering school. The goal was to learn about making efficient algorithms and multithreading, Rust is a great language for multithreading so that is what was used.

The task was to implement a basic alpha-beta pruning search algorithm that played blobwar, and then make as many optimizations as we wanted. At the end of the project, every student team made their algorithm play in a tournament against each other. Algorithms had a maximum of one second to think of a move, and our algorithm won the tournament!

Blobwar is a game I am currently remaking in Unity and the rules are explained [here](/solo-games/blobwar-game).

In this picture we can see an example of a human playing against the algorithm.

![Blobwar AI](/assets/pictures/Blobwar-ai-example.png)

Optimizations we implemented included pruning the 25% worst moves on the first level of the search, making the first level of the search parallel, sorting the moves on the first level and exploring the best ones first, and hashing each position we explore in order to not evaluate an identical position multiple times.

#### Links

- [Source code](https://github.com/WillTheWizard42/blobwar-ai)
- [Alpha-beta pruning](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning)