# Sticky

Sticky is a jQuery plugin that gives you the ability to make any element on your page always stay visible.

The version in this fork is a bit different than the [original](https://github.com/garand/Sticky):

- When the target element is about to be hidden, the plugin will add the class `className` to it (and to it's parent wrapper), set it to `position: fixed` and calculate it's new `top`, based on the element's height, the page height and the `topSpacing` and `bottomSpacing` options.
- That's it. The plugin won't mess with your element's size, so you should do it in your own css if you need to. Check the `example-*.html` files for some examples.

## Usage

- Include jQuery & Sticky.
- Call Sticky.

```javascript
<script src="jquery.js"></script>
<script src="jquery.sticky.js"></script>
<script>
  $(document).ready(function(){
    $("#sticker").sticky({topSpacing:0});
  });
</script>
```

- Edit your css to position the elements (check the examples in `example-*.html`).


## Options

|topSpacing      |
|:--------------:|
|bottomSpacing   |
|className       |
|wrapperClassName|

## Methods

* `sticky(options)`: Initializer. `options` is optional.
* `sticky('update')`: Recalculates the element's position.

 