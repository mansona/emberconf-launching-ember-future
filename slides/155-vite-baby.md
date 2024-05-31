# Vite baby!

![vite](/vite.png)

Note:

Vite is the dream for Ember for so many reasons. If we were able to run an Ember app on Vite our rebuild speed would be incredible. Vite is able to keep track of each of the modules that your app loads and if you change something it doesn’t need to rebuild and reprocess all the modules that didn’t change. So if you have a build cost for processing your files you only need to pay it for modules that have changed. 

But we have one problem. The current rewritten app model really confuses Vite for a number of different reasons. If anyone is interested in what those reasons are come find me after the talk and I’ll be happy to go into the gory details! So we need to stop relying on the rewritten app and point vite at your source files.

This means that we need to implement all the things that we were relying on the rewritten app for slightly differently. Some changes that have already landed for example we used to build your entrypoint JS as part of the stage 2 app rewriting, but now we don’t do that. We used to inject all this strange stuff into your index.html in the rewritten app. Now we don't do that