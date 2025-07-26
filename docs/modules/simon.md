# 🎮 Simon Says Module  

## 🔍 Overview  
**Simon Says** is a classic memory game based on colors and sounds.  
The player must repeat the sequence of colors shown by the LEDs.  
With every successful attempt, the sequence grows longer, and the difficulty increases.  

---

## 🛠 Hardware Components  
- 🔲 **5x5 LED Matrix** (25 LEDs)  
- 🔔 **Buzzer** for sound feedback  
- 🔴🟢🔵🟡 **4 Colored Buttons** (Red, Green, Blue, Yellow)  
- 🖥 **Arduino UNO** or compatible board  

---

## 🔌 Connections  
- The **LED matrix** is connected to Arduino’s digital pins (e.g., 8, 9, 10...).  
- Buttons and buzzer are connected to their respective pins.  
- Buttons must use **pull-down resistors** to ensure proper signal.  
- The **buzzer** is connected to a **PWM pin** for tone control.  

---

## ⚙️ Game Logic  
1️⃣ Arduino generates a random color sequence.  
2️⃣ The LED matrix lights up to display the color pattern.  
3️⃣ The player repeats the pattern by pressing the colored buttons.  
4️⃣ If correct ✅, the sequence adds **one more color** and repeats.  
5️⃣ If wrong ❌, the game resets to the beginning.  

---

## 🖥 Example Circuit Layout  
Arduino UNO
| | |
LED Matrix → Digital Pins
Buttons → Digital Pins
Buzzer → PWM Pin
GND → Common Ground

## 💡 Tips for Success  
✔️ Make sure the LED matrix is properly wired and driven.  
✔️ Verify buttons provide **clean signals** (debouncing if necessary).  
✔️ Audio feedback helps players understand errors or success.  

---

📎 **Related:** [Full Module Documentation](modules-list.md)


