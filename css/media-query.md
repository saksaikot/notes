## @media queries

```css
/* @media media-type */
/* media-type:print/screen/all */

@media print {
  div {
    color: red;
  }
}

/* using and condition */

@media screen and (max-width: 700px) {
}

/* or */
@media all and (max-width: 700px) {
}

/* this is same as above */
/* for all media and width is 700px or below 700px */

@media (max-width: 700px) {
}
```

best use first style for mobile device and then add style for larger devices

```css
div {
  display: flex;
  flex-direction: row;
}

@media (min-width: 40rem) {
  flex-direction: column;
}
```

<html>
<head>
<style>
div {
  display: flex;
  flex-direction: row;
  gap:1rem;
}

@media (min-width: 40rem) {
flex-direction: column;
}
</style>

</head>
<body>
<div>
  
  <p>This is paragraph one</p>
  <p>This is paragraph two</p>
  <p>This is paragraph three</p>
</div>
</body>
</html>
