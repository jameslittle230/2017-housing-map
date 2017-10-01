# 2017 Housing Map

This repository holds code used to embed an interactive map on <bowdoinorient.com/housing>. The code is based on the site's WordPress installation, and thus shouldn't be cloned; rather, it just shows the mechanisms used to make the map.

`base.html` is the HTML structure of the article, and goes in the content field in WordPress. The `[map]` shortcode on line 169 is replaced with the contents of map.svg by the WordPress engine.

`embedded-code.html` is embedded onto the page using a WordPress plugin. It contains custom CSS and JavaScript used to enable the interactivity.

`map.svg` is the entire SVG code for the map, which is rather uninteresting, but was included because I manually added class names to specific paths in order to enable the color changing aspect of the visualization.