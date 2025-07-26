# Cables Module 🧩🔌

## Overview

The Cables Module tests the player’s attention and logical thinking skills.  
The player must identify and either cut or connect the correct cable among multiple cables of different colors and types.  
Cutting or connecting the wrong cable results in an error.

## Components Used

- Multiple cables of different colors and thicknesses (e.g., red, black, yellow)  
- Connection points and connectors  
- Cut button or mechanism (optional)  
- Arduino UNO (or compatible)  
- Buttons (to confirm cable cutting)  
- LEDs (to indicate success or error)  

## Circuit Connections 🔧

| Component            | Arduino Connection       |
|----------------------|-------------------------|
| Cable Cut Button     | D2                      |
| Cable Selection Buttons | D3, D4, D5 (optional)  |
| Success LED          | D9                      |
| Error LED            | D10                     |

> Note: The cutting action is triggered by pressing a button. Correct cable cutting lights up the success LED; wrong cutting activates the error LED and alarm.

## Working Principle ⚙️

1. There are multiple cables on the module.  
2. Arduino pre-selects the correct cable (e.g., the red cable).  
3. The player must find and cut the correct cable by pressing the button.  
4. Correct cable cutting leads to module success and game progression.  
5. Wrong cable cutting causes module error and activates the alarm.

## Tips for Players 🎯

- Pay close attention to cable colors and order.  
- Some modes may provide hints via cable numbers or color codes.  
- Take your time and make logical, careful choices.

## Development Suggestions 🚀

- Increase the number of cables to raise difficulty.  
- Add different button combinations for cutting or connecting cables.  
- Implement time limits or max wrong cuts allowed to increase challenge.

---

🛠️ *This module enhances players’ focus, decision-making, and fine motor skills, making gameplay more engaging and challenging.*
