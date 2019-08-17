# eocNewsticker: A jQuery newsticker plugin

eocNewsticker is a fully responsive newsticker. It adjusts size and content to any device and window size. It can be configured to read it's contents from the invoking HTML-document or from an AJAX-source (JSON or JSONP). If AJAX is chosen, the newsticker is updated in a given interval on-the-fly.

## Requirements

jQuery 2.2.4 or higher

## Usage

1. Include the provided JS/CSS files

```html
<script src="eoc-newsticker.js"></script>
<link rel="stylesheet" href="eoc-newsticker.css">
```

2. Static or AJAX usage

Write your HTML Content (only for static use)

```html
<div id="example">The quick brown fox jumps over the lazy dog</div>
```

-OR-

Leave the HTML empty and provide a source for AJAX load (see example)

```html
<div id="example"></div>
```

3. Invoke the newsticker on your selected HTML Tag

```javascript
$(function() {
  $("#example").eocNewsticker();
});
```

4. Options

    * speed: The time it takes (in seconds) to move the text 1000px from right to left (normalized) (default: 20)
    * timeout: The time the slider waits after domready, before starting to run (default: 1)
    * divider: The signs used as a divider between the text blocks (default: +++)
    * type:
      * static: Regular usage (default)
      * ajax: Get contents with AJAX from a JSON file
    * source: AJAX source (URL)
    * dataType:
      * json: Regular JSON file from same domain (default)
      * jsonp: JSONP from any source, can be cross-domain
    * callback: Used for jsonp (default: callback)
    * interval: Polling interval of the AJAX source (default: 120)

## Example

Here are some working <a href="https://nightside.de/eoc-newsticker/example.html">eocNewsticker examples</a>.

## License

Released under the MIT license - https://opensource.org/licenses/MIT