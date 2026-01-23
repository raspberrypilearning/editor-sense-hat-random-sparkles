<h2 class="c-project-heading--task">Light a pixel</h2>
--- task ---

Set a pixel to light red.

--- /task ---

x indicates the horizontal axis, and can have a value between 0 (on the left) and 7 (on the right). 

y indicates the vertical axis, and can have a value between 0 (at the top) and 7 (at the bottom). 

Therefore, the x, y coordinates 0, 0 address the top left-hand LED, and the x, y coordinates 7, 7 address the bottom right-hand LED.

Setting r to 255, with g and b set to 0 means that the pixel will display full red.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5-9
---
from sense_hat import SenseHat

sense = SenseHat()

x = 3
y = 3
r = 255
g = 0
b = 0

sense.set_pixel(x, y, r, g, b)

--- /code ---
</div>

**Run** your code to see the result.

<div class="c-project-output">

![A single red pixel lit on the HAT](images/red_pixel.png)
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

Each pixel can be given value for r, g and b between 0 (fully off) and 255 (fully on).
- r = Red
- g = Green
- b = Blue

</div>
