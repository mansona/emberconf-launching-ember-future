# Robots load files

```js
// app/app.js
import Application from '@ember/application'; 🔭🤖
```

```js
const rewritten_packages = '/path/to/your/repo/node_modules/.embroider/rewritten-packages';

function mySuperPlugin(options) {
  return {
    name: 'my-super-plugin', 
		
    async load(id) {
      if (id === `${rewritten_packages}/ember_source/dist/application.js`) {
        return `export default class Application {}`;
      }
    }
  }
}
```

Note:

The same sort of process happens with the load hook, but instead of thinking of it as the right hand side of an import statement that you can influence, it’s more about what the contents of that file are when you read that file. If you’re trying to refer to a real file in a package somehwere you probabely don’t need this. But we currently make heavy use of this concept when we try to load “virtual files”. I’ll tell you more bout this later.