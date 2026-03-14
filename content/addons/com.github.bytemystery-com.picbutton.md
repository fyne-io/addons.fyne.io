---
addonid: com.github.bytemystery-com.picbutton

title: PicButton
home: https://github.com/bytemystery-com
icon: https://github.com/bytemystery-com/picbutton/raw/master/example/screenshots/02.png?raw=true
screenshots:
- url: https://github.com/bytemystery-com/picbutton/raw/master/example/screenshots/01.png?raw=true
- url: https://github.com/bytemystery-com/picbutton/raw/master/example/screenshots/02.png?raw=true
- url: https://github.com/bytemystery-com/picbutton/raw/master/example/screenshots/03.png?raw=true

date:      2026-02-04 15:50:00
excerpt:   Implements a button using pictures for the states
category:  widgets
developer: Reiner Pröls

git: https://github.com/bytemystery-com/picbutton.git
package: github.com/bytemystery-com/picbutton
version: v0.2.1
layout: "addon"
---

Implements a button (normal push button or toggle button) with
customer provided pictures for up, down and inactive state
if inactive pictures are missing they will be generated from the provided up and down pictures.
Pictures can be changed on the fly.
You can also specify which mouse button can be used to press / toggle the button.
Also the keyboard keyState and used Mouse button can be retrieved for implementing click + Ctrl
or right click + Shift.
You can also specify if the padding from the theme is used or displaying without a padding.