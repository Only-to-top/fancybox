# fancybox

<h2>Автоматический клик по ссылке после загрузки страницы</h2>

```html
<div id="firstModal" style="display: none;">
  <p>Подтвердите, что вам больше 18 лет</p>
  <button class="close_modal_no">Нет, мне меньше 18</button>
  <button data-fancybox-close class="close_modal">Да, мне больше 18</button>
</div>
```

```js
jQuery(function($) {
  
	$.fancybox.open({
		src: '#firstModal',
		type: 'inline',
		modal: true,
	});
	
});
```
