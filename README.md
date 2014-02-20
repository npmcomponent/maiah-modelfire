*This repository is a mirror of the [component](http://component.io) module [maiah/modelfire](http://github.com/maiah/modelfire). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/maiah-modelfire`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

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
