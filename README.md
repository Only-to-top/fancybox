# fancybox

<h2>Автоматический клик по ссылке после загрузки страницы</h2>

```html
<a data-fancybox data-src="#firstModal" data-modal="true" href="javascript:;" style="display: none;" class="hidden_link"></a>
<div id="firstModal" style="display: none;">
	<p>Подтвердите, что вам больше 18 лет</p>
	<p><button data-fancybox-close class="close_modal_no">Нет, мне меньше 18</button></p>
	<p><button data-fancybox-close class="close_modal">Да, мне больше 18</button></p>
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
