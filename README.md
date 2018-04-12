# x-express-session
A clear and direct fork of [express-session](https://github.com/expressjs/session) but with the option to set the sessionid either directly on the header or as a cookie.

## Usage

To install
```sh
$ npm install x-express-session
```

API:
```js
var session = require('x-express-session')
```

### session(options)
Please refer to express-session [session(options)](https://github.com/expressjs/session#sessionoptions) description




## NOTE!!
This Fork is the result of a personal need and hence should not be expected to work miracles besides what it was intended to do (pass sessionid directly in the header)

The included test is the default express-session test. None has been added for the modifications done.