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

[`v-pre`](https://vuejs.org/v2/api/#v-pre) -> Skip compilation for this element and all its children. You can use this for displaying raw mustache tags. Skipping large numbers of nodes with no directives on them can also speed up compilation.

[`v-once`](https://vuejs.org/v2/api/#v-once) -> Render the element and component __once__ only. On subsequent re-renders, the element/component and all its children will be treated as static content and skipped. This can be used to optimize update performance. Also, see [Cheap Static Components with v-once](https://vuejs.org/v2/guide/components.html#Cheap-Static-Components-with-v-once) -> Rendering plain HTML elements is very fast in Vue, but sometimes you might have a component that contains __a lot__ of static content. In these cases, you can ensure that it’s only evaluated once and then cached by adding the `v-once` directive to the root element.

[`v-cloak`](https://vuejs.org/v2/api/#v-cloak) -> This directive will remain on the element until the associated Vue instance finishes compilation. Combined with CSS rules such as `[v-cloak] { display: none }`, this directive can be used to hide un-compiled mustache bindings until the Vue instance is ready.

### 04 - [`v-bind` directive](https://vuejs.org/v2/api/#v-bind)

Shorthand: `:`
