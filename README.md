# webpack-serve-issue-70-demo

This is a demo to showcase [issue 70 from webpack-serve](https://github.com/webpack-contrib/webpack-serve/issues/70).

I use `stats: 'minimal'` which should just output `1 module`, but as you can see I get the defaut output when I use `webpack-serve` (everything after `ℹ ｢wdm｣:`).

```
$ npm install
$ npm run build

> webpack-serve-issue-70-demo@1.0.0 build /home/pipo/workspace/webpack-serve-issue-70-demo
> webpack

   1 module
$ npm run start

> webpack-serve-issue-70-demo@1.0.0 start /home/pipo/workspace/webpack-serve-issue-70-demo
> webpack-serve

ℹ ｢hot｣: webpack: Compiling...
ℹ ｢hot｣: WebSocket Server Listening at localhost:8081
ℹ ｢serve｣: Project is running at http://localhost:8080
ℹ ｢serve｣: Server URI copied to clipboard
ℹ ｢hot｣: webpack: Compiling Done
ℹ ｢wdm｣: Hash: f9a7cb7fa2e714209f14
Version: webpack 4.2.0
Time: 11521ms
Built at: 2018-3-22 13:25:03
  Asset     Size  Chunks             Chunk Names
main.js  109 KiB    main  [emitted]  main
Entrypoint main = main.js
[./node_modules/loglevelnext/dist/loglevelnext.js] 18.1 KiB {main} [built]
[./node_modules/punycode/punycode.js] 14.3 KiB {main} [built]
[./node_modules/querystring-es3/encode.js] 2.48 KiB {main} [built]
   [0] multi ./src 28 bytes {main} [built]
[./node_modules/webpack-hot-client/client/index.js?8dbc4980-c6fa-4860-9051-353c04e71ac3] (webpack)-hot-client/client?8dbc4980-c6fa-4860-9051-353c04e71ac3 1.78 KiB {main} [built]
   [1] multi webpack-hot-client/client?8dbc4980-c6fa-4860-9051-353c04e71ac3 ./src 40 bytes {main} [built]
[./node_modules/querystring-es3/index.js] 127 bytes {main} [built]
[./node_modules/url/url.js] 22.8 KiB {main} [built]
[./node_modules/url/util.js] 314 bytes {main} [built]
[./node_modules/webpack-hot-client/client/hot.js] (webpack)-hot-client/client/hot.js 4.23 KiB {main} [built]
[./node_modules/webpack-hot-client/client/log.js] (webpack)-hot-client/client/log.js 2.4 KiB {main} [built]
[./node_modules/webpack-hot-client/client/socket.js] (webpack)-hot-client/client/socket.js 1.37 KiB {main} [built]
[./node_modules/webpack/buildin/global.js] (webpack)/buildin/global.js 509 bytes {main} [built]
[./node_modules/webpack/buildin/module.js] (webpack)/buildin/module.js 519 bytes {main} [built]
[./src/index.js] 20 bytes {main} [built]
    + 1 hidden module
ℹ ｢wdm｣: Compiled successfully.
^Cℹ ｢serve｣: Process Ended via SIGINT
```