# 📡 Morse Code Module  

## 🔍 Overview  
The **Morse Code Module** displays a flashing LED sequence representing a Morse code pattern.  
The player must decode the message and identify the correct letter or word.  
Codes follow the **International Morse Alphabet**, and the module keeps running until the solution is provided.  

---

## 🛠 Hardware Components  
- 💡 **1 LED** (for Morse code signals)  
- 🔘 **1 Push Button** (for user input)  
- 🔔 **1 Buzzer** (optional for audio feedback)  
- 🖥 **Arduino UNO** (or compatible board)  

---

## 🔌 Circuit Connections  
- **LED** → D2 (with a 220Ω resistor)  
- **Button** → D3 (must include a pull-down resistor)  
- **Buzzer (optional)** → D4  
- **GND** & **5V** connections required  

---

## ⚙️ Working Principle  
1️⃣ The LED flashes Morse code representing a **letter or word**:  
   - **Short Blink:** `.` (dot)  
   - **Long Blink:** `-` (dash)  
   - Short pause between symbols  
2️⃣ The player decodes the Morse pattern.  
3️⃣ If correct ✅, a success tone plays. If wrong ❌, an error tone plays and the sequence repeats.  

---

## ⏱ Timing Rules  
- **Dot (.)** → 250ms blink  
- **Dash (-)** → 750ms blink  
- **Gap between dots/dashes:** 250ms  
- **Gap between letters:** 1000ms  

**Example:**  
`.-` = Letter **A**  

---

## 💡 Player Tips  
✔️ Watch the LED carefully and note the timing differences.  
✔️ Keep a Morse code reference nearby for quick decoding.  
✔️ Mistakes will reset the sequence, so stay focused!  

---

## 🚀 Development Ideas  
- Allow the player to **input Morse code via the button**.  
- Add **buzzer sounds** for audible Morse signals.  
- Create **time-limited challenges** for advanced players.  

---

🛠 *This module tests observation skills and memory – perfect for improving decoding abilities!*  


