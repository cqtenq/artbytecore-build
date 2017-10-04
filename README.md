# artbytecore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install artbytecore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var artbytecoreTasks = require('artbytecore-build');

artbytecoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var artbytecoreTasks = require('artbytecore-build');
artbytecoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/Bushstar/artbytecore) on the main artbytecore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2017 The ArtByte Core Developers
