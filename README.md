# Morgan
> Lightweight boilerplate for modularization

Morgan is a tiny library for registering, extending, loading and using custom web components.  

- morgan.html `1,53 KB`
- morgan.min.html `930 bytes`
- morgan.min.html.gz `497 bytes`

## "Install"
`<link rel="import" href="morgan.html">`

## Documentation
### Register
```
var name = 'x-component';
var options = {
  base, // Base element name
  setup, // Executed when instantiated
  update, // Executed when attributes change
  attach, // Executed when the element is attached to DOM
  detach // Executed when the element is detached to DOM
};
Morgan.register(name, options);
```
Note that Morgan will associate the first `<template>` with the component, enforcing separated files.
### Load
```
var href = '/components/x.html';
Morgan.load(href);
```
### Use
```
var element = Morgan.use('x-biometric', { // Element name
  type: 'password' // Attributes
}, 'input'); // Base element name
```
## Todo
- Enchance documentation

## Meta
Distributed under the MIT license. See ``LICENSE.md`` for more information.

[Huijari](https://github.com/huijari/)