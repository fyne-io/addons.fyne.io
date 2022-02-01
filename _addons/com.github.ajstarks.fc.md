---
id: com.github.ajstarks.fc

title: fc
home: https://github.com/ajstarks/fc
image: https://github.com/ajstarks/fc/raw/master/hw.png
screenshots:
- url: https://github.com/ajstarks/fc/blob/master/presentation/images/mondrian.png?raw=true
- url: https://github.com/ajstarks/fc/blob/master/presentation/images/confetti.png?raw=true
- url: https://github.com/ajstarks/fc/blob/master/presentation/images/fcdeck5.png?raw=true

date:      2022-02-01 00:50:00
excerpt:   High-level canvas for the fyne toolkit
category:  widgets
developer: Anthony Starks

git: https://github.com/ajstarks/fc.git
package: github.com/ajstarks/fc
version: 
---

There are methods for Text (begin, centered, and end aligned), Circles, Lines, Rectangles, and Images.

## Code
```go
fc.NewCanvas(name string, w, h int) Canvas
```

### Percent coordinate based methods

```go
	(canvas *Canvas) EndRun()
	(canvas *Canvas) Text(x, y float64, size float64, s string, color color.RGBA)
	(canvas *Canvas) CText(x, y float64, size float64, s string, color color.RGBA)
	(canvas *Canvas) EText(x, y float64, size float64, s string, color color.RGBA)
	(canvas *Canvas) Circle(x, y, r float64, color color.RGBA)
	(canvas *Canvas) Line(x1, y1, x2, y2, size float64, color color.RGBA)
	(canvas *Canvas) Rect(x, y, w, h float64, color color.RGBA)
	(canvas *Canvas) CornerRect(x, y, w, h float64, color color.RGBA)
	(canvas *Canvas) Image(x, y float64, w, h int, name string)
```

### Absolute methods: uses absolute coordinate system and fyne structures directly

```go
	func AbsStart(name string, w, h int) (fyne.Window, *fyne.Container)
	func AbsEnd(window fyne.Window, content *fyne.Container, w, h int) 
	func AbsText(c *fyne.Container, x, y int, s string, size int, color color.RGBA)
	func AbsTextMid(c *fyne.Container, x, y int, s string, size int, color color.RGBA)
	func AbsTextEnd(c *fyne.Container, x, y int, s string, size int, color color.RGBA)
	func AbsLine(c *fyne.Container, x1, y1, x2, y2 int, size float32, color color.RGBA)
	func AbsCircle(c *fyne.Container, x, y, r int, color color.RGBA)
	func AbsCornerRect(c *fyne.Container, x, y, w, h int, color color.RGBA)
	func AbsRect(c *fyne.Container, x, y, w, h int, color color.RGBA)
	func AbsImage(c *fyne.Container, x, y, w, h int, name string)
	func AbsCornerImage(c *fyne.Container, x, y, w, h int, name string)
```
