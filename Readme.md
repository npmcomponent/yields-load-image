*This repository is a mirror of the [component](http://component.io) module [yields/load-image](http://github.com/yields/load-image). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-load-image`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# load-image

  Creates and loads an image.

## Installation

    $ component install yields/load-image

## Example

```js
var image = require('load-image');
var body = document.body;
body.className = 'loading';
image('/foo.jpg', function(err, img){
  if (err) throw err;
  body.className = '';
  body.style.background = 'url(' + img.src + ')';
});
```
   

## License

  MIT
