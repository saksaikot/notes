## Float and clear

```css
.div3 {
  float: left;
}

.div4 {
  clear: left;
}

float:left; left/right
clear:left;
float: left/right;
clear: left/right/both;
```

syntax:

- `float`:`left|right`
- `clear`:`left|right|both`

`Float` move a content within its containers to most left or to most right and their sibling wrap around them. First float element are positioned most first left or right element,a{float:right;}{b float:right;} then the right position will be b,a.

`Clear` removes wrapping other content otherwise will wrap for float,we can clear left, right or do both.
