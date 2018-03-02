# cordova-plugin-appinfo

console.log('identifier: %s', navigator.appInfo.identifier);
console.log('version: %s', navigator.appInfo.version);
console.log('build: %s', navigator.appInfo.build);
```

Before version 2.1, the information had to be accessed through
asynchronously. This is no longer needed, but the old method
shown below will be kept for backwards compatibility:

```js
navigator.appInfo.getAppInfo(function(appInfo) {
  console.log('identifier: %s', appInfo.identifier);
  console.log('version: %s', appInfo.version);
  console.log('build: %s', appInfo.build);
}, function(err) {
	alert(err);
});
```

### Contributing

Pull requests are welcome.

* @thomas-mullaly added the WP8 implementation
* @yezhiming added functionality to get identifier and build.
* @jcesarmobile added synchronous implementation

