# Same HTML

![diff](/html-diff.webp) <!-- .element style="max-height: 650px;" -->

Note:

All of these embroider/core prefixed locations are virtual files that the Embroider vite plugin (which is just a rollup plugin) loads the content for by defining a load hook. 

There is one other class of thing that we need to deal with as a vite plugin here. You notice the content-for implementation in the index.html, well that used to be something that ember-cli dealt with for us in it’s frantic file laying. Now we have a vite plugin that reads the value that needs to go there from a config file that was output during stage 1. 

This and about a million other little changes to the internal hard parts of Embroider were needed to even get this far and it's worth shouting out some of the reason why we were able to get this far.