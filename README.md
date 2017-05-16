Apache OpenWhisk Web action redirecting request to Express applications

How to use
==========

The basic usage is:

```
const app = require('./server');
const forward = require('openwhisk-expressjs')(app);

function main(request) {
  return forward(request);
}

exports.main = main;
```
