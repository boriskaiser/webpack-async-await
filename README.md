# webpack-async-await

A plugin for webpack understands the ES7 keywords `async` and `await`, making building code for Chrome 53, Edge 14 and other 
ES7-capable platforms simple.

Usage:

```

var webpack = require('webpack');
var AsyncAwaitPlugin = require('webpack-async-await') ;

var options = { } ; // See https://github.com/MatAtBread/acorn-es7-plugin#options--compliance

webpack({
    plugins: [
      new AsyncAwaitPlugin(options)
    ],
    
    ...
}).run(function(err,stats){
    ...
});

```

Further details on the available options can be found at https://github.com/MatAtBread/acorn-es7-plugin#options--compliance
