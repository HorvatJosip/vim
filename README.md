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