# Robots look at your app

```html
<!DOCTYPE html> 
<html>
  <head> 🔭🤖
    <meta charset="utf-8">
    <title>AppTemplate</title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link integrity="" rel="stylesheet" href="/@embroider/core/vendor.css">
    <link integrity="" rel="stylesheet" href="/assets/fancy-app.css">
  </head>
  <body>
    <script src="/@embroider/core/vendor.js"></script>
    <script src="/@embroider/core/entrypoint" type="module"></script>
  </body>
</html>

```

Note:

You can think of the rollup as a robot that is looking at your app, but starting from a top-level entry point like a html file. It starts at the top and keeps going until it finds some sort of file that it knows it needs to deal with.
