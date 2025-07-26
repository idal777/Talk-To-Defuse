# 🤲 Hand Skill Module

## 🧩 Module Overview

This module tests the player’s physical hand skills and attention.  
The player must carefully guide a metal ring along an inclined spiral wire without touching it.  
Contact between the ring and the wire triggers an error and activates alerts.  
This task requires precision, focus, and hand-eye coordination.

## ⚙️ Components Used

- 1x Spiral-shaped rigid conductive wire (e.g., aluminum or copper)  
- 1x Metal ring (held by the player)  
- 1x Buzzer (for contact alert)  
- 1x LED (optional, for visual warning)  
- Arduino UNO (or compatible board)  
- 10K Ohm resistor (pull-down)  
- Jumper wires  
- Breadboard (or soldered circuit)  

## 🔌 Circuit Connections

| Component       | Arduino Connection      |
|-----------------|-------------------------|
| Spiral Wire     | GND                     |
| Metal Ring      | D2 (digital input pin)  |
| Buzzer          | D9                      |
| LED (optional)  | D10                     |

*Note:* When the metal ring touches the spiral wire, pin D2 receives a LOW signal, which is detected as an error.

## 🎮 Gameplay Mechanics

- The player starts at one end and guides the ring along the spiral wire.  
- Contact triggers the buzzer and LED alerts.  
- There may be 3 allowed contacts or the contact time may be measured to score performance.

## 🛠️ Difficulty Adjustment

- Increasing the wire’s slope and length raises the difficulty level.  
- Narrower passages or time limits add further challenge.

## 📷 Visual Reference

*3D model or real-life photo can be inserted here.*

---

🎯 *Great for improving fine motor skills and concentration in an engaging, hands-on way!*

