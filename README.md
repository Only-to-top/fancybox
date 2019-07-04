# fancybox

<h2>Автоматический клик по ссылке после загрузки страницы</h2>

```html
<div id="firstModal" style="display: none;">
  <p>Подтвердите, что вам больше 18 лет</p>
  <button class="close_modal_no">Нет, мне меньше 18</button>
  <button data-fancybox-close class="close_modal">Да, мне больше 18</button>
  <div style="display: none;">Вам необходимо покинуть сайт!</div>
</div>
```

```js
jQuery(function($) {
	
  var cookieOptions = { expires: 3, path: '/' };
  if ($.cookie('visit') == undefined) {
    setTimeout(function() {
		$.cookie('visit', true, cookieOptions);
		
		$.fancybox.open({
			src: '#firstModal',
			type: 'inline',
			modal: true,
		});
		
    }, 4000);
  }

 });
```

<h4>Так же необходимо подключение jQuery.cookie.js</h4>
