# Lazyload Print Test

Have you ever been asked to make your lazily loaded images available for the print?
Here's how to do this!

This demo implements a custom print button and it uses [vanilla-lazyload](https://github.com/verlok/lazyload), specifically:

- its `loadAll()` method to load all images in the page before printing
- its `callback_finished` option to pass in a callback which is called when all images finished loading

So when you push the print button it starts loading all images and waits until all images have been loaded to open the print dialog.

If all images were already loaded before and you pus the print button, it just open the print dialog.