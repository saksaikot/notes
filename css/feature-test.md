## @support

We can check if a specific feature is available in the browser, if not we can give a fallback css.The revert property of background color is available in firefox but not in chrome,so we can check like this

```css
@supports (background-color: revert) {
  .div {
    background-color: revert;
  }
}

/* or like this as fallback  */
@supports not (background-color: revert) {
  .div {
    background-color: transparent;
  }
}
```

We can also check with 'and' and 'or'
