## Make it random

Generate numbers to place a random colour at a random location on the Sense HAT display.

Import the `random` library.

Define random positions for x and y, to choose which pixel on the Sense HAT will light, then define random colour values for r, g, and b.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="2,6-10"
from sense_hat import SenseHat
from random import randint

sense = SenseHat()

x = randint(0, 7)
y = randint(0, 7)
r = randint(0, 255)
g = randint(0, 50)
b = randint(0, 255)

sense.set_pixel(x, y, r, g, b)

```

## Now run your code

Run your code a few times and check that the pixel that lights up is in a different place and has a different colour each time.
