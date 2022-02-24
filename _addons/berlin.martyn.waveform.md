---
id: berlin.martyn.waveform

title: waveform
home: https://musings.martyn.berlin
image: https://cdn.discordapp.com/attachments/837686172494725160/941765851919564911/unknown.png
screenshots:
- url: https://cdn.discordapp.com/attachments/837686172494725160/941765851919564911/unknown.png

date:      2022-02-24 20:10:00
excerpt:   Audio waveform display component
category:  widgets
developer: Martyn Ranyard

git: https://git.martyn.berlin/martyn/fyne-widgets
package: git.martyn.berlin/martyn/fyne-widgets/pkg/waveform
version:
---

A little widget for displaying a recorded waveform.

Expects a slice of int32 samples, and displays them in a familiar way. Doesn't "curve" the waveform, simply plots it.

Can just display data 1 sample per pixel or resample data (uses `disintegration/imaging` to do nearest neighbour image resampling) to the width of the widget.

Default is themable, Colors are overridable. Background can be removed or not.

