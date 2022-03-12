## pseudo classes

Pseudo classes are special state of an element.

#### Syntax

```css
selector:pseudo-class {
  property: value;
}
```

### User action pseudo classes

- `:hover`: element under mouse pointer
- `:active`: ie: user clicked on the element
- `:focus`:focus with mouse or keyboard

### Input pseudo classes

- `:autofill`: when an input auto filled by browser
- `:enabled`: inputs those are not disabled
- `:disabled`: those are disabled
- `:read-only` or `moz-read-only`: when `readonly` attribute defined
- `:read-write`: when not `readonly`
- `:placeholder-shown` : the state when place holder shown, and typography will not affected.
- `:checked`:matches when checkboxes and radio buttons are toggled
- `:blank`: when user-input containing an empty string or null value.
- `:valid`:ie: email is valid.
- `:invalid`: ie: email is not valid
- `:required`: when required state true.

## Tree structural pseudo class

- `:root`:
- `:empty`:
- `:first-child`:
- `:last-child`:
- `:only-child`:
- `:first-of-type`
- `:last-of-type`:
- `:only-of-type`:

- `:nth-child`:
- `:nth-last-child`:
- `:nth-of-type`:
- `:nth-last-of-type`:
-

<html>
    <head>
    <style>
      .active-state:enabled{
       color:red;
       width:100%;
      }
      .place-holder-shown:placeholder-shown{
          border: 5px solid red;
          width:100%;
      }
      </style>
      </head>
    <body>

  <input class="active-state" type="text"  value="`:enabled` select inputs elements that are not disabled"> 
    <input class="place-holder-shown" type="text"  placeholder="`:placeholder-shown` bold border only when showing placeholder"> 
  </body>
  </html>
  <!-- 
  .class:hover{

}

:focus{ }
:disabled{}
:required{}

// these are based on container or a parent element
:first-child{}
:last-child{}
span:first-child{}// span needs to be first child
:first-of-type{} // select first of that type
:last-of-type{}
:nth-child(2)// select second child
:nth-child(even)
:nth-child(odd)
::nth-child(2n)
:nth-child(2n+1)

:nth-last-child(2)//same as nth-child but in reverse order

:nth-first-of-type,nth-last-of-type

<input disabled required/> -->
