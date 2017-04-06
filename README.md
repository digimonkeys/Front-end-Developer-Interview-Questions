
* How do you reset a $timeout, $interval(), and disable a $watch()?  
To reset a timeout and/or $interval, assign the result of the function to a variable and then call the .cancel() function on this variable. To disable $watch(), we call it.  

```
var customTimeout = $timeout(function () {
// arbitrary code 
}, 55);
$timeout.cancel(customTimeout);
var deregisterWatchFn = $rootScope.$watch(‘someGloballyAvailableProperty’, function (newVal) {
if (newVal) {
// we invoke that deregistration function, to disable the watch
deregisterWatchFn();
...
}
});
```
