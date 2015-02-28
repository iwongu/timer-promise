# timer-promise
Promise version of setTimeout and clearTimeout

You can start and stop timer like this.
```js
var timer = require('timer-promise');

timer.start('foo', 5000).
  then(function() {
  }, function(cancelled) {
  });
...
timer.stop('foo');
```
instead of
```js
var timeoutId = setTimeout(function() {
}, 5000);
...
clearTimeout(timeoutId);
```
