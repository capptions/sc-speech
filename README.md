sc-speech
============

Polymer 1.0 element that speaks text using the HTML5 speech api

`sc-speech` is an invisible element that speaks a given text

- Detects the language of the text automatically using the franc.js library

The element has the following public properties:

- `text`: the text to be spoken
- `accent`: the default accent to be used (`en-US`)
- `autodetect` set to true to automatically detect the accent (`true`)
- `supported` resolves to false if the browser doesn't support the speech api

And the following public api:

- `speak`: actually invoke the speak method on the speech api

The speak method is automatically bound to the `tap` event of the element, in case you want to put an icon in there.

Usage:

```html
  <sc-speech text="How are you doing today?">
  	<iron-icon icon="settings-voice"></iron-icon>
  </sc-speech>
```

Contributions welcome, please create issues!