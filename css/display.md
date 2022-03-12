# display

[details on mdn](https://developer.mozilla.org/en-US/docs/Web/CSS/display#formal_syntax)
[more example on css-trick](https://css-tricks.com/almanac/properties/d/display/)
also in `display` folder with live example
common values:`block/inline/inline-block/none/flex/inline-flex/grid/inline-grid/table/list-item/flow-root/content`

- `block`: margin collapse, if parent and children have same margin then parent and children margin will be same.
- `inline`: will not accept `width` and `height` and no padding/margin top and bottom will apply.
- `inline-block`: will be inline with other element but will accept width and height and top/bottom margin/padding.
- `flex/grid`: will make the direct children flex or grid item respectively.`flex` default direction column.`grid` row.
- `none`: removes from content flow, ignored by the screen reader and solve floating problem
- `content`: `.element { display: contents;}` this will make the children of element to be children of the parent of element. this is use full in case of div wrapper.
