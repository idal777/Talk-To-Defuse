# 🔀 Switch Module  

## 🔍 Overview  
The **Switch Module** is a mini-game that requires the player to press buttons in a specific sequence.  
It challenges quick reflexes and attention. If a wrong button is pressed, the module triggers an alarm and resets.  

---

## 🔌 Circuit Connections  
- The module uses **4 buttons (switches)**.  
- Each button is connected to Arduino digital pins (e.g., D2, D3, D4, D5).  
- Buttons should be connected with **pull-down resistors**, ensuring the input pin stays **LOW** when not pressed.  
- When pressed, the pin state becomes **HIGH**.  

---

## ⚙️ How It Works  
- Arduino stores a predefined button sequence in memory.  
- The player must press the buttons in this exact order.  
- As the player succeeds, the sequence becomes longer.  
- A wrong press triggers an **error alert** and forces the player to restart.  

---

## 🖥️ Example Circuit Diagram  

**Arduino UNO**  
| | | |
D2 (Button1) D3 (Button2) D4 (Button3) D5 (Button4)
| | | |
Buttons → GND via 10kΩ resistors

## 💡 User Tips  
✅ Press the buttons **quickly and accurately**.  
✅ An **audio alert (buzzer)** may signal an error.  
✅ The game becomes harder as the sequence **increases in length**.  

---

📎 **Related:** [Full Module Documentation](modules-list.md)