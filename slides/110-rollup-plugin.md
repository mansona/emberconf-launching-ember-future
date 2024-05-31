# Rollup Plugin

```js
function mySuperPlugin(options) {
  return {
    name: 'my-super-plugin', 
		
    async resolveId(source, importer, options) { // <- this is a hook
      // TODO do stuff
    }
  }
}
```

Note:

how it rolls up your app into a bundle is defined by a bunch of plugins. Plugins have a  number of hooks that can “do things” in your build at certain times as rollup is lookig at your app

This resolveId function is the hook that I'm talking about