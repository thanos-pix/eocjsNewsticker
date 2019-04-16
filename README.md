# eocNewsticker: A simple jQuery newsticker plugin

## Requirements

jQuery 1.10.2 or higher

## Usage

1. Include the provided JS/CSS files

```html
<script src="jquery.eocnewsticker.js"></script>
<link rel="stylesheet" href="eocnewsticker.css">
```

2. Write your HTML Content

```html
<div id="eocnewsticker">The quick brown fox jumps over the lazy dog</div>
```

3. Invoke the newsticker on your selected HTML Tag

```javascript
$(function() {
  $("#eocnewsticker").eocNewsticker();
});
```

4. Options

    * speed: The time it takes (in seconds) to move the whole text from right to left
    * timeout: The time the slider waits after domready, before starting to run
    * divider: The signs used as a divider between the text blocks (if the text is not long enough to fill the whole width)

## Notice

Please bear in mind, that this project is in a very early stage of development, so please have mercy with me :)
