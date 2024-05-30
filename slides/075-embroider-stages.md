# Embroider Stages

 - stages of embroider

Note:

Enter the 3 stages of an Embroider build

- animate stage 1

Stage 1 - rewrite all your addons into v2 


If anyone is running Embroider you can take a look at this in action in your own repo right now. After you’ve done an embroider build you can look in `node_modules/.embroider/rewritten_packages` and see that there are a bunch of the addons you have installed. This will only list the addons that need to be rewritten, I.e. classic addons. But if you have any reasonably sized app you will notice way more in this folder than you have in your package.json. This is because it needs to rewrite your addons but also any addon dependencies your addons might have. This can cause some strange version differences and not only that there can be same version addons that need different v2 representations based on their broccoli builds. This may seem like a nightmare to keep track of but it’s much easier than trying to support broccoli builds later in the Embroider process.