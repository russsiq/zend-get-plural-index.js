# zend-get-plural-index.js
Get the index to use for pluralization. The plural rules are derived from code of the Zend Framework.

```php
* @category    Zend
* @package     Zend_Locale
* @public      https://github.com/zendframework/zf1/blob/master/library/Zend/Translate/Plural.php
* @copyright   2005-2015 Zend Technologies USA Inc. http://www.zend.com
* @license     http://framework.zend.com/license     New BSD License
```

### Installation

Download library or can be installed as `npm` package:

```console
npm i zend-get-plural-index.js --save-dev
```

### Getting started and usage examples

```js
<script type="text/ecmascript-6">
import getPluralIndex from 'zend-get-plural-index.js'

let count, index
let locale = 'ru_Ru'
let choices = ['яблоко', 'яблока', 'яблок']

count = 22
index = getPluralIndex(locale, count)
console.log(`У меня было ${count} ${choices[index]}.`)

count = 1
index = getPluralIndex(locale, count)
console.log(`У меня осталось ${count} ${choices[index]}.`)

count = 888
index = getPluralIndex(locale, count)
console.log(`Но у меня скоро будет ${count} ${choices[index]}.`)
</script>
```
