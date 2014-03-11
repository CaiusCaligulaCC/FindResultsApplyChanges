Original package can be installed via **[Sublime Text 3+](http://www.sublimetext.com/) Package**. Install via an updated version of  [Package Control 2+](https://sublime.wbond.net/installation).
This has to be installed manually by placing the folder into Packages/.

# Find Results Apply Changes

## Description

Apply any change you made to a "Find Results" buffer back to the files. ie:
- Search for "foo" in a folder.
- This will open a "Find Results" buffer listing all the files with "foo" in it.
- Change the instances of "foo" for "bar" or something else...
- Go to the -> Main menubar -> "Find" -> "Find Results - Apply Changes"
- This will write all the changes made back to the files.
- Will be enabled only if the focused view is the "Find Results" tab.

## Bugs

- Uses regions to allow you do multiline changes, but when inserting new newlines, will corrupt files **if you commit more than once**, this because the new newlines will shift the line numbers. Will also 'corrupt' files if you add/remove newlines in other instances of the modified files. eg in another tab. To prevent corruption this packages will alert you and prevent most of these.

## Possible features

- Hook CTRL/CMD+S to apply the changes (how to?)
- Double click in these lines with numbers and a colon will open the file, default ST behaviour(how to disable it?)

## Encoding

If encoding is different, tries to convert the encoding of a non-utf-8-file to utf-8 first and then apply the changes again.

## Source-code

https://github.com/SublimeText/FindResultsApplyChanges

## Forum Thread

http://www.sublimetext.com/forum/viewtopic.php?f=6&t=14118
