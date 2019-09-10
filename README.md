# input-mask library

## Install Jquery Mask Plugin
```bash
npm install jquery-mask-plugin

yarn add jquery-mask-plugin
```

## Add to app.js
```javascript
require('jquery-mask-plugin');

function mask(elements, mask) {
    if (!$().mask) {
        console.error('JQuery Mask Plugin not loaded');
        return;
    }

    if (elements.length) {
        for (let element of elements) {
            $(element).mask(mask);
        }
    }
}

$(document).ready(function () {
    var elements = document.getElementsByClassName('phone-input');

    mask(elements, "(999) 999-9999")
});
```


## How to use
```html
<input class="phone-input" type="text" />
```
