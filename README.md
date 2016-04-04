# equalHeights
equalHeights is a jQuery plugin to make bootstrap pod-like elements to have the same height.
### Use
First of all you have to include the css file inside `<head>` tag.
```<link rel="stylesheet" href="css/equal-height.css" />```

Inlcude also the js file at the bottom of `<body>` and after jquery is incuded.
```<script src="js/equal-heights.js"></script>```

In order to use equalheights with it's default options you simply have to add the class `pods-container` to the row element and the `pod` class to every column element. You'll also need to have a div with class `content`.
```
  <div class="row pods-container">
    <div class="pod col-md-3 col-sm-6">
        <div class="content">
            ...
        </div>
    </div>
    <div class="pod col-md-3 col-sm-6">
        <div class="content">
            ...
        </div>
    </div>
    <div class="pod col-md-3 col-sm-6">
        <div class="content">
            ...
        </div>
    </div>
    <div class="pod col-md-3 col-sm-6">
        <div class="content">
            ...
        </div>
    </div>
  </div>
```
### Options
```
$('.pods-container').equalHeights({
    'container' : '.pods-container',
    'equalElements': '.pod',
    'vw': '480'
  });
```
As you can see you can add your own options in order to use the plugin in your way.
`container` defaults to `.pods-container`, is the container class of the pods.
`equalElements` defaults to `.pod`, is the class added to the elements we want to have the same height.
`vw` defaults to `768`, is the view port width we want to stop the plugin from running.

The plugin runs on the resize event of the window also.

  
