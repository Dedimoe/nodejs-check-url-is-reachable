# nodejs-check-url-is-reachable
Nodejs: check url, is reachable

### Prepare
```
npm install is-reachable
```

### Code
a.js :
```
const isReachable = require('is-reachable');
 
(async () => {
  console.log(await isReachable('https://github.com/Dedimoe/nodejs-check-url-is-reachable/edit/master/README.md'));  //=> true: url is reachable
  console.log(await isReachable('https://github.com/Dedimoe/nodejs-check-url-is-reachable/edit/master/READMExxx.md'));  //=> false : url is unreachable
})();
```

### Run
```
node a.js
```

### Output
```
true
false
```
