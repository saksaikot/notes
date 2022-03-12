## Position

#### Formal syntax: `static | relative | absolute | sticky | fixed`

Values-

- `static`: It is the default value. Component positioned according to normal flow, `top/bottom/left/right/z-index` have no impact.
- `relative`: It create new stacking context except `z-index:auto`. Without `top/bottom/left/right` it acts like position static. With `top/right/left/bottom` it moved from original position. No other element move by this.
- `absolute`:It remove the content from normal flow and no space is given in the document.the top is the nearest positioned ancestor, if there is no ancestor then the containing block ie: the `html. same as relative without `z-index:auto`it creates`stacking context`.margin do not collapse.
- `fixed`:removes from document flow and no space is created. content positioned initial containing block created by viewport. its position calculate by the view port. always create stacking context. **The containing block changes when it ancestor have `transform`,`perspective`,`filter` property**.In printed document element is placed on same position on every page.
- `sticky`:Position is relative to its containing block. does not changes position of other content. always creates stacking context

<html>
<head>
<style>
.container{
  padding:4rem;
  background:red;
  width:10rem;
  margin:3rem 0;
}
.box{
  width:6rem;
  height:6rem;
  background:yellow;
  display:block;
  margin:0 auto;
}
.relative{
position:relative;
top:-5rem;
}
.absolute{
position:absolute;
right:1rem;
}
.fixed{
position:fixed;
bottom:1rem;
}
.sticky{
position:sticky;
top:1rem;
}
.big-height{
  height:300rem
}
</style>

</head>
<body>

<div class="container">
<div class="box relative">
position relative
</div>
</div>

<div class="container">
<div class="box absolute">
Position absolute
</div>
</div>

<div class="container">
<div class="box fixed">
Position fixed
</div>
</div>
<div class="container big-height">
<div class="box sticky">
position sticky
</div>
</div>
</body>
</html>
