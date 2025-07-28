#  Switch Panel Module


Contains 4 toggle switches and 3 LEDs. Depending on the position of each switch, the LEDs change color. If all switches remain in the required position for a while, the module is defused.



---

##  Electronic Details

### Materials

| **Component**   | **Details**                                  | **Link**                                                            | **Qty** |
|-----------------|----------------------------------------------|--------------------------------------------------------------------|---------|
| Toggle Switch   | 3-pin On-Off toggle                           | https://www.direnc.net/kts102-on-off-3-ayak-toggle                 | 4       |
| RGB LED         | Diffused, 5mm. One for status, others for switch feedback | https://www.direnc.net/5mm-rgb-led-ortak-anot-4-pin          | 4       |
| 220Ω Resistor   | Current limiting resistor for LEDs           | https://www.direnc.net/220r-18w-direnc                             | 12      |
| 10KΩ Resistor   | Pull-down resistor for switches               | https://www.direnc.net/10k-14w-direnc                              | 4       |

---

### Component Functions

1. **Status LED:** Shows module status with colors — blue for ready, red blinking for error, green for solved.
2. **Switch LEDs:** Light up in different colors according to the puzzle's progress.
3. **Switches:** Must be set to correct positions as per the solution guide to defuse the module.

*Note:* Only two pins of each switch are connected. Arduino Pro Mini analog pins are used as digital inputs.

---

##  Circuit Diagram

*(Insert circuit diagram image here)*

---

##  Gameplay

This module requires careful attention. You need to set the 4 switches in the correct sequence to achieve specific LED color combinations. Each color change represents progression. Wrong switch positions may reset progress or cause penalties.

### Rules

- Always toggle switches in order.
- Changing multiple switches at once can cause instant failure.
- Repeated mistakes reduce module patience.

---

### Step 1

- **If no LEDs are lit:**
  - Turn ON switches 1 and 2.
    - If first two LEDs turn red, turn OFF switch 1 and proceed to Step 2.
    - If first LED turns blue, turn OFF switch 2 and turn ON switch 4, then proceed to Step 2.

- **If only one LED is lit:**
  - Turn ON switch 2.
    - If all LEDs light, proceed to Step 2.
    - If lit LED changes or another lights, turn OFF switch 2 and turn ON switch 4, then proceed to Step 2.

- **If LED1 and LED2 are blue and LED3 is green:**
  - Turn ON all switches in this order: 1, 3, 4, 2.
    - If LED1 turns red when turning ON switch 3, turn OFF switch 1 and proceed to Step 2.
    - Otherwise, turn OFF all switches in the same order. Failure to do so costs 30% of remaining time but you still proceed to Step 2.

---

### Step 2

- **If any LED is red:**
  - Toggle all switches to the opposite positions.
    - If LED1 blinks, toggle switches 3 and 4.
    - If LED2 blinks, toggle switches 1 and 4.

- **If LED1 is green and LED2 is blue:**
  - Toggle all switches.
    - If LED colors swap, toggle switches 1 and 3.
    - If no change, toggle switches 1 and 2.

- **If no LEDs light:**
  - Toggle all switches.
    - If all LEDs blink, toggle switches 1, 2, and 3.
    - If one LED turns green, toggle switch 4.
    - If one LED turns red, toggle switch 2.

---

> *Tip:* Be patient and precise. Avoid toggling multiple switches simultaneously to prevent failure.
