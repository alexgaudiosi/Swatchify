# Swatchify
So building on Shopify's existing swatch selector found [HERE](https://help.shopify.com/themes/customization/showcase-products/add-color-swatches), follow the guide there, then we'll make a few adjustments.
This addition gives you a bit more versatility when you have two different variant selectors, the two most common being size and colour, and updating out of stock variants as you switch between colours, allowing the user to quickly get the stock information they need.

![Swatch GIF](/images/swatch.gif)

This method doesn't use the default soldout.png image - but it's preserved in there and can be added with a few modifications. There may be a few issues with implementation I've overlooked, just let me know if there are and I'll update the guide.

##### What you need to do

1. In your product.liquid, find the selectCallback function, and below what's already in there, replace the existing swatch JS with that in `swatch-callback.js`

2. In your `swatch.liquid` snippet, copy and replace the entire swatch.liquid file contents.

3. In `timber.scss.liquid` (or stylesheet equivalent), add the 'unavailable' class styling from `swatch.css`. Style as you see fit, this is just one I baked earlier. 

##### To Do

In it's current state, it's somewhat project specific, I'll generalise it soon so it's more widely useable, though you shouldn't have too much trouble making adjustments.