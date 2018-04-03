# Eight Sleep Shogun Element Builder
By Peter Laxalt 2018

[www.laxaltandmciver.co](http://www.laxaltandmciver.co/)

Simple structure for building custom [Shogun](http://getshogun.com/) elements.

## Setup
1. Install Sass using [their guide.](http://sass-lang.com/install)
2. Install `wget` with Homebrew. `brew install wget`.
2. Create a new `element` in the `/elements/` directory. Feel free to duplicate the base template. 
3. `cd` into the respective directory and use `sass --sourcemap=none --watch sass:css`  to convert your SCSS into CSS for the element.
4. Make sure you are loading the most up to date Shopify SCSS from the Live Eight site. I set up a `eight-shopify` directory outside of my `eight-shogun` directory and loading it from there. 
6. Clean your `shopify-styles` directory, make a new one, and copy the latest CSS from the Eight site to your directory.
```rm -rf shopify-styles && mkdir shopify-styles && wget -P shopify-styles/ "https://cdn.shopify.com/s/files/1/1354/6123/t/9/assets/app.min.css" && wget -P shopify-styles/ "https://cdn.shopify.com/s/files/1/1354/6123/t/9/assets/theme.scss.css"```
5. Unix: Boot up a SimpleHTTPServer with Python to serve your files with ```python -m SimpleHTTPServer 1337```. *Make sure your `eight-shopify` and `eight-shogun` directories are visible to the server.
6. Navigate to [localhost:1337](localhost:1337) to test your elements.

https://cdn.shopify.com/s/files/1/1354/6123/t/9/assets/theme.scss.css

rm -rf shopify-styles && mkdir shopify-styles && wget -P shopify-styles/ "https://cdn.shopify.com/s/files/1/1354/6123/t/9/assets/app.min.css" && wget -P shopify-styles/ "https://cdn.shopify.com/s/files/1/1354/6123/t/9/assets/theme.scss.css"