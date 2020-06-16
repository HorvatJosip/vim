# Vim

### Modes

* Normal / Command Mode - browsing - default (name `command mode` is sometimes used because everything you type is interpreted as a command)
* Insert Mode - file editing - enter by using `i`, exit with `ESC`
* Line Mode - performing actions (save, for example) - enter by typing `:`, exit with `ESC` or by executing the command with `Enter`

### Terminal

`vim` [options]

* Running `vim` without specifying anything will just start Vim
* Specifying file as an options will have different outcomes:
  * file exists - it will open it for editing
  * file doesn't exist - it will create it and open it for editing

### Actions

> Line Mode executable actions which start with `:`

* `q` (quit) - quits out of the editor
* `wq` (write & quit) - writes changes to the file and quits the editor
* `$` - go to end of the file
* <n> - go to line <n>
* `set <option>` turns the <option> on (for example, `set ruler` will turn on ruler which will show position information at bottom right)
* `set no<option>` turns the <option> off (for example, `set noruler`)
* `set <option>!` toggles the <option> on or off (for example, `set ruler!`)

### Browsing (Command Mode)

Movement

* `h` - move left
* `l` - move right
* `j` - move down (j looks sort of like down arrow or fishing hook that is thrown down into the water)
* `k` - move up
* `Ctrl` + `f` - forward - page down operation
* `Ctrl` + `b` - backward - page up operation
* `w` - word - moves to the start of next word (sequence of non-blank characters)
* `W` - WORD - same as `w`, but ignores punctuation and uses whitespace as word boundaries
* `b` - back - moves back to the start of the current word, or if we are at the start, moves to the start of the previous word
* `B` - BACK - `b`, but with same logic as `W`
* `z` then `Enter` - changes view (position stays the same, but the view will reposition so that the cursor position is near the top - the view position relative to cursor position can be changed in the configuration)
* `0` - moves to the start of the line
* `^` (`AltGr + 3`) - moves to the first character of the line (non-whitespace)
  * In `regex`, this symbol is the opening character
* `$` - moves to the end of the line
  * In `regex`, this symbol is the closing character
* `gg` - go to start of the file
* `G` - go to end of the file
* <n> then `gg` or `G` - go to line <n>
* `Ctrl` + `g` - prints file info ("<File Name>" <n> lines --<Progress In Lines In The File>--)
* `g` then `Ctrl` + `g` - prints more detailed file info

### Other

Single `~` (Tilda) character per row at the end of file - visual indicator to show that the file ends there (it isn't part of the file)