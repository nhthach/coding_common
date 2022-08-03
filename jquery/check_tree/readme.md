
### How to use it

Call this code

Html
```

```

jQuery

```
$(".parent-checkbox input:checkbox").cbFamily(function (){
  return $(this).parents(".parent-checkbox").next().find("input:checkbox");
});
``