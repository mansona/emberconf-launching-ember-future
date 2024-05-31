# House of cards

<video controls data-autoplay loop muted playsinline style="height: 500px;" src="/house-of-cards.webm"></video> <!-- .element style="height: 550px; margin-top: 50px" -->

Thing 1: What Embroider is doing
<!-- .element style="position: absolute; bottom: -100px; left: 0; font-size: 60%; color: grey;" -->

Note:

I don’t know the the first feature that influenced the initial concept of Embroider, but one big thing that started to be talked about in the post-ESM era of JavaScript was tree shaking and route splitting. Now that you could effectively describe the the whole graph of files that an entry point imported, you can just use a smart bundle and only include those files in your output bundle. But remember that complex layering that ember-cli was doing, that would of course prevent us from easily enabling these more modern techniques. 

Enter embroider