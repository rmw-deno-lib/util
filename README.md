<!-- 本文件由 ./readme.make.md 自动生成，请不要直接修改此文件 -->

# sleep for seconds

## sleep

export in your `deps.js`

```
export sleep from 'https://deno.land/x/rmw_sleep@0.0.2/lib/sleep.js'
```

source code

```coffee
export default (sec)=>
  new Promise((resolve) => setTimeout(resolve, sec * 1000))


```

coffeescript version

```coffee
import sleep from './sleep.js'


do =>
  n = 0
  while ++n < 3
    console.log new Date()
    await sleep 1

```


javascript version

```javascript
// Generated by CoffeeScript 2.5.1
import sleep from './sleep.js';

(async() => {
  var n, results;
  n = 0;
  results = [];
  while (++n < 3) {
    console.log(new Date());
    results.push((await sleep(1)));
  }
  return results;
})();

//# sourceMappingURL=sleep_test.js.map

```
