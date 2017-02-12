Based on [Vue.js Fundamentals - YouTube](https://www.youtube.com/playlist?list=PLwAKR305CRO_1yAao-8aZiQnBqJeyng4O).

## Notes

### 02 - Setup

Starter `index.html` template.

Minimal Vue app.

### 03 - Directives

Directive begin with 'v-'.

[`v-text`](https://vuejs.org/v2/api/#v-text) -> Updates the element’s `textContent`. If you need to update the part of `textContent`, you should use `{{ Mustache }}` interpolations.

[`v-html`](https://vuejs.org/v2/api/#v-html) -> Updates the element’s `innerHTML`. Note that the contents are inserted as plain HTML - they will not be compiled as Vue templates. If you find yourself trying to compose templates using `v-html`, try to rethink the solution by using components instead.

[`v-show`](https://vuejs.org/v2/api/#v-show) -> Toggle’s the element’s `display` CSS property (adds `display: none` if `false`) based on the truthy-ness of the expression value. This directive triggers transitions when its condition changes.

[`v-if`](https://vuejs.org/v2/api/#v-if) -> Conditionally render the element based on the truthy-ness of the expression value. The element and its contained directives / components are destroyed and re-constructed during toggles. If the element is a `<template>` element, its content will be extracted as the conditional block. This directive triggers transitions when its condition changes.
