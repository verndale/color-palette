# Color Palette
> @verndale/color-palette - A customizable map of colors.

Color palette is a function and a simple map of colors that can be overriden.

## Install
```sh
npm install @verndale/color-palette --save
```

This should be the first file you import in to your main SCSS entry file. You can import this
file either after or before your normalize or reset SCSS, it doesn't matter as color-palette
does not depend on these styles.

## Usage
Define a color map and import the color-palette after the map definition.
```scss
$colors: (
  "blue": "#0000FF",
  "green": "#00FF00"
);

import "node_modules/@verndale/color-palette/colors";


html,
body {
  background: color("blue");
}
```

There are default colors already defined in color-palette, ready for use.

### Standard colors
* "white": #FFF
* "black": #000

### Social media colors
* "reddit-one": #CEE3F8
* "reddit-two": #FF5700
* "twitter": #55ACEE
* "pinterest": #CB2027
* "instagram": #125688
* "facebook": #3B5998
* "linkedin": #007BB5
* "dropbox": #007EE5
* "vine": #00BF8F
* "whatsapp": #4DC247
* "flickr": #FF0084
* "tumblr": #32506D
* "vimeo": #AAD450
* "spotify": #00E461
* "github": #000
* "behance": #1769FF
* "youtube": #B00
* "googleplus": #DD4B39
* "rss": #F60
* "snapchat": #FFFC00

These colors can be used just like the [example above](#usage)
```scss
$colors: (
  "blue": "#0000FF",
  "green": "#00FF00"
);

import "node_modules/@verndale/color-palette/colors";


html,
body {
  color("black");
  background: color("blue");
}

.icon--facebook {
  color: color("facebook");
}
```
