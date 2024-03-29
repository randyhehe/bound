# bound

![my image](http://i.imgur.com/gZajOFb.png)

This is my UCR CS120B Spring 2016 final project. It is based on a popular game mode in Starcraft, Bound, in which the objective is to get to the dodge patterned explosions to get to the other side. 

On the 8x8 LED matrix, the user is the single green dot and can be moved with the keypad with the arrow keys. Touching a red explosion will "kill" the user, deducting a life or ending the game if no more lives are left. A blue dot represents a wall that the user cannot move onto. When the user gets to the other side of the LED matrix, he/she beats the level and gains a life. The amount of levels and the levels will vary depending on how the user customizes the game.

This game has full level customization for up to 8 levels, with 20 unique patterns for each level. Each pattern has a set duration determining how long it lasts and waits until the next pattern. EEPROM stores all levels, even on poweroff, and brown out detection is enabled to prevent memory glitching with unstable voltages.

Some hardware and technologies that were used:
* 2 ATMEGA1284's communicate via USART
* 8x8 RGB LED Matrix (Red: Explosions, Green: User, Blue: Walls)
* 3 Shift Registers (Daisy chained together to lessen microcontroller ports)
* LCD Display
* Keypad

The project is described in full detail in the following video: https://www.youtube.com/watch?v=6lrzXC5bqX8
