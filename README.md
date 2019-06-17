# Responsive images resizer

This package allows you to minify and resize a folder of images to an array of resolutions

`npm install responsive-images-resizer`

## How to use

function: `resizer(inputFolder, outputFolder, resolutionArray)`

Example: <br />

```
const resizer = require('responsive-resizer');
resizer('./images', './build', ['144', '360', '720', '1080']);
```

this will output to `./build` the folders

- 144/
- 360/
- 720/
- 1080/

and inside each folder you will find every image in the input folder at their new resolution

### Note

- this package assumes you want initial aspect ratio

- this package uses GraphicsMagick and as such requires the GraphicsMagick binaries installed and executable from the system PATH

## License

(The MIT License)

Copyright (c) 2019 Andries Kloppers

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
