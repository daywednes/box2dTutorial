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

# The basics

* We built an HTML5 game -- [Agent 8 Ball](http://agent8ball.com). We wanted it to have cool physics.
* We took an existing javascript library - Box2d - and made it our own. http://github.com/thinkpixellab/box2d
* We created a demo site - http://box2d.heroku.com/ - and opened the source to it here - http://github.com/thinkpixellab/box2dWeb
* Now we're going to give you a walk through of how to build your own app using Box2d.
