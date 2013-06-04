# Bootstrap Image Gallery

## Demo
[Bootstrap Image Gallery Demo](http://blueimp.github.com/Bootstrap-Image-Gallery/)

## Description
Bootstrap Image Gallery is an extension to the [Modal](http://twitter.github.com/bootstrap/javascript.html#modal) dialog of Twitter's [Bootstrap](http://twitter.github.com/bootstrap/) toolkit, to ease navigation between a set of gallery images.  
It features mouse and keyboard navigation, transition effects, fullscreen mode and slideshow functionality.

## Usage

### Preparation

To get your photos on there make sure its public and you have an API Key.
You can request on here (http://www.flickr.com/services/apps/create/apply/)

Put your API key under api_key and your photoset id under photoset_id.
To get the photoset id you must create a set, make sure its public, go to the set, and look at the end of the url.
Ex. http://www.flickr.com/photos/87973856@N04/sets/72157633918666858/
72157633918666858 would be the photoset_id

```js
 $.ajax({
        url: 'https://secure.flickr.com/services/rest/',
        data: {
            format: 'json',
            method: 'flickr.photosets.getPhotos',
            api_key: '(api_key)',
			photoset_id: '(photoset_id)',
			extras: 'original_format'
        },
```

## Requirements
* [jQuery](http://jquery.com/) v. 1.7+
* [Bootstrap Modal](http://twitter.github.com/bootstrap/javascript.html#modal) v. 2.2.2+
* [JavaScript Load Image](https://github.com/blueimp/JavaScript-Load-Image) v. 1.2.3+

## License
Released under the [MIT license](http://www.opensource.org/licenses/MIT).
