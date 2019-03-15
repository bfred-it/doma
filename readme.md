# doma [![(size)][badge-gzip]](#no-link) [![(status)][badge-travis]][link-travis]

  [badge-gzip]: https://img.shields.io/bundlephobia/minzip/doma.svg?label=gzipped
  [badge-travis]: https://api.travis-ci.com/bfred-it/doma.svg?branch=master
  [link-travis]: https://travis-ci.org/bfred-it/doma
  [link-npm]: https://www.npmjs.com/package/doma

> Parse an HTML string into `DocumentFragment` or one `Element`, in a few bytes (in browser or jsdom)

## Install

```
npm install doma
```

## Setup

```js
const doma = require('doma');
```

```js
import doma from 'doma';
```

## Usage

```js
doma('<h1>Cats</h1> and dogs');
//=>  DocumentFragment[<h1>, Text(' and dogs')]

doma('the cow');
//=>  DocumentFragment[Text('the cow')]

doma.one('beautiful <i>bird</i>');
//=>  <i>

doma.one('wild animal');
//=>  null
```

## Related

- [select-dom](https://github.com/bfred-it/select-dom) - Lightweight `querySelector`/`All` wrapper that outputs an Array.
- [delegate-it](https://github.com/bfred-it/delegate-it) - DOM event delegation, in <1KB.
- [Refined GitHub](https://github.com/sindresorhus/refined-github) - Uses this module.
