# html-dom-pdf

[![NPM version][npm-image]][npm-url]

[npm-image]: https://img.shields.io/npm/v/html-dom-pdf.svg?longCache=true&style=for-the-badge
[npm-url]: https://www.npmjs.com/package/html-dom-pdf

> A javascript tool of transform html-dom-pdf-dom to pdf, support paging Lossless.

## Usage

### install

```bash
# install
$ npm html-dom-pdf -S
```

### project

```js
import HtmlDomPdf from 'html-dom-pdf';

new HtmlDomPdf(options).then(() => {
    // do something.
});

const options = {}; // 👇
```

| Object  |   Prop      |  Type  | Default |   Note            |
| ------- | ----------- | ------ | ------- | ----------------- |
| options. | selector    | String | ''      | [🔗 CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)  |
|         | title       | String | 'pdf'   | filename of pdf   |
|         | marginTB    | Number | 0       | margin of `top` & `bottom` |
|         | marginLR    | Number | 0       | margin of `left` & `right` |
|         | offsetLimit | Number | 40      | <div style="width: 100px;">Maximum offset: Get effective content when paging, trying to intercept upwards, this is the `maximum offset`</div> |

## Releases

* 2019-08-19
    * 0.0.1