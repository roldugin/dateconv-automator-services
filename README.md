# Mac OS X Services for date conversion

Automator Services that convert and replace selected text in any editable field with a UTC timestamp:
- `Convert Date to ISO 8601` will convert into a UTC date in ISO 8601 format (e.g. `2016-04-07T06:10:00+00:00`)
- `Convert Date to Milliseconds` will convert into milliseconds since UNIX Epoch (e.g. `1460009400000`)

## Accepted input

- Freeform datetime string (`7 Apr, 2016 6:10:00.001am` and many others)
- ISO 8601 (`2016-04-07T06:10:00.001`, `2016-04-07T06:10:00.001Z`, `2016-04-07T16:10:00.001+10:00`)
- Seconds since UNIX Epoch (`1460009400`)
- Milliseconds since UNIX Epoch (`1460009400001`)

## Installation

```
svn checkout https://github.com/roldugin/dateconv-automator-services/trunk/Convert\ Date\ to\ ISO\ 8601.workflow ~/Library/Services/Convert\ Date\ to\ ISO\ 8601.workflow
svn checkout https://github.com/roldugin/dateconv-automator-services/trunk/Convert\ Date\ to\ Milliseconds.workflow ~/Library/Services/Convert\ Date\ to\ Milliseconds.workflow
```

## Usage example

1. Select a date in any editor or editable field
2. Choose `Application Menu (e.g. Chrome) -> Services -> Convert Date to ISO 8601`
3. If the text is detected as date/time, it will be replaced with an equivalent UTC timestamp in ISO 8601 format (e.g. `2016-04-07T06:10:00+00:00`)

## Keyboard shortcuts

I have been using the following mappings without clashes so far:
- Convert Date to ISO 8601 `⌥⇧⌘I`
- Convert Date to Milliseconds `⌥⇧⌘M`
