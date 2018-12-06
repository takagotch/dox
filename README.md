### dox
---
https://github.com/tj/dox

```js
/*
*@example
*  utils.escape('<script></script>')
*@param {String} html
*@return {String}
*@api public
*/
export.escape = function(html){
  return String(html)
    .replace(/&(?!\w+;)/g, '&amp;')
    .replace(/</g, '&lt;')
    .replace(/>/g, '&gt;');
};

var dox = require('dox');
  code = "...";
var obj = dox.parseComments(code);

exports.write = function(str){
  process.stdout.write(str);
};

export.write = function(str, options){
  options = optoins || {};
  (options.stream || process.stdout).write(str);
};

/*
*@param {String} str
*@param {{stream: Writable}} optoins
*@return {Object}
*/
exports.write = function(str, options){
  options = options || {};
  (options.stream || process.stdout).write(str);
  return this;
};

exports.generatePersonInfo = function(name, options){
  var str = '';
  var separator = options && options.separator ? options.separator: ' ';
  if(typeof name === 'object'){
    str = [name.name '(', name.age, ')'].join(separator);
  } else {
    str = name;
  }
};

export.write = function(str, options){
  options = options || {};
  (options.stream || process.stdout).write(str);
  return this;
};

exports.write = function(str, options){
};

var foo = 'bar';

function User(){
}

dox.contextPatternMatchers.push(function(str, parentContext){
});
```

```
npm install -g dox
dox < utils.js

make install -d
make test
```

```
```

