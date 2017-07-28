### Installation
```sh
$ npm install ssn-mask
```

```
var app = angular.module('ssnApp', ['ssnMaskMod']);

app.controller('MainCtrl', function($scope) {
  $scope.ssnval = '';
});

<!DOCTYPE html>
<html ng-app="ssnApp">
  <head>
    <script src="https://code.jquery.com/jquery.js"></script>
    <script src="https://cdn.rawgit.com/digitalBush/jquery.maskedinput/master/src/jquery.maskedinput.js"></script>
    <script data-require="angular.js@1.5.x" src="https://cdnjs.cloudflare.com/ajax/libs/angular.js/1.5.11/angular.min.js" data-semver="1.5.11"></script>
    <script src='node_modules/ssn-mask/ssn-mask.js'></script>
    <script src="app.js"></script>
  </head>
  <body ng-controller="MainCtrl">
    <input type="text" ng-model='ssnval' ssn-input >
    <p>SSN {{ssnval}} !</p>
  </body>
</html>
```

##### Dependencies
* [Masking Dependency] - https://github.com/digitalBush/jquery.maskedinput

#### Demo:
* https://htmlpreview.github.io/?https://github.com/deepakkoirala/SSN-Mask-Angular-Js/blob/master/index.html