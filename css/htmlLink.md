# link tag

`link` is external resource link element, can be same domain or other domain.
more on
[link mdn](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link)
[Preload mdn](https://developer.mozilla.org/en-US/docs/Web/HTML/Link_types/preload)

```html
<!-- include stylesheets -->
<link href="main.css" rel="stylesheet" />

<!-- declare favicon -->
<link rel="icon" href="favicon.ico" />
<!-- declare other device icon, here rel is the relation and the purpose of the icon -->
<link
  rel="apple-touch-icon-precomposed"
  sizes="144x144"
  href="favicon144.png"
  type="image/png"
/>

<link
  rel="preload"
  href="myFont.woff2"
  as="font"
  type="font/woff2"
  crossorigin="anonymous"
/>
```

Attributes-

- `rel`

  - `preload`:

        ```html
        <link
          rel="preload"
          href="bg-image-narrow.png"
          as="image"
          media="(max-width: 600px)"
        />
        <link rel="preload" href="style.css" as="style" />
        <link rel="preload" href="main.js" as="script" />
        <link rel="preload" href="sintel-short.mp4" as="video" type="video/mp4" />
        <link
          rel="preload"
          href="fonts/cicle_fina-webfont.woff2"
          as="font"
          type="font/woff2"
          crossorigin
        />
        ```

    rel:preload,as possible values-

- `audio`: Audio file, as typically used in <audio>.
- `document`: An HTML document intended to be embedded by a `<frame>` or `<iframe>`.
- `embed`: A resource to be embedded inside an `<embed>` element.
- `fetch`: Resource to be accessed by a fetch or XHR request, such as an ArrayBuffer or JSON file.
- `font`: Font file.
- `image`: Image file.
- `object`: A resource to be embedded inside an `<object>` element.
- `script`: JavaScript file.
- `style`: CSS stylesheet.
- `track`: WebVTT file.
- `worker`: A JavaScript web worker or shared worker.
- `video`: Video file, as typically used in `<video>`.
