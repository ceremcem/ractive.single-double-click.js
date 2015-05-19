# ractive.single-double-click.js

jQuery-like implementation of single and double click handlers.
Allows you to use `dblclick` event without been spammed by `click`. See [this question][0] for details.

## Usage

Include `ractive.single-double-click.js` after `ractive.js`.

**Template**
```html
<div on-singleclick="custom-click" on-doubleclick="custom-dblclick"></div>
```

**Code**
```js
var ractive = new Ractive({
    // nothing special here
});

ractive.on('custom-click', function (event) {
    // ...
});

ractive.on('custom-dblclick', function (event) {
    // ...
});
```

[0]: http://stackoverflow.com/q/1067464/944911
