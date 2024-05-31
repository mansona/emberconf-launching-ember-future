# Rocking the boat

<video controls data-autoplay loop muted playsinline style="height: 500px;" src="/big-house-of-cards.webm"></video> <!-- .element style="height: 550px; margin-top: 50px" -->

Thing 1: What Embroider is doing
<!-- .element style="position: absolute; bottom: -100px; left: 0; font-size: 60%; color: grey;" -->

Note:

This is how I imagine Ed writing the v2 addon spec

The v2 spec isn’t formalising the old way of doing things, it’s actually specifying how to write a new kind of ember-addon that still integrates strongly into your ember app (we’re not talking about dropping down into a normal npm package that you need to use “manually” like some of the other ecosystems), but it no longer strongly integrates into your build system. 

If all our addons moved over to v1 this goes most of the way towards being able to fully statically analyse all the modules in your app and addons like the “perfect” ESM situation I described earlier. 

This was important to get out there as a spec because it means that a bunch of the popular addons could move to this new format and it solves a lot of embroider’s translation woes. But this also gave Embroider a great format to target as part of the translation.