#  Main Module

The **Main Module** is the central control unit of the *Talk to Defuse* modular bomb defusal game. It manages communication with all modules, oversees game flow, user interaction, and timing mechanics. From boot-up to victory or failure, the main module ensures everything runs in sync.

---
## Circuit Diagram


##  Features

- **Status Indicator:** 3 RGB LEDs that change color depending on game state.
- **Lives Display:** 3 red LEDs indicate player lives. Each mistake turns one off.
- **Power Switch:** Main on/off switch for the system.
- **Countdown Timer:** Displays remaining time using a 4-digit 7-segment display.
- **LCD Screen:** Displays user interface elements like difficulty selection and serial number.
- **Control Button:** Used to navigate options and start/stop the game.

---

##  Components

| **Component**      | **Description**                                      | **Link**                                                                                      | **Qty** |
|--------------------|------------------------------------------------------|-----------------------------------------------------------------------------------------------|--------|
| Red LED            | Dome type, 5mm                                       | [direnc.net](https://www.direnc.net/5mm-led-kirmizi)                                          | 3      |
| RGB LED            | Common Anode, 5mm                                    | [direnc.net](https://www.direnc.net/5mm-rgb-led-ortak-anot-4-pin)                             | 3      |
| 2x16 LCD Display   | Blue background, elegant UI                          | [direnc.net](https://www.direnc.net/2x16-lcd-display-sol-ust-mavi-qapass)                     | 1      |
| Push Button        | Spring-based, non-latching                           | [direnc.net](https://www.direnc.net/dc180-isikli-yayli-buton)                                 | 1      |
| TM1637 Clock Module| Easy-to-use 4-digit display                          | [direnc.net](https://www.direnc.net/4-digit-led-display-saat-modul-tm1637-kirmizi)            | 1      |
| Buzzer             | Active, includes internal driver                     | [direnc.net](https://www.direnc.net/12mm-aktif-buzzer-5v-12v-devreli)                         | 1      |
| 220Ω Resistor      | Limits current to LEDs                               | [direnc.net](https://www.direnc.net/220r-18w-direnc)                                          | 6      |
| 10KΩ Resistor      | Used as pull-down for the button                     | [direnc.net](https://www.direnc.net/10k-14w-direnc)                                           | 1      |
| On-Off Switch      | Round, illuminated power switch                      | [direnc.net](https://www.direnc.net/dc131a-3p-on-off-anahtar-12v-isikli-yuvarlak-20mm)        | 1      |

---

##  Software Architecture

- Language: **Arduino C++**
- Structure: Central file is `main.ino`
- Communication: **I2C**, where the Main Module is the **Master**, and other game modules are **Slaves**

### Main Responsibilities

- Game start, reset, and difficulty selection
- Countdown management based on total module requirements
- Displaying the serial number and game info on the LCD
- Monitoring module completion states
- Handling lives and time acceleration upon mistakes

### I2C Communication Protocol

- **Protocol:** I2C
- **Master:** Main Module
- **Slaves:** Puzzle Modules (e.g., Switch, Simon, Wire, etc.)
- **Addresses:** Each module has a unique I2C address

#### Command Signals

- `RESP_START_ERR`: Checks whether modules are in their initial state  
- `RESP_SOLVED`: Indicates a module has been solved  
- `RESP_MISTAKE`: Indicates a mistake occurred  
- `RESP_ERROR`: General error state

---

## ⏱ Time Management

- Time is tracked using Arduino’s `millis()` function
- Remaining time is displayed on TM1637
- Each mistake speeds up the countdown by 10%
- When timer reaches 0, the game ends

---

##  Game Flow

1. System powers on and the LCD shows startup screen.
2. Main Module checks if all modules are in their initial states.
3. Player selects a difficulty level using the button.
4. Holding the button starts the countdown and begins the game.
5. The game monitors each module's status via I2C.
6. Mistakes reduce lives and accelerate time.
7. If all modules report “solved”, the game is won.
8. If time runs out or all lives are lost, the game is lost.

---

##  Game States

### 1. Initialization

- Game waits until all modules report they are in a valid starting state (e.g., switches OFF).
- If any module sends `RESP_START_ERR`, the system remains in this state.

### 2. Pre-Game

- Player chooses a difficulty level:
  - **Easy:** Long timer, 3 lives  
  - **Hard:** Shorter timer, 3 lives  
  - **Expert:** No timer visible, no lives

### 3. Gameplay

- Timer begins  
- Monitors `RESP_MISTAKE` and `RESP_SOLVED` from modules  
- On completion, returns to Initialization mode  
- Holding the button during the game resets to Initialization

---

##  Expandability

- New modules can be added by assigning a new I2C address and handling logic
- Each module contains its own solution algorithm
- The main module only evaluates the result

---

