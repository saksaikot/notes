## overflow

#### Formal syntax:`[ visible | hidden | clip | scroll | auto ]{1,2}`

```css
div {
  /* for both x and y axis */
  overflow: scroll;
  /* for x axis */
  overflow-x: auto;
  /* for y axis */
  overflow-y: hidden;
  /* shorthand overflow-x overflow-y */
  overflow: auto hidden;
}
```

The default overflow is visible. Thats why if the container is smaller than its children comes out of its container. `overflow-x` for x axis,`overflow-y` for y axis,`shorthand`:`overflow-for-x overflow-for-y;` overflow values-

- `visible`: will visible overflow content,will get mixed with other elements.
- `hidden`:don't show any overflow content
- `scroll`:always show scroll bar
- `auto`:only scrollbar if x axis or y axis have overflow content

Overflow example

<html>

<head>
  <style>
    .main {
      display: flex;
      justify-content: space-around;
    }

    .main>* {
      margin: 1em;
      font-size: 1.2em;
      height: 20rem;
    }

    .paragraph {
      width: 8em;
      height: 5em;
      border: dotted;
    }

    div.visible {
      overflow: visible;
    }

    div.hidden {
      overflow: hidden;
    }

    div.scroll {
      overflow: scroll;
    }

    div.auto {
      overflow: auto;
    }

  </style>
</head>

<body>
  <div class="main">
    <div>
      <code>visible</code>
      <div class="paragraph visible">
        Out of another, I get a lovely view of the bay and a little divrivate wharf belonging to the estate. There is a
        beautiful shaded lane that
        div
      </div>
    </div>
    <div>
      <code>hidden</code>
      <div class="paragraph hidden">
        Out of another, I get a lovely view of the bay and a little private wharf belonging to the estate. There is a
        beautiful shaded lane that
        div
      </div>
    </div>
    <div>
      <code>scroll</code>
      <div class="paragraph scroll">
        Out of another, I get a lovely view of the bay and a little private wharf belonging to the estate. There is
        a
        beautiful shaded lane that
        div
      </div>
    </div>
    <div>
      <code>auto</code>
      <div class="paragraph auto">
        Out of another, I get a lovely view of the bay and a little private wharf belonging to the estate. There
        is a
        beautiful shaded lane that
        div
      </div>
    </div>

</body>

</html>
