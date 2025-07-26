# 🧩 Labyrinth Module

## 📖 Overview

The Labyrinth Module challenges players to navigate through a maze and find the exit.  
It features a **5x5 LED matrix** combined with a joystick or directional buttons for intuitive control.

## 🛠️ Hardware Components

- 5x5 LED Matrix display  
- Joystick or directional buttons  
- Arduino microcontroller board  

## 🔌 Wiring & Connections

- Connect the LED matrix rows and columns to Arduino digital pins.  
- Connect joystick X and Y axes to Arduino analog inputs.  
- If available, connect joystick button to a digital pin.  

## 🎮 Gameplay Mechanics

- Arduino stores the maze layout internally.  
- Players move their character using the joystick or buttons.  
- The goal is to reach the exit point without hitting walls or obstacles.  
- Invalid moves trigger an error state, requiring players to retry.  

## 🔧 Sample Circuit Diagram

Arduino UNO
| | |
LED Matrix Joystick X,Y GND

## 💡 Pro Tips

- Ensure the joystick is properly calibrated for smooth and responsive control.  
- Design the maze layout to be easily changeable for different difficulty levels.  
- Provide clear visual feedback on the LED matrix to help players track their position.  

---

🎯 *This module is excellent for developing spatial reasoning and fine motor skills in a fun and interactive way!* 