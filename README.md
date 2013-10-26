
# modelfire

  [Model](https://github.com/component/model) plugin that uses [Firebase](http://www.firebase.com) datasource

## Installation

  Install with [component(1)](http://component.io):

    $ component install maiah/modelfire

## Usage
```js
var model = require('model'),
    modelfire = require('modelfire');

var Person = model('Person')
  .attr('name')
  .attr('job')
  .attr('address')
  .use(modelfire('https://myapp.firebaseio.com/'));

var gohan = new Person();
```

## API

### modelfire(firebaseLocation)

  Enables your [model](https://github.com/component/model) to use and bind to the specified `firebaseLocation`.

## License

  MIT
