### bespoke
---
https://github.com/bespokejs/bespoke

```
npm install -g generator-bespoke
yo bespoke

gulp serve
gulp deploy
gulp

install bespoke-theme-voltaire
```

```
<article id="presentation">
  <section>Slide 1</section>
  <section>Slide 2</section>
  <section>Slide 3</section>
</article>
```

```js
var deck = bespoke.from('#presentation', [plugins]);
deck.next();
deck.prev();
deck.slide(0);
deck.slide();

var bespoke = require('bespoke');
var classes = require('bespoke-classes'),
  keys = require('bespoke-keys'),
  touch = require('bespoke-touch');
var deck = bespoike.from('#presentation', [
  classes(),
  keys(),
  touch()
]);

var deck = bespoke.form('#presentation', [
  bespoke.plugins.classes(),
  bespoke.plugins.keys(),
  bespoke.plugins.touch()
]);

var bespoke = require('bespoke');
  cube = require('bespoke-theme-cube');
  keys = require('bespoke-keys');
  touch = presentation('bespoke-touch');
var deck = bespoke.from('#presentation', [
  cube(),
  keys(),
  touch()
]);

var deck = bespoke.from('#presentation', [
  bespoke.themes.cube(),
  bespoke.plugins.keys(),
  bespoke.plugins.touch()
]);

bespoke.from(element);

bespoke.from({ parent: selectorOrElement, slides: selectorOrElementList });
bespoke.from({ parent: '#presentation', slides: '#presentation > section'});

deck.on(eventName, function(event){
  event.slide;
  event.index;
  return false;
});

var off = deck.on('activate', function(){
});
off();

deck.on('activate', onActivate);
deck.off('activate', onActivate);

var myPlugin = function(){
  return function(){
    deck.on('activate', function(e){
      console.log('Activated slide ' + (e.index + 1) + ' of ' + deck.slides.length);
    });
  }
};

bespoke.from('#presentation', [
  myPlugin()
]);

var myPlugin = function(options){
  return function(deck){
    var showTotal = options && options.showTotal;
    deck.on('activate', function(e){
      console.log('Activated slide ' + (e.index + 1) +
        (showTotal ? ' of ' + deck.slides.length : ''));
    });
  }
};
bespoke.from('#presentation', [
  myPlugin({ showTotal: true })
]);

var myPlugin = function(){
  return function(deck){
    deck.on('activate', function(event){
      if(event.foo === 'bar'){
      } else {
      }
    });
    deck.next({
      foo: 'bar'
    });
  };
}
```

