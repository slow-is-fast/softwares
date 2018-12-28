# Sublime Text 3

## Reason to Choose Sublime Text over Emacs/Vim
- Beautiful UI
- Simple Learning Curve


## Features
- Command Palette
- Go To Anything
- Multiple cursors
- Snippets(especially your customized snippets)
- Minimap
- shortcuts(of course)


## CLI setup
> ln –s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl

## The Data directory
### Location
The location of theData directory is platform-dependent:
- Windows: %APPDATA%\Sublime Text 3
- OS X: ~/Library/Application Support/Sublime Text 3
- Linux: ~/.config/sublime-text-3

### Directory brief
We should see at least three directories inside the Data directory:
- Installed Packages: 
	This contains a copy of every sublime-packageinstalled. It's used to restore packages.
- Local: 
	This stores all the information about our current and previous session. This is used to restore Sublime to the stage we were in, when we last quit Sublime.
- Packages: 
	This contains all package folders that Sublime will load


## packages, plugins, snippets, and macros


## Plugins 

- AdvancedNewFile
- Alignment
- All Autocomplete
- BracketHighlighter
- Github Color Theme
- Inspired GitHub Color Scheme
- PHP Companion
- Package Control
- SublimeLinter-php
- SublimeLinter

## Custom Snippets


## Config

``` javascript
{
	"always_show_minimap_viewport": true,
	"color_scheme": "Packages/Github Color Theme/GitHub.tmTheme",
	"font_size": 18,
	"highlight_line": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"line_padding_bottom": 5,
	"line_padding_top": 5,
	"rulers":
	[
		80,
		100
	],
	"theme": "Default.sublime-theme"
}
```


## Color Themes
recommended by Dan Bader

- default
- SoDaReloaded Theme + Tomorrow Night Scheme
- Predawn Theme
- Material Nil Theme
- Boxy Theme
- Seti UI Theme + Seti UX Scheme