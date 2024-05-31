# Stop the clock

- Stop the clock! 

Note:

How did I do? A bit more than 2 minutes, and how many people have at least a better understanding of rollup plugins now? 

So what can we use this resolveId hook for then, well remember i said that we rewrote your classic addons? Well in your app.js when you come across an import for something that has been rewritten we change it from what rollup would normally finde, to the rewritten version in your node_modules/.embroider/rewritten_packages folder. And how do we know which one we should rewrite to? Well the resolveID knows what file the import is in and when we were rewriting all your addons we kept track of which package should see which version of the rewritten addon. That’s all tracked in the resolver.json in the .embroider folder. 