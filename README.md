# img-onload

```js
document.addEventListener('DOMContentLoaded', function() {

    document.querySelectorAll('.works__img').forEach(function(el, index) {
        el.onload = function() {
            if ($(window).width() > 1200) {

                let height_block = $('.works__img').height();
                $('.works--height').height(height_block);

                $(window).resize(function () {
                    let height_block = $('.works__img').height();
                    $('.works--height').height(height_block);
                });
            };
        }
    });

});
```
