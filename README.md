ionic-rating
============

An angularjs directive that take care of visualising a star rating bar, build
for ionic.

![rating](https://cloud.githubusercontent.com/assets/1183541/3007107/3cee642c-de6c-11e3-8449-18b86ca130a7.png)


#### Why?

`angular-ui` has the same [rating](http://angular-ui.github.io/bootstrap/#/rating) directive,
but it is build on top of bootstrap. This repo just reuse most of the js code, but build for
the [ionic](http://ionicframework.com/) framework.

#### How to use?

Install with bower:

```
$ bower install ionic-rating
```

In you template:

```
<rating ng-model="rate" max="max"></rating>
```

In you controller:

```
// first inject it into your app
angular.module('youApp', ['ionic.rating'])

.controller('yourCtrl', function($scope) {

  // set the rate and max variables
  $scope.rate = 3;
  $scope.max = 5;

});

```

**Note:** You may also need to include the style file. But I suggest you just copy it to your
project.

#### Build

```
$ npm i
$ make all
```

#### License

MIT