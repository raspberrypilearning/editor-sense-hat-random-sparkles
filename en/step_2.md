<h2 class="c-project-heading--task">Make it random</h2>

Generate numbers to place a random colour at a random location on the Sense HAT display.

<h2 class="c-project-heading--explainer">Follow these instructions</h2>

Import the `random` library.

Define random positions for x and y, to choose which pixel on the Sense HAT will light, then define random colour values for r, g and b.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 2, 6-10
---
from sense_hat import SenseHat
from random import randint

sense = SenseHat()

x = randint(0, 7)
y = randint(0, 7)
r = randint(0, 255)
g = randint(0, 50)
b = randint(0, 255)

sense.set_pixel(x, y, r, g, b)

--- /code ---
</div>

**Run** your code a few times to see the random results.

## Now run your code

Run your code a few times and check that a pixel lights up in a different place and colour.
