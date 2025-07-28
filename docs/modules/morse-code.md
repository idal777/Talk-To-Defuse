## Morse Code Module


**Morse Code** 

This module contains a buzzer, an LED, and a button. Messages are transmitted via Morse code using the buzzer and LED. When the correct code is entered in Morse code according to the defusal document, the module is defused.


# Electronic Details

## Materials

| **Component** | **Details**                               | **Link**                                                                 | **Quantity** |
|---------------|-------------------------------------------|-------------------------------------------------------------------------|--------------|
| RGB LED       | Diffused, 5mm, 1 status LED, others for indication | https://www.direnc.net/5mm-rgb-led-ortak-anot-4-pin                     | 3            |
| 220Ω Resistor | Current limiting resistor for LEDs        | https://www.direnc.net/220r-18w-direnc                                  | 12           |
| 10KΩ Resistor | Pull-down resistor for button              | https://www.direnc.net/10k-14w-direnc                                   | 1            |
| Buzzer        | Active buzzer for Morse code sound         | https://www.elektronikmalzeme.com/5-12v-aktif-sesli-buzzer-devreli      | 1            |
| Button        | For entering Morse code                    |                                                                         | 1            |

# Gameplay

Communication in this module is done through beeps. The module sends you a word in Morse code; you decode the word, find the corresponding answer in the document, and send the new word back to the module using Morse code. Each short and long beep represents a correct letter; however, even the slightest rhythm mistake can quickly cause confusion. Waiting too long or rushing can lead to disaster instead of a solution. This module requires clarity—hesitation could be costly.

# Defusal

Press the button once to receive the Morse signal. Listen carefully and decode the code using the document. Then enter the correct code back into the module via Morse code. A new Morse signal will then start; decode it and enter the correct message into the module again. Continue until the module’s status indicator lights green.
