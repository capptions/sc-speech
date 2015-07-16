sc-speech
============

Polymer 1.0 element that speaks text using the HTML5 speech api

`<sc-speech>` is an invisible element that speaks a given text

- Detects the language of the text automatically using the franc.js library

## Getting started

### Install with bower

First you need bower, [see their site](http://bower.io/) for details 

```
bower install --save sc-speech
```

### Attributes

| Attribute Name | Functionality  | Default |
|----------------|-------------|-------------|
| text | The text to be spoken | `jibberish` |
| accent | the default accent to be used | `en-US` |
| autodetect | set to true to automatically detect the accent | `true` |
| supported | resolves to false if the browser doesn't support the speech api | |

### How to use

The element exposes the method `speak` which actually invokes the speak method on the speech api
This method is automatically bound to the `tap` event of the element, in case you want to put an icon in there.

Usage:

```html
  <sc-speech text="How are you doing today?" id="speech">
  	<iron-icon icon="settings-voice"></iron-icon>
  </sc-speech>
```

Contributions welcome, please create issues!
