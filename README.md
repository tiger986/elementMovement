## Click the corresponding button to move the element up and down
#### HTML code
```html
<div class="box">
    <div class="d1">
	<p class="p1">up</p>
	<p>d1</p>
	<p class="p2">down</p>
    </div>		
    <div class="d2">
	<p class="p1">up</p>
	<p>d2</p>
	<p class="p2">down</p>
    </div>
</div>
```
#### JS code
```javascript
$(function(){		
    $(".p1").click(function(){
        $(this).parent().after($(this).parent().prev());
    });
		
    $(".p2").click(function(){
        $(this).parent().before($(this).parent().next());
    });			
})
