# v2 addon spec

This is a slide!

Note:

So enter the v2 addon spec. This isn’t formalising the old way of doing things, it’s actually specifying how to write a new kind of ember-addon that still integrates strongly into your ember app (we’re not talking about dropping down into a normal npm package that you need to use “manually” like some of the other ecosystems), but it no longer strongly integrates into your build system. This goes 90% of the way towards being able to fully statically analyse all the modules in your addon like the “perfect” ESM situation I described earlier. 

This was important to get out there as a spec because it means that a bunch of the popular addons could move to this new format and it solves a lot of embroider’s translation woes. But this also gave Embroider a great format to target as part of the translation.