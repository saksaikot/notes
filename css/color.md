## color

The color property sets the color of the text.
Formal syntax - `<rgb()> | <rgba()> | <hsl()> | <hsla()> | <hwb()> | <hex-color> | <named-color>`

- `rgb()`
  - `<percentage>{3} [ / <alpha-value>?]`:`rgb(0% 100% 12% / 45)` or `rgb(0% 100% 12%)`
  - `<number>{3} [ / <alpha-value>?]`
- `rgba()`, **same as rgb**
- `hsl()`: **Hue,saturate,light**
  - `<hue> <percentage> <percentage> [ / <alpha-value> ]?`
  - `<hue>, <percentage>, <percentage>, <alpha-value>?`
- hsla(): **same as hsl()**
- hwb(): **Not supported, specified for css4**,**Hue,Whiteness,Blackness**

Other value:

- `<alpha-value> = <number> | <percentage>`: value 1 is full opacity means no transparent, 0 means full transparent.
- `<hue> = <number> | <angle>`: angle 0 to 360
