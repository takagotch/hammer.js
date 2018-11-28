### hammer.js
---
https://github.com/hammerjs/hammer.js

https://github.com/takagotch/hammerjs

```js
var square = document.querySelector('.square');
var hammer = new Hammer(square);
hammer.on('press', function(e){
  e.target.clasList.toggle('expand');
  console.log("You're pressing me!");
  console.log(e);
});

var square = document.querySelector('.square');
var manager = new Hammer.Manager(square);
var TripleTap = new Hammer.Tap({
  event: 'tripletap',
  taps: 3
});
manager.add(TripleTap);
manager.on('tripletap', function(e){
  e.target.classList.toggle('expand');
  console.log("You're triple tapping me!");
  console.log(e);
});
```

```
npm install --save hammerjs
yarn add hammerjs
```

```
```


