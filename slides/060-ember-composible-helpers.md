# ember-composible-helpers

- pick of composable helpers

Note:

The easiest example I can think of is ember-composible-helpers. Now this is not calling out a bad design by the way. Docyard actually went above and beyond when they divined through the ember-cli addon api and figured out a decent way to allow you to prune unused helpers from your build, but those sorts of microoptimisations were symptoms of needing to deal with the madness of ember-cli

Not long into the history of embroider Ed realised that the real problem were the addons. The addon api was a mish mash of things that had grown over the years and nobody had sat down to write a specification that described what an addon can or can’t do, and if we wanted to change anything we sure need a spec for the v2 