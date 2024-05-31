# Robots look at your app.js

```js
// app/app.js
import Application from '@ember/application'; 🔭🤖
import Resolver from 'ember-resolver';
import loadInitializers from 'ember-load-initializers';
import config from 'fancy-app/config/environment';

export default class App extends Application {
  modulePrefix = config.modulePrefix;
  podModulePrefix = config.podModulePrefix;
  Resolver = Resolver;
}

loadInitializers(App, config.modulePrefix);
```

Note:

I’m going to show the app.js file because this is hopefully going to be the first file that rollup will see when the current work on main is done

When it sees a line like this at the top of a javascript it has to do two things, resolve where that is coming from and then load the contents of the file.