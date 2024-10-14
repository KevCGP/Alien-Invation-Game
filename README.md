# Alien Invation Game
Purpose of this project was to explore Pygame and use its modules to build a game. Objective of the game is to shoot down alien ships by controlling a rocket ship that can move left and right. After the ships are destroyed, the game resets and the difficulty increases. If the alien ships touches the bottom or the rocket ship, the player loses. Throughout the game, a scoreboard tracks levels and points of the player.


<img width="1187" alt="Screen Shot 2024-10-01 at 4 40 15 PM" src="https://github.com/user-attachments/assets/aa04eed2-26a3-4bd5-adb3-27c5a8597f85">


## Technologies Used
Python, Pygame


## Lessons Learned
From this project, I learned how to manage projects with multiple files. I had to organize the project by refractoring code and managing file contents. One challenging part was ordering the logic of collisions. Once 2 images came into contact, I had to make sure a certain action occurred and then update the scores accordingly. 

```
def _check_bullet_alien_collisions(self):
        """Respond to bullet-allien collisions """
        # Remove any bullets and aliens that have collided
        collisions = pygame.sprite.groupcollide(
                    self.bullets, self.aliens, True,True)
```

Pygame simplifies this process by using the sprite.groupcollide() function. The function can detect collisions by comparing the rects of one element with the rects of another.
