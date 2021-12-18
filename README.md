# vue-pagination-tw

[![npm version](https://badge.fury.io/js/vue-pagination-tw.svg)](https://badge.fury.io/js/vue-pagination-tw) [![Build Status](https://travis-ci.org/anburocky3/vue-pagination-tw.svg?branch=main)](https://travis-ci.org/anburocky3/vue-pagination-tw) [![Code Climate](https://codeclimate.com/github/anburocky3/vue-pagination-tw/badges/gpa.svg)](https://codeclimate.com/github/anburocky3/vue-pagination-tw)

[![NPM](https://nodei.co/npm/vue-pagination-tw.png)](https://nodei.co/npm/vue-pagination-tw/)

Simple Vue Pagination component that can be used in any project with range &amp; ui customization.

[Online demo](#) (will be updated shortly)

## Installation

### NPM

Install the npm package.

```js
$ npm install vue-pagination-tw --save
```

Register the component.

- ES5

```js
var VuePaginationTw = require("vue-pagination-tw");
Vue.component("VuePaginationTw", VuePaginationTw);
```

- ES6

```js
import VuePaginationTw from "vue-pagination-tw";
Vue.component("VuePaginationTw", VuePaginationTw);
```

### CDN

Include the source file.

```html
<!-- use the latest release -->
<script src="https://unpkg.com/vue-pagination-tw@latest"></script>
<!-- or use the specify version -->
<script src="https://unpkg.com/vue-pagination-tw@0.9.0"></script>
```

Register the component.

```js
Vue.component("VuePaginationTw", VuePaginationTw);
```

## Usage

### In Vue Template

**Basic Usage**

```html
<VuePaginationTw
  :total-items="20"
  :current-page="1"
  :per-page="6"
  @page-changed="functionName"
  :go-button="false"
  styled="centered"
/>
```

_Note_: In vue template, camelCase and kebab-case are both supported. For example, you can either use prop `total-items` or `totalItems`. They are leading to the same result.

So this is also avaliable

```html
<VuePaginationTw
  :totalItems="20"
  :currentPage="1"
  :perPage="6"
  @pageChanged="functionName"
  :goButton="false"
  styled="centered"
/>
```

#### roadmaps

- [ ] Make different versions of paginations (xs, md, lg, xlg)
- [ ] Change Pagination ui templates directly from initialization.
- [ ] Support for make different ui styles by default.
