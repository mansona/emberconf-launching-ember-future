# Webpack with added Broccoli

![webpack](/webpack.svg) <!-- .element style="height: 165px;" --> 🥦 🫠

<!-- .element style="font-size: 400%" -->


Thing 1: What Embroider is doing
<!-- .element style="position: absolute; bottom: -100px; left: 0; font-size: 60%; color: grey;" -->

Note:

This is kinda hard to understand, and if you look at the code that handles this you can see that it’s reaching deep into Webpack’s internals and mucking around with things in complex and hard to understand ways. Webpack’s api doesn’t make this easy for us but we’re not even following Webpack’s best practices here.

There is a better way! We call it inversion of control in the Embroider team, but to understand it we need to teach you a little background on bundlers