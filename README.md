#KAT-API
A simple Node module for fetching data from the Kickass Torrents API in json format.

##Installation
```sh
npm install kat-api
```

##Usage
Get the most popular entries from a category.

```js
var kat = require("kat-api");
kat.mostPopular({
  category: "tv",
  page: 1
},function(err,data){
  if ( err ) {
    throw err;
  }
  
  console.log(data);

});
```
