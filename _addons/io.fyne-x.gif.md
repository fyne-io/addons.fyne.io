---
id: io.fyne-x.map

title: Animated Gif
home: https://github.com/fyne-io/fyne-x
image: https://github.com/fyne-io/fyne-x/raw/master/img/gifwidget.gif
screenshots:

date:      2023-04-11 20:52:00
excerpt:   Embedding animated Gif images in your Fyne app
category:  widgets
developer: The Fyne-x Team

git: https://github.com/fyne-io/fyne-x.git
package: fyne.io/x/fyne/widget
version: 
---

The default Fyne image widgets only show the first frame of a gif image.
This widget allows you to start and stop the animation through all the frames.

### Code

```go
gif, err := NewAnimatedGif(storage.NewFileURI("./testdata/gif/earth.gif"))
gif.Start()
```
