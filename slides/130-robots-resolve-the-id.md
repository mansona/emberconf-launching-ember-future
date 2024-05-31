# Robots resolve the ID

```js
function mySuperPlugin(options) {
  return {
    name: 'my-super-plugin', 
		
    async resolveId(source, importer, options) {
      console.log(source === '@ember/application'); // true
      console.log(importer === '/path/to/your/repo/app/app.js'); // true
    }
  }
}
```

Note:

The resolveId hook in all your rollup plugins are called and each of them are given a chance to influence your build, and maybe change what this line means!

If the resolveId hook retuns nothing that plugin hasn’t change anything, but you could if you wanted to return a different answer, essentially redirecting that import to somewhere else. 