#  Simon Says Module  

 
**Simon Says** 
Contains 4 spring-loaded push buttons and 1 RGB LED. The player repeats the lit sequence in order. Each correct repetition extends the sequence. The sequence length increases further depending on the difficulty level.



# Electronic Details


## Materials

| **Component**   | **Details**                                | **Link**                                                            | **Quantity** |
|-----------------|--------------------------------------------|--------------------------------------------------------------------|--------------|
| Push Button     | Spring-loaded, colored                      | https://www.elektronikmalzeme.com/12mm-yayli-push-buton-mavi       | 4            |
| RGB LED         | Diffused, 5mm, 1 status LED, others for game | https://www.direnc.net/5mm-rgb-led-ortak-anot-4-pin                | 4            |
| 220Ω Resistor   | Current limiting resistor for LEDs          | https://www.direnc.net/220r-18w-direnc                             | 12           |
| 10KΩ Resistor   | Pull-down resistor for buttons               | https://www.direnc.net/10k-14w-direnc                              | 4            |
| Passive Buzzer  | Passive buzzer to play different tones       | https://www.direnc.net/12mm-aktif-buzzer-5v-12v-devreli            | 1            |

# Gameplay

This module tests rhythm, memory, and attention. The LEDs in the center show you a color sequence. Your task is to remember and press the buttons in the same order. Each correct input adds a new color to the chain; the module asks for a little more each time. But be careful: if you remember even one color incorrectly, the module becomes displeased. Also, waiting too long or hesitating will test its patience. The colors are clear, the rules simple, but even simple things can get complicated under pressure.

## Defusal

Press the green button to start. The LED will show the sequence in different colors. Press the buttons in the correct order according to the sequence. When you finish pressing, a new color will be added to the sequence. You will hear a beep for each color. Colors without beep sounds are not counted in the sequence.

If you wait too long, the module assumes you forgot the sequence and punishes you by restarting it from the beginning. When the status LED turns green, the module is defused and goes silent, but if you keep pressing buttons unnecessarily, you may disturb this peace.
