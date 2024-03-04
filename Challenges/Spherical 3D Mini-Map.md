
Specific Theory: [[Linear Algebra#Vector Math|Vector Math]], Line Rendering, [[UI]]
Difficulty: Medium

# The Challenge

You're making a space game, and you want to make a 3D Mini-Map of space around your spaceship. Your goal is to generate a game prefab object for this Mini-Map.

You have your player ship, which can take any rotation and position in 3D Space.
In your game, you have friendly spaceships, and enemy spaceships.

Your Mini-Map should at minimum:

- Have all friendly and enemy ships within a radius be displayed in your Mini-Map
- Friendly and Enemy ships should be graphically distinct 
- A line should be projected from any ship in the Mini-Map to the horizontal plane that the player ship currently exists on
- The user is able to rotate the player's ship on Roll, Yaw, and Pitch axes, as if they were in space, and the map should accurately represent ships and their distance and 3D height to the player based on this orientation
- BONUS: The player is able to move in 3D Space like a spaceship in all directions 
- BONUS: The 3D forward direction of any ship in the Mini-Map should be represented in some way
### Examples

These are just to demonstrate the problem space, feel free to bend the rules and be creative.

![[EliteDangerousMinimap.png]]

![[Homeworld1Minimap.png]]

### Basic Solution

- There exists some player object with some 3D space controls
- Some object representing the Mini-Map exists and has a reference to the Player
- The Mini-Map updates a collection of entities around the player in a certain radius
- The Mini-Map draws and renders 