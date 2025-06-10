# 🐍 TypeScript Snake Game

A classic Snake game built with React and TypeScript using HTML5 Canvas.

## Features

- **Classic Gameplay**: Navigate the snake to eat apples and grow longer
- **Score System**: Track current score and high score with local storage
- **Collision Detection**: Game ends when hitting walls or the snake's own body
- **Responsive Controls**: Use arrow keys to control the snake direction
- **Retro Design**: Styled with a vintage monitor frame

## Tech Stack

- **React**: UI framework
- **TypeScript**: Type safety and better development experience
- **HTML5 Canvas**: Game rendering
- **CSS**: Styling and animations

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation & Running

```bash
# Clone the repository
git clone <repository-url>
cd ts-snakegame

# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build

# Run tests
npm test
```

The game will open at `http://localhost:3000`

## How to Play

1. Click the **Play** button to start
2. Use **Arrow Keys** to control the snake:
   - ↑ Arrow Up: Move up
   - ↓ Arrow Down: Move down
   - ← Arrow Left: Move left
   - → Arrow Right: Move right
3. Eat apples to increase your score and grow the snake
4. Avoid hitting the walls or the snake's own body
5. Try to beat your high score!

## Game Mechanics

- **Snake Movement**: The snake moves continuously in the current direction
- **Food Generation**: Apples appear randomly on the grid after being eaten
- **Scoring**: Each apple eaten increases the score by 1
- **High Score**: Best score is automatically saved to browser local storage
- **Game Over**: Occurs when the snake hits a wall or itself

## Project Structure

```
src/
├── App.tsx              # Main game component
├── App.css              # Game styling
├── UseInterval.ts       # Custom hook for game loop
├── applePixels.png      # Apple sprite image
└── oldMonitor.png       # Monitor frame image
```

## Key Implementation Details

- **Game Loop**: Uses `useInterval` custom hook with `requestAnimationFrame`
- **State Management**: React hooks for snake position, apple location, and game state
- **Collision Detection**: Checks boundary and self-collision on each frame
- **Canvas Rendering**: Direct pixel manipulation for smooth gameplay

---

*A simple implementation of the classic Snake game for learning React, TypeScript, and Canvas API.*
