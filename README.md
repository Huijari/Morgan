# Morgan
> Simple boilerplate for WebComponents

Library for registering, loading and using custom web components.  
Under 2kb without minify, without compression.

## "Install"
`<link rel="import" href="morgan.html">`

## Documentation
### Register
```
var name = 'x-component';
var options = {
  setup, // Executed when instantiated
  update, // Executed when attributes change
  attach, // Executed when the elements is attached to DOM
  deattach // Executed when the elements is deattached to DOM
};
Morgan.register(name, options);
```
### Load
```
var href = '/components/x.html';
Morgan.load(href);
```
### Use
```
var element = Morgan.use('input', {
  type: 'password'
});
```
## Todo
- Inheritance
- Enchance documentation

## Meta
Distributed under the MIT license. See ``LICENSE.md`` for more information.

[Huijari](https://github.com/huijari/)