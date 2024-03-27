
Specific Theory: [[Linear Algebra#Vector Math|Vector Math]], [[Linear Algebra]], [[Linear Algebra#Dot Product|Dot Product]], [[Performance Optimization]], [[Computer Graphics]]
Difficulty: Easy

# The Challenge

You got a classic case of asteroids in your game

The challenge is a straightforward test of your math skills.

- Create a generation system that populates your game world with N asteroids, N being a number of your choice. The system can exist in 3D or 2D
- There exist controls for regenerating the system, which clears the simulation space, and regenerates all asteroids. The system begins paused. 
- Each asteroid spawns with a random velocity
- When two asteroids collide, they are deleted from the simulation, but right before, the collision position is recorded and logged
- When you press a "Play" button the simulation occurs and records all asteroid collisions so you can compare your solution to the physical simulation of the game
- Your simulation should play at a reasonable framerate, even for large N. ~30+ FPS.
- **Every time you generate the system, the system precomputes all collisions that will occur, and at what time in the future.**
- BONUS: Add an automatic validation system that verifies that your precomputed collisions and the recorded simulation collisions are approximately the same
