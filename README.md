# csskit-button

simple css for buttons.

## Install

```
npm i --save csskit-button
```

Or just grab the css.

## Usage

If you installed with npm:

- In your main css file: `@import "csskit-button";`
- Use [sheetify](http://npmjs.org/sheetify) or [npm-rework-cli](http://npmjs.org/npm-rework-cli) to bundle the css.
- Example using npm-rework-cli: `npm-rework main.css -o bundle.css`

### CSS classes:

- `.button` – **required on `a` tags that need button styles**
- `.small`- **optional**
- `.medium`- **optional**
- `.large`- **optional**
- `.full-width`- **optional** – makes button full width

Example:

```
<button class="button medium full-width">Save</button>
```

To add your own colors or other styles, you can overwrite the classes:

```
.button,
.button:link,
.button:visited,
button,
input[type="submit"],
input[type="reset"],
input[type="button"] {

}

.button:hover,
.button:focus,
button:hover,
input[type="submit"]:hover,
input[type="reset"]:hover,
input[type="button"]:hover,
button:focus,
input[type="submit"]:focus,
input[type="reset"]:focus,
input[type="button"]:focus {

}

.button:active,
button:active,
input[type="submit"]:active,
input[type="reset"]:active,
input[type="button"]:active {

}
```

Or make your own secondary classes, similar to the included size or full-width classes:

```
.button-example,
.button-example:link,
.button-example:visited {}

.button-example:hover,
.button-example:focus {}

.button-example:active {}
```

Then use the new button-example class on all button-style inputs:

```
<button class="button-example">Example</button>
```

## License
[MIT](/LICENSE.md)