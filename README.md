This is a box2d tutorial.

# Steps

## 0 - Create an empty git repository

* Create a dir. Any dir.
* run `git init` in it

## 1 - Add box2d as a submodule

`git submodule add git://github.com/thinkpixellab/box2d.git box2d`

You should now have a `box2d` directory with a bunch of fun javascript. Right?

## 2 - Add Tools

`git submodule add git://github.com/thinkpixellab/google-closure-tools.git tools`

This adds the python scripts and compiler jar needed to build.mat

## 3 - Add Closure Library

`svn checkout http://closure-library.googlecode.com/svn/trunk/ closure-library`

You'll want to add a `.gitignore` file to `closure-library` to remove a bunch of stuff you don't want.

    .svn
    *.html
    closure/goog/demos

## 4 - Bootstrap your code

Let's get a simple html + js file together.

### index.html
    <html>
    <head>
      <title>Demo!</title>
      <script src="code.js" type="text/javascript" charset="utf-8"></script>
    </head>
    <body>
    </body>
    </html>

### code.js
    alert("Hello, code!");

Do you see an alert? We're good to go!

# The basics

* We built an HTML5 game -- [Agent 8 Ball](http://agent8ball.com). We wanted it to have cool physics.
* We took an existing javascript library - Box2d - and made it our own. http://github.com/thinkpixellab/box2d
* We created a demo site - http://box2d.heroku.com/ - and opened the source to it here - http://github.com/thinkpixellab/box2dWeb
* Now we're going to give you a walk through of how to build your own app using Box2d.
