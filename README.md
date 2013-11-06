# ngLivi18n

Angular Module for Livi18n.js

## Requirements

 - AngularJS 1.0.5+
 - Livi18n.js 0.1.0

## Installing

Simply download the `ngLivi18n.js` file and add it to your web application. Just make sure it's included after the AngularJS script.

## Usage

 1. Add the `ngLivi18n` module as a dependency in your AngularJS app;
 2. Inject the `$livi18n` factory wherever you need to use Livi18n.js;
 3. You're done!

## Example
```html
<script src="angular.min.js"></script>
<script scr="livi18n.min.js"></script>
<script src="ngLivi18n.js"></script>
<script>
    var myApp = angular.module('myApp', ['ngLivi18n']);
    myApp.controller('MyCtrl', function($scope, $livi18n) {
        // Translate
        $livi18n.t(options);

        // Pluralize
        $livi18n.p(options);
        
        // Require
        $livi18n.require(function(t, p) {
            //
        });
    });
</script>
``` 