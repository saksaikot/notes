## Box Model

In a normal context, other than grid,`margin` of two element collapse, side by side element share the margin. Margins are calculated from the border and border of other element, not from the margin of other element.
In generale the width is the size of the content, and with padding it becomes more, thats why we see contents are breaking out from its layout, one simple adjustment can solve this problem as in consistency. using `box-sizing:border-box`, it will then calculate the width including padding.

```css
box-sizing: border-box;
*,
::after,
::before {
  box-sizing: border-box;
}
```
