## testapi

Extremely simple node.js api using [express](https://expressjs.com/en/starter/hello-world.html), just to demonstrate that pulling in one dependency to build a hello-world API, brings at first the following dependency tree:

```
$ npm ls -p

/home/pablo/tesis/testapi
/home/pablo/tesis/testapi/node_modules/express
```

But adding transitive dependencies (which all are rooted in express):
```
$ npm ls -ap

/home/pablo/tesis/testapi
/home/pablo/tesis/testapi/node_modules/express
/home/pablo/tesis/testapi/node_modules/accepts
/home/pablo/tesis/testapi/node_modules/array-flatten
/home/pablo/tesis/testapi/node_modules/body-parser
/home/pablo/tesis/testapi/node_modules/content-disposition
/home/pablo/tesis/testapi/node_modules/content-type
/home/pablo/tesis/testapi/node_modules/cookie-signature
/home/pablo/tesis/testapi/node_modules/cookie
/home/pablo/tesis/testapi/node_modules/debug
/home/pablo/tesis/testapi/node_modules/depd
/home/pablo/tesis/testapi/node_modules/encodeurl
/home/pablo/tesis/testapi/node_modules/escape-html
/home/pablo/tesis/testapi/node_modules/etag
/home/pablo/tesis/testapi/node_modules/finalhandler
/home/pablo/tesis/testapi/node_modules/fresh
/home/pablo/tesis/testapi/node_modules/http-errors
/home/pablo/tesis/testapi/node_modules/merge-descriptors
/home/pablo/tesis/testapi/node_modules/methods
/home/pablo/tesis/testapi/node_modules/on-finished
/home/pablo/tesis/testapi/node_modules/parseurl
/home/pablo/tesis/testapi/node_modules/path-to-regexp
/home/pablo/tesis/testapi/node_modules/proxy-addr
/home/pablo/tesis/testapi/node_modules/qs
/home/pablo/tesis/testapi/node_modules/range-parser
/home/pablo/tesis/testapi/node_modules/safe-buffer
/home/pablo/tesis/testapi/node_modules/send
/home/pablo/tesis/testapi/node_modules/serve-static
/home/pablo/tesis/testapi/node_modules/setprototypeof
/home/pablo/tesis/testapi/node_modules/statuses
/home/pablo/tesis/testapi/node_modules/type-is
/home/pablo/tesis/testapi/node_modules/utils-merge
/home/pablo/tesis/testapi/node_modules/vary
/home/pablo/tesis/testapi/node_modules/mime-types
/home/pablo/tesis/testapi/node_modules/negotiator
/home/pablo/tesis/testapi/node_modules/bytes
/home/pablo/tesis/testapi/node_modules/destroy
/home/pablo/tesis/testapi/node_modules/iconv-lite
/home/pablo/tesis/testapi/node_modules/raw-body
/home/pablo/tesis/testapi/node_modules/unpipe
/home/pablo/tesis/testapi/node_modules/ms
/home/pablo/tesis/testapi/node_modules/inherits
/home/pablo/tesis/testapi/node_modules/toidentifier
/home/pablo/tesis/testapi/node_modules/ee-first
/home/pablo/tesis/testapi/node_modules/forwarded
/home/pablo/tesis/testapi/node_modules/ipaddr.js
/home/pablo/tesis/testapi/node_modules/side-channel
/home/pablo/tesis/testapi/node_modules/mime
/home/pablo/tesis/testapi/node_modules/send/node_modules/ms
/home/pablo/tesis/testapi/node_modules/media-typer
/home/pablo/tesis/testapi/node_modules/mime-db
/home/pablo/tesis/testapi/node_modules/safer-buffer
/home/pablo/tesis/testapi/node_modules/call-bind
/home/pablo/tesis/testapi/node_modules/get-intrinsic
/home/pablo/tesis/testapi/node_modules/object-inspect
/home/pablo/tesis/testapi/node_modules/function-bind
/home/pablo/tesis/testapi/node_modules/has-proto
/home/pablo/tesis/testapi/node_modules/has-symbols
/home/pablo/tesis/testapi/node_modules/has
```

Total, itś 58 dependencies.