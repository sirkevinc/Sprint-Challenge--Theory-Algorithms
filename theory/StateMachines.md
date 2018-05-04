The VT-100 terminal (console) outputs text to the screen as it receives it over the wire. One exception is that when it receives an ESC character (ASCII 27), it goes into a special mode where it looks for commands to change its behavior.

`ESC[12;45f`

`ESC[1m`

Come up with regexes for the two above sequences. The one to set the cursor position should accept any digits for the row and column. The bold sequence need only accept `1` (and is a trivial regex). (ESC is a single character which can be represented with `\e` in the regex.)

Cursor position regex: `ESC\[\d*;\d*[a-z]`

Bold regex: `ESC\[1m`