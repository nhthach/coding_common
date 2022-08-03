
### How to use it

Call this code

Html structure

```html

<section>
  <h3><label><input type="checkbox" /> Parent 1</label></h3>
  <div class="children">
    <label><input type="checkbox" /> Child 1-1</label> &nbsp; &nbsp;
    <label><input type="checkbox" /> Child 1-2</label> &nbsp; &nbsp;
    <label><input type="checkbox" /> Child 1-3</label>
  </div>
</section>
<section>
  <h3><label><input type="checkbox" /> Parent 2</label></h3>
  <div class="children">
    <label><input type="checkbox" checked="checked" /> Child 2-1</label> &nbsp; &nbsp;
    <label><input type="checkbox" checked="checked" /> Child 2-2</label> &nbsp; &nbsp;
    <label><input type="checkbox" checked="checked" /> Child 2-3</label>
  </div>
</section>

```

jQuery

```js

$(".parent-checkbox input:checkbox").cbFamily(function (){
  return $(this).parents(".parent-checkbox").next().find("input:checkbox");
});

``