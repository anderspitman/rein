# Introduction

rein is a JavaScript UI framework so small it doesn't exist. "rein" is a
German word meaning pure, plain, or clean. It is pronounced similar to
"mine".

The goals of rein
are:

1. Make UI components with no dependencies
2. Tiny runtime
3. Efficient rendering
4. Reusable components, even between frameworks

# Components

rein components are functions that take a state object, and return a DOM
element. That's it. You can render them with raw DOM operations:

```javascript
function MyComponent(state) {
  return document.createElement('div')
    .appendChild(state.);
}

```


Or use your favorite DOM generator:

```javascript
import h from 'hyperscript';

function MyComponent(state) {
  return h('div',
    state.value,
  );
}


```
For more info, check out
[the docs](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model).
