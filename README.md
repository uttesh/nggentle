# nggentle

Is an AngularJS module for simple gentle plugin which will allow only good words and filter out bad/sear world form on static data. simple directives here the will show the bad word on type and service 'paragraph' with methods 'isGentle' method which will take input string and find or the bad/swear worlds if found return the list is bad words in input text, here around thousand bad/sear words are listed and can be filtered.

Mostly based on various snippets which I found on JSFiddle, with some changes by me.

## Quick start

```
bower install ngGentle
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
