# x-express-session
A clear and direct fork of [express-session](https://github.com/expressjs/session) but with the option to set the sessionid either directly on the header or as a cookie.

## NOTE!!
This fork is the result of a personal need and hence should not be expected to work miracles besides what it was intended to do (pass sessionid directly in the header). You should have at least used express-session before coming over to use this.

The included test is the default express-session test. None has been added for the modifications done.

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
##### options.carrier
Where the session id should be set and retrieved from. Possible values are:

  - `'cookie'`: Set the session id as cookie in the response and read as cookie from the request (default)
  - `'header'`:  Set the session id as header in the response and read as header from the request. The header name is the value passed to the `name` option
  - `'both'`: Performs the above two cases together with the cookie having a higher priority




Please refer to express-session's [session(options)](https://github.com/expressjs/session#sessionoptions) for the remaining full description of `options`.
