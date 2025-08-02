# Pong Game

A classic Pong arcade game implementation built with Python's Turtle graphics library. Two players control paddles to bounce a ball back and forth, scoring points when the opponent misses.

## Features

- **Two-Player Gameplay**: Local multiplayer for two players
- **Real-time Score Tracking**: Live scoreboard displaying both players' scores
- **Collision Detection**: Ball bounces off paddles and walls realistically
- **Classic Gameplay**: Faithful recreation of the original Pong mechanics
- **Smooth Movement**: Fluid paddle controls and ball physics
- **Game Reset**: Ball automatically resets to center after each point
- **Responsive Controls**: Separate controls for each player

## Game Rules

- **Left Player**: Use `W` (up) and `S` (down) keys to control the left paddle
- **Right Player**: Use `Arrow Up` and `Arrow Down` keys to control the right paddle
- **Scoring**: Player scores when the ball passes the opponent's paddle
- **Winning**: First player to reach the target score wins (continuous play)

## Requirements

- Python 3.x
- turtle (built-in Python module)

## Project Structure

```
pong-game/
│
├── main.py          # Main game loop and collision detection
├── paddle.py        # Paddle class with movement controls
├── ball.py          # Ball class with physics and bouncing
└── scoreboard.py    # Score tracking and display system
```

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/pong-game.git
```

2. Navigate to the project directory:
```bash
cd pong-game
```

3. Make sure you have all required files:
   - `main.py` (main game file)
   - `paddle.py` (paddle logic)
   - `ball.py` (ball physics)
   - `scoreboard.py` (score management)

## Usage

Run the main game file:
```bash
python main.py
```

### Controls

**Left Player (Left Paddle):**
- **W Key**: Move paddle up
- **S Key**: Move paddle down

**Right Player (Right Paddle):**
- **↑ Arrow Key**: Move paddle up
- **↓ Arrow Key**: Move paddle down

**Game Control:**
- **Click anywhere**: Exit game

## Game Specifications

- **Screen Size**: 800x600 pixels
- **Background**: Black
- **Paddle Positions**: Left at x=-350, Right at x=350
- **Ball Speed**: Updates every 0.1 seconds
- **Wall Collision**: Ball bounces at y=±285
- **Paddle Collision**: Detected within 50 pixels distance
- **Scoring Zones**: Ball passes x=±380 coordinates

## Gameplay Mechanics

1. **Ball Movement**: Continuous diagonal movement across the screen
2. **Wall Bouncing**: Ball reverses Y-direction when hitting top/bottom walls
3. **Paddle Bouncing**: Ball reverses X-direction when hitting paddles
4. **Scoring System**: Points awarded when ball passes opponent's paddle
5. **Ball Reset**: Returns to center after each point with random direction

## Physics Implementation

- **Collision Detection**: Distance-based collision between ball and paddles
- **Bounce Mechanics**: Separate X and Y axis bouncing for realistic physics
- **Speed Control**: Consistent game speed with time.sleep() regulation
- **Boundary Detection**: Precise wall and scoring zone detection
- 
## Code Structure

### Main Components

- **main.py**: Game loop, collision detection, and event handling
- **paddle.py**: Paddle class with up/down movement methods
- **ball.py**: Ball physics including movement and bouncing logic
- **scoreboard.py**: Score display and point tracking system

### Key Features

- Object-oriented design with separate classes
- Event-driven input handling
- Real-time collision detection
- Automatic game state management

## Future Enhancements

- [ ] AI opponent for single-player mode
- [ ] Sound effects for paddle hits and scoring
- [ ] Particle effects for ball collisions
- [ ] Difficulty levels with varying ball speeds
- [ ] Win condition with game over screen
- [ ] Paddle size customization
- [ ] Tournament mode with multiple rounds
- [ ] High score persistence
- [ ] Custom color themes

## Contributing

Feel free to fork this project and submit pull requests for improvements or new features.

## Acknowledgments

Inspired by the original Pong arcade game from 1972. Built as part of learning Python game development with Turtle graphics.
