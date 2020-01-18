![](https://badgen.net/badge/Editor.js/v2.0/blue)

# Paragraph Tool for Editor.js

Edited text (paragraph) Tool for the [Editor.js] (https://ifmo.su/editor) that allows empty blocks that can be converted to line breaks. This package was made from Editor.js paragraph tool (https://github.com/editor-js/paragraph).

## Installation

### Install via NPM

Get the package

```shell
yarn add @xinruili07/@xinruili07/paragraph-with-line-breaks
```

Include module at your application

```javascript
const Paragraph = require('@xinruili07/paragraph-with-line-breaks');
```

### Download to your project's source dir

1. Upload folder `dist` from repository
2. Add `dist/bundle.js` file to your page.

### Load from CDN

You can load specific version of package from [jsDelivr CDN](https://www.jsdelivr.com/package/npm/@editorjs/paragraph).

`https://cdn.jsdelivr.net/npm/@editorjs/paragraph@2.0.2`

Then require this script on page with Editor.js.

```html
<script src="..."></script>
```

## Usage

Add a new Tool to the `tools` property of the Editor.js initial config.

```javascript
var editor = EditorJS({
  ...
  
  tools: {
    ...
    paragraph: {
      class: Paragraph,
      inlineToolbar: true,
    },
  }
  
  ...
});
```

## Config Params

This Tool has no config params

## Output data

| Field  | Type     | Description      |
| ------ | -------- | ---------------- |
| text   | `string` | paragraph's text |


```json
{
    "type" : "paragraph",
    "data" : {
        "text" : "Check out our projects on a <a href=\"https://github.com/codex-team\">GitHub page</a>.",
    }
}
```

