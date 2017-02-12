Based on [Vue.js Fundamentals - YouTube](https://www.youtube.com/playlist?list=PLwAKR305CRO_1yAao-8aZiQnBqJeyng4O).

## Notes

### 02 - Setup

Starter `index.html` template.

Minimal Vue app.

### 03 - Directives

Directive begin with 'v-'.

[`v-text`](https://vuejs.org/v2/api/#v-text) -> Updates the element’s `textContent`. If you need to update the part of `textContent`, you should use `{{ Mustache }}` interpolations.

[`v-html`](https://vuejs.org/v2/api/#v-html) -> Updates the element’s `innerHTML`. Note that the contents are inserted as plain HTML - they will not be compiled as Vue templates. If you find yourself trying to compose templates using `v-html`, try to rethink the solution by using components instead.
