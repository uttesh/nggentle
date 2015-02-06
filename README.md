# nggentle

Is an AngularJS module for simple gentle plugin which will allow only good words and filter out bad/swear world from input static data. simple directives here will show the bad word on type and service 'paragraph' with 'isGentle' method, method will take input string and find or the bad/swear worlds if found return the list of bad words in input text, it checks around thousand bad/swear words and can be filtered.

Mostly based on various snippets which I found on JSFiddle, with some changes by me.

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/uttesh/nggentle/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
## Quick start

```
bower install ngGentle
```
new version

```
bower install ngGentle0.0.1
```

or alternatively download and include `ngGentle.js` after `angular.min.js`.

Add the `ngGentle` module as a dependency when creating your app, e.g.

```
var app = angular.module('myApp', ['ngGentle']);`

Inject or use in controller

app.controller('filterCtrl', function($scope,paragraph) {
    $scope.txt = "testing the function shi+";
    console.log("gentle : "+paragraph.isGentle($scope.txt));
    
}); 
```

u can use in html as filter.

## Rendering


```
        <textarea ng-model="txt" style=" width:400px;height:200px;"></textarea>
        <gentle ng-model="txt"></gentle>
```


## Contributions

For problems/suggestions please create an issue on Github.

## Contributors

* [@uttesh](https://twitter.com/uttesh)

## Credits

* Other uknown JSFiddles
