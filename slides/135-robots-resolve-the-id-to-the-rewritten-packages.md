# Robots resolves rewritten packages

```js
const rewritten_packages = '/path/to/your/repo/node_modules/.embroider/rewritten-packages';

function mySuperPlugin(options) {
  return {
    name: 'my-super-plugin', 
		
    async resolveId(source, importer, options) {
      if (source === '@ember/application') {
        return `${rewritten_packages}/ember_source/dist/application.js`;
      }
    }
  }
}
```

Note:

This example is a vast over-simplification of what is going on but we're on a crash course here and it's a good enough mental model. Looking at this slide it is a bit of an exestensial crisis that all the work that we've been doing in Embroider for the past year could be conceptually thought of as a long list of really complicated if statements. But I guess that's true for all software since that's what a turing machine is, but anyway! 

Lets not get distracted!!!