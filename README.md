# element-matches-polyfill
Polyfill for Element.matches

Provides a polyfill for [Element.forEach()](https://developer.mozilla.org/en-US/docs/Web/API/Element/matches) to all Browsers.

## Native support

See [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Element/matches) for more information.

### Reduced scope

I personally use: https://github.com/jelmerdemaat/element-matches as I don't need to support all browsers.

## Import

```JavaScript
// CommonJS
require('element-matches-polyfill');

// ES6 Modules import / Typescript import
import 'element-matches-polyfill';
```

## Install

```shell
npm install --save element-matches-polyfill
```

## Usage

```HTML
<ul id="birds">
  <li>Orange-winged parrot</li>
  <li class="endangered">Philippine eagle</li>
  <li>Great white pelican</li>
</ul>

<script type="text/javascript">
  var birds = document.getElementsByTagName('li');

  for (var i = 0; i < birds.length; i++) {
    if (birds[i].matches('.endangered')) {
      console.log('The ' + birds[i].textContent + ' is endangered!');
    }
  }
</script>
```
