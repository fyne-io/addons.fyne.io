---
addonid: org.limafresh.messagebubble

title: messagebubble
home: https://github.com/limafresh/messagebubble
icon: https://raw.githubusercontent.com/limafresh/messagebubble/main/demo.gif
screenshots:
- url: https://raw.githubusercontent.com/limafresh/messagebubble/main/demo.gif

date:      2026-04-21 07:56:43
updated:   2026-04-23 17:27:00
excerpt:   Modern message bubble widget
category:  widgets
developer: limafresh

git: https://github.com/limafresh/messagebubble
package: github.com/limafresh/messagebubble/v3
version:
layout: "addon"
---

Modern, customizable and adaptive message bubble widget. You can set different colors for the light and dark themes, and they will update automatically when you change the theme. It also supports text selection, which is probably important for any chat.

### Code

```go
bubble := messagebubble.NewMessageBubble(
	"Alex", // sender's name
	"Hi, how are you?", // message text
	"13:36", // sending time
	false, // mine: true, other: false
)
```
