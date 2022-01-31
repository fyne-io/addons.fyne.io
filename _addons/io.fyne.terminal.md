---
id: io.fyne.terminal
requires: linux,darwin,windows

title: Terminal
home: https://github.com/fyne-io/terminal
image: https://github.com/fyne-io/terminal/raw/master/img/linux.png
screenshots:
- url: https://github.com/fyne-io/terminal/raw/master/img/linux.png
- url: https://github.com/fyne-io/terminal/raw/master/img/macos.png
- url: https://github.com/fyne-io/terminal/raw/master/img/windows.png

date:      2022-01-31 23:19:00
excerpt:   A terminal widget for use in shells or remote consoles
category:  widgets
developer: The Fyne Team

git: https://github.com/fyne-io/terminal.git
package: github.com/fyne-io/terminal
version: 
---

This terminal widget allows you to simply drop a command line terminal into your app,
useful for embedded command lines or remote terminals.

Currently supports Linux, macOS and Windows with more platforms to follow.

### Code

```go
t := Terminal.New()
```
