# Pong Game Information

## Overview
A classic Pong game built with HTML5, CSS3, and vanilla JavaScript. The player controls the left paddle while competing against a computer AI opponent on the right side.

## Game Features

### Player Controls
- **Mouse Control:** Move your mouse up and down to control the left paddle
- **Keyboard Control:** Use arrow keys (⬆️⬇️) to control the left paddle
- **Start/Pause:** Press SPACE to start or pause the game

### Computer AI
- Right paddle controlled by intelligent AI that tracks the ball
- AI has built-in reaction delay for balanced difficulty
- Computer adjusts paddle position based on ball trajectory

### Ball Physics
- **Wall Collisions:** Ball bounces off top and bottom walls
- **Paddle Collisions:** Full collision detection with both paddles
- **Speed Mechanics:** Ball speed increases with each paddle hit (up to maximum speed)
- **Spin System:** Ball trajectory changes based on where it hits the paddle
- **Ball Reset:** Ball returns to center after each score

### Scoring System
- **Player Score:** Increases when computer fails to hit the ball (ball goes past left)
- **Computer Score:** Increases when player fails to hit the ball (ball goes past right)
- **Real-time Display:** Score updates instantly on the scoreboard

### Visual Design
- **Modern UI:** Gradient background with purple and blue tones
- **Neon Effects:** Glowing paddles (green) and ball (magenta)
- **Canvas Graphics:** 800x400 pixel game canvas with dark blue gradient
- **Center Line:** Dashed line dividing the court
- **Responsive Layout:** Centered container with shadow effects
- **Status Display:** Real-time game status messages

## Game Mechanics

### Paddle Movement
- Paddles confined within canvas boundaries
- Smooth movement with collision detection against walls
- Player paddle: Speed of 6 units per frame
- Computer paddle: Speed of 4.5 units per frame

### Ball Behavior
- Initial velocity: 5 units per frame in random direction
- Maximum speed: 8 units per frame
- Ball size: 8 pixels radius
- Speed increase per paddle hit: 5% (1.05x multiplier)
- Spin effect: Up to ±3 units based on paddle hit position

### AI Difficulty
- AI has a 35-pixel reaction zone (doesn't react to balls beyond this range)
- This creates challenging but winnable gameplay
- Ball tracking is predictive, not perfect

## Files Included

### index.html
- HTML5 structure
- Game canvas element
- Score display
- Control instructions
- Game status indicator
- Script imports

### style.css
- Modern CSS styling
- Gradient backgrounds
- Flexbox layout
- Responsive design
- Neon glow effects
- Professional UI components

### script.js
- Complete game logic
- Physics engine
- Collision detection
- AI algorithms
- Event listeners
- Game loop using requestAnimationFrame

## How to Play

1. Open `index.html` in a web browser
2. Press **SPACE** to start the game
3. Control your paddle (left side) using:
   - Mouse movement (up/down)
   - Arrow keys (⬆️⬇️)
4. Hit the ball toward the computer to score
5. The game continues until you decide to pause
6. Press **SPACE** again to pause/resume

## Game Rules

- Each paddle can only be moved vertically
- The ball bounces off walls automatically
- A point is scored when the opponent fails to return the ball
- The ball increases speed with each paddle hit
- The game can be paused at any time by pressing SPACE

## Technical Details

### Technologies Used
- **HTML5:** Canvas API for graphics rendering
- **CSS3:** Gradients, flexbox, animations
- **JavaScript (ES6):** Game logic, physics, AI

### Browser Compatibility
- Modern browsers with HTML5 Canvas support
- Tested on Chrome, Firefox, Safari, Edge

### Performance
- Uses `requestAnimationFrame` for smooth 60 FPS gameplay
- Optimized collision detection algorithms
- Minimal DOM manipulation

## Customization Options

You can easily modify these values in `script.js`:
- `paddleWidth` - Size of paddles
- `paddleHeight` - Height of paddles
- `ballSize` - Ball radius
- `playerPaddle.speed` - Player paddle movement speed
- `computerPaddle.speed` - Computer paddle movement speed
- `ball.maxSpeed` - Maximum ball velocity
- Canvas dimensions (width and height in HTML)

## Future Enhancement Ideas

- Sound effects (paddle hit, score, wall bounce)
- Difficulty levels (Easy, Medium, Hard)
- Multiplayer mode (two players)
- Ball trail animation
- Paddle rotation on spin
- Power-ups and obstacles
- High score persistence
- Mobile touch controls
- Game statistics and analytics
