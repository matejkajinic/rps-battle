# Rock Paper Scissors Battle Simulation

Created by: Claude 3.5 Sonnet (Anthropic AI)
Date: August 1, 2024

## Description

This project is an interactive, visual simulation of a Rock Paper Scissors battle using HTML5 Canvas. Multiple rock, paper, and scissors symbols float around in a confined space, colliding and competing based on the classic game rules until only one symbol remains as the winner.

## Features

- Dark-themed background for better visibility
- Compact 400x400 pixel arena
- 50 initial battlers (rock, paper, scissors symbols)
- Dynamic movement and collision detection
- Automatic battles upon collision
- Winner declaration at the end of the simulation

## Technical Details

### HTML Structure
The HTML file consists of:
- A `<canvas>` element for rendering the simulation
- A control div containing a "Start Simulation" button and a winner display span

### CSS Styling
- Dark background (#1a1a1a) for the body and canvas
- Styled button for starting the simulation
- Positioned controls for easy access

### JavaScript Functionality

#### Battler Class
Represents each rock, paper, or scissors symbol:
- Properties: choice, position (x, y), velocity (dx, dy), size
- Methods: draw(), move(), collidesWith()

#### Main Functions
- `startSimulation()`: Initializes 50 battlers and starts the animation
- `animate()`: Main game loop, handles movement, collisions, and battles
- `battle()`: Determines the winner between two colliding battlers

## How to Use

1. Save the HTML file to your local machine.
2. Open the file in a modern web browser (Chrome, Firefox, Safari, or Edge).
3. Click the "Start Simulation" button to begin the battle.
4. Watch as the symbols move, collide, and eliminate each other.
5. The simulation ends when only one symbol remains, which is declared the winner.

## Customization

You can easily modify the following aspects of the simulation:
- Canvas size: Adjust `canvas.width` and `canvas.height`
- Number of battlers: Change the number in `Array(50).fill()`
- Symbol size: Modify the `size` property in the `Battler` class
- Movement speed: Adjust the multiplier in `this.dx` and `this.dy` initialization

## Browser Compatibility

This simulation uses HTML5 Canvas and modern JavaScript features. It should work in all up-to-date versions of major browsers. For the best experience, use the latest version of Chrome, Firefox, Safari, or Edge.

## License

This project is open-source and free to use, modify, and distribute. Please provide attribution to Claude 3.5 Sonnet (Anthropic AI) if you use or adapt this code.

## Acknowledgments

Special thanks to the classic game of Rock Paper Scissors for inspiring this simulation.