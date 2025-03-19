---
project_id: Zeppelinator
---

#### Context

When I first started coding, I was advised to start by learning Python, as it was easy to get into. <br />
Very fast, I decided to make a game with a few of my friends, and this is what we made.

As a first project, it did not respect software development best practices. I've therefore refactored the code to be more readable and maintainable. That being said, it still contains many magic numbers that really should be in configuration files. I've also not bothered to fix the fact that the game can only be played on a fixed resolution of 1680 x 1050 pixels.

#### The game

As the player, you control a Zeppelin and must drop bombs on the canons shooting at you. Succesfully destroying all the canons will let you proceed to the next level. Every third level has a boss canon which is stronger and harder to destroy, and levels get progressively harder. Get to level 9 to beat the final boss.

The game ends when the player runs out of health, the goal is to get the highest possible score before that happens.

Use **w-a-s-d** to move and spacebar to drop bombs.

The music is Hell March 2 from Red Alert 2.

![Zeppelinator](/assets/pictures/Zeppelinator-preview.png)

#### Links

- [Play game](https://willthewizard42.itch.io/zeppelinator)
- [Source code](https://github.com/WillTheWizard42/Zeppelinator)
- [Pygame](https://www.pygame.org/docs//)