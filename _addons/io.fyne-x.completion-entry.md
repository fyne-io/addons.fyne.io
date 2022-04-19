---
id: io.fyne-x.completion-entry

title: CompletionEntry
home: https://www.metal3d.org
image: https://github.com/fyne-io/fyne-x/blob/master/img/widget-completion-entry.png?raw=true
screenshots:
- url: https://github.com/fyne-io/fyne-x/raw/master/img/widget-completion-entry.png?raw=true

date:      2022-04-19 09:10:00
excerpt:   Text entry with completion
category:  widgets
developer: Patrice Ferlet

git: https://github.com/fyne-io/fyne-x.git
package: github.com/fyne-io/fyne-x/widget
version: 1.0.0
---

The CompletionEntry is a text entry with a List that is completed when `OnChanged` is triggered.

### Code

```go
entry := widget.NewCompletionEntry([]string{})

// When the use typed text, complete the list.
entry.OnChanged = func(s string) {
    // completion start for text length >= 3
    if len(s) < 3 {
        entry.HideCompletion()
        return
    }

    // Make a search on wikipedia
    resp, err := http.Get(
        "https://en.wikipedia.org/w/api.php?action=opensearch&search=" + entry.Text,
    )
    if err != nil {
        entry.HideCompletion()
        return
    }

    // Get the list of possible completion
    var results [][]string
    json.NewDecoder(resp.Body).Decode(&results)

    // no results
    if len(results) == 0 {
        entry.HideCompletion()
        return
    }

    // then show them
    entry.SetOptions(results[1])
    entry.ShowCompletion()
}
```
