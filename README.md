# svelte-simple-fileuploader

[![npm version](https://badge.fury.io/js/svelte-simple-fileuploader.svg)](https://badge.fury.io/js/svelte-simple-fileuploader)


A very simple Svelte fileuploader Action to put on HTML elements

![Example](https://github.com/nordquist/svelte-simple-fileuploader/blob/main/fileuploader_0.gif?raw=true)



## Usage
```javascript
import fileuploader from 'svelte-simple-fileuploader';

	use:fileUploader={options}
```
**options**

* enabled - Title of the fileuploader \<optional\>
* dropEnabled - Title of the fileuploader \<optional\>
* allowedFileTypes - Title of the fileuploader \<optional\>
* imageCover - Title of the fileuploader \<optional\>


______________________________________


```
options = {
  allowedFileTypes: '.png,.jpg,.jpeg,.pdf', //allowed file types with .
  imageCover: true //if the image should be used as background on the node
}
```

*Example*
```html
<section id="hero-section"
	use:fileUploader={{
		allowedFileTypes: '.png,.jpg,.jpeg,.pdf',
		imageCover: true
	}}
	on:filesUploaded={handleUploadedFiles}
>
</section>
```


## License

The MIT License (MIT)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.