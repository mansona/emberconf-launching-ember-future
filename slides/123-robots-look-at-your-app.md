# Robots look at your app

```html
<!DOCTYPE html> 
<html>
  <head>
    <meta charset="utf-8"> 
    <title>AppTemplate</title>
    <meta name="description" content="">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link integrity="" rel="stylesheet" href="/@embroider/core/vendor.css">
    <link integrity="" rel="stylesheet" href="/assets/fancy-app.css">
  </head>
  <body>
    <script src="/@embroider/core/vendor.js"></script>
    <script src="/@embroider/core/entrypoint" type="module"></script> 🔭🤖
  </body>
</html>

```

Note:

Skipping ahead a bit we get to your entry point JavaScript file. It can see that the file exists on disk so it is a dutiful little robot and starts loading that file starting at the top and working down through it line by line.
