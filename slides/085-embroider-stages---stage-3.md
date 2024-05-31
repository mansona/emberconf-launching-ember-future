# Embroider Stages - stage 3

- Stage 1 - rewrite all your addons into v2 
- Stage 2 - rewrite your app
- Stage 3 - pass to the packager

Thing 1: What Embroider is doing
<!-- .element style="position: absolute; bottom: -100px; left: 0; font-size: 60%; color: grey;" -->

Note:

Stage 3 - pass to the packager

The third stage could be conceptually thought of as just pointing your packager at these combinations of rewritten classic addons, rewritten app and all the other non classic ember addon packages you have in your dependencies. There should be no broccoli involved in an ideal world but unfortunately in the current stable version of Embroider, this pointing of the packager at your app happens in a broccoli tree 