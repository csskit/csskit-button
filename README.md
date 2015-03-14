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

- `.button` – **required** – apply to any buttons or a tags you want styled
- `.small`- **optional**
- `.medium`- **optional**
- `.large`- **optional**
- `.full-width`- **optional** – centers, makes button full width on mobile

Example:

```
<button class="button medium full-width">Save</button>
```

To add your own colors or other styles, you can overwrite the classes:

```
.button,
.button:link,
.button:visited {}

.button:hover,
.button:focus {}

.button:active {}
```

Or make your own secondary classes, similar to the included size or full-width classes:

```
.button.example,
.button.example:link,
.button.example:visited {}

.button.example:hover,
.button.example:focus {}

.button.example:active {}
```

```
<a href="#" class="button example">Example</a>
```

## License
[MIT](/LICENSE.md)