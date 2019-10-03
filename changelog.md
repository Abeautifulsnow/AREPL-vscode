## [v1.0.19](https://github.com/Almenon/AREPL-vscode/milestone/37?closed=1) (??/??/2019) 🔧

🔧 Changed filepath for temporary files to current workspace root
🔧 UI change: Variables section is now titled "Variables"

## [v1.0.18](https://github.com/Almenon/AREPL-vscode/milestone/36?closed=1) (09/28/2019) 🚀

🔧 Made print output font monospaced - now it should render output more evenly
🐛 Fixed error with infinite generators - thanks @purpledot!
🐛 Fixed python 2 error message not showing up on linux

## [v1.0.16](https://github.com/Almenon/AREPL-vscode/milestone/35?closed=1) (06/30/2019) 🚀

🐛 Fixed Conda env not working whatsoever. Conda will still not work with numpy but you can use it with other stuff now. 

## [v1.0.15](https://github.com/Almenon/AREPL-vscode/milestone/34?closed=1) (06/02/2019) 🚀

🚀 Added icon to launch arepl. Click on the cat to open arepl on the current document. Click on the cat again to close. If you highlight a piece of code arepl will be opened on a new doc with that code.

🚀 Added customCSS setting for custom styling of arepl

🐛 Fixed arepl failing on linux

## [v1.0.14](https://github.com/Almenon/AREPL-vscode/milestone/33?closed=1) (04/18/2019) 🚀

🚀 Added ability to run blocks of code

🚀 Added #$end comment for section where arepl will not auto-run on changes

🚀 Setting changes now take effect instantly (no need to reload arepl)

🐛 Fixed silent spawn error on mac

## [v1.0.13](https://github.com/Almenon/AREPL-vscode/milestone/32?closed=1) (03/23/2019) 🐛

🚀 right click on editor title to launch arepl

🚀 Added cache var. See https://github.com/Almenon/AREPL-vscode/wiki/Caching-data-between-runs

🐛 Fixed vars dissapearing when there is syntax error

🐛 Fixed vars not clearing when using gui library

## [v1.0.12](https://github.com/Almenon/AREPL-vscode/milestone/30?closed=1) (03/17/2019) 🐛

🚀 Reduce arepl bundle size

🔧 Changed turtle setting for much nicer turtle experience

🔧 Added more internal unit tests for less bugs in future releases

🐛 Fixed broken readme links

🐛 Fixed uppercase pip python modules reloading when they shouldnt be

## [v1.0.11](https://github.com/Almenon/AREPL-vscode/milestone/29?closed=1) (03/04/2019) 🐛

🚀 give friendly error message when bad python version

🐛 Fixed time taken flashes when using dump

🐛 Fixed 'C:\Program' is not recognized as an internal or external command, operable program or batch file

🐛 Fixed TypeError: Cannot read property 'setDecorations' of undefined

## [v1.0.10](https://github.com/Almenon/AREPL-vscode/milestone/28?closed=1) (02/19/2019) 🐛

🐛 Fixed stdout/vars persisting across arepl sessions

🐛 Fixed error in telemtry crashing arepl

## [v1.0.9](https://github.com/Almenon/AREPL-vscode/milestone/27?closed=1) (02/17/2019) 🐛

🐛 Variables that before crashed AREPL entirely now just show up as "AREPL could not pickle this object"

🐛 Fixed var output being retained inbetween sessions

🐛 Fixed FileNotFoundError (for real this time)

🚀 python path now supports the ${env:NAME} macro

## [v1.0.8](https://github.com/Almenon/AREPL-vscode/milestone/26?closed=1) (02/05/2019) 🐛

[🔧 Default pythonPath to be same as the python extension's python path](https://github.com/Almenon/AREPL-vscode/issues/170)

[🐛 Fixed FileNotFoundError](https://github.com/Almenon/AREPL-vscode/issues/162)

[🐛 Fixed pandas bug](https://github.com/Almenon/AREPL-vscode/issues/162)

[🐛 Fixed bug with reloading system modules unnecessarily](https://github.com/Almenon/AREPL-vscode/issues/162)

[🐛 Fixed bug with reloading pip modules unnecessarily](https://github.com/Almenon/AREPL-vscode/issues/162)

## [v1.0.7](https://github.com/Almenon/AREPL-vscode/milestone/25?closed=1) (01/22/2019)

[🔧 give better error when control-shift-a is invoked with nothing open](https://github.com/Almenon/AREPL-vscode/issues/159)

[🐛 Fixed python path for dump](https://github.com/Almenon/AREPL-vscode/issues/165)

[🚀 allow ${python.pythonPath} macro in pythonPath](https://github.com/Almenon/AREPL-vscode/issues/161)

## [v1.0.6](https://github.com/Almenon/AREPL-vscode/milestone/24?closed=1) (01/14/2019)
🔧 Changed message you get when python path is misconfigured

🐛 Fixed bug when closing editor with error decorations

## [v1.0.5](https://github.com/Almenon/AREPL-vscode/milestone/23?closed=1) (12/29/2018)
🚀 input() support! Hardcode input like so: standard_input = "hello\\nworld" to be able to use input()

🔧 inline errors icons are now turned on by default - you can turn them off in settings

🔧 AREPL on windows now uses py (C:\\Windows\\py.exe) to launch python

🐛 Fixed bug where inline error icons stayed present when closing arepl

🐛 Fixed bug where items kept on being added to sys.path between runs

## [v1.0.4](https://github.com/Almenon/AREPL-vscode/milestone/22?closed=1) (12/15/2018) 🚀
🚀 pythonPath setting now supports paths relative to the workspace

🚀 Added optional inline error icons - this can be turned on by setting inlineResults setting to true

[howdoi](https://github.com/gleitz/howdoi) integration - install howdoi with pip to be able to call howdoi from arepl. For example
<code>howdoi('calculate fibbonaci in python')</code> will give you a function to calcualate a fibonaci number

## v1.0.3
🚀 ${workspaceFolder} can now be used in pythonPath for pointing to workspace-specific python interpreters

jsonPickle version upgrade w/ slightly better numpy and pandas support

🐛 Fixed bug with linux

## v1.0.2
🐛 Fixed error with using gui

## v1.0.1
🐛 Fixed error on mac due to a filename having the wrong case when packaging extension

## [v1.0.0](https://github.com/Almenon/AREPL-vscode/milestone/16?closed=1)

Fixed: 🐛 
#86 unittest causes arepl to fail silently bug
#101 styling becomes wierd when in certain scenarios bug 
#102  internal error does not show bug
#94  arepl frequently has problems rendering when there is a lot of prints bug

Updated:
#56  use new webview enhancement
#52 Update vscode-extension-telemetry to the latest version 🚀  greenkeeper

## [v1.5](https://github.com/Almenon/AREPL-vscode/milestone/15?closed=1)

fixed #84 #87 #98

AREPL now works with python 3.7

🚀 AREPL now shows stderr (logs, for example) in print output

AREPL will no longer fail silently when help or input is called

## [v1.4](https://github.com/Almenon/AREPL-vscode/milestone/14?closed=1)

### Fixed: 🐛 
dump output does not appear if exception [#91](https://github.com/Almenon/AREPL-vscode/issues/91)

arepl does not update when user changes a imported file [#82](https://github.com/Almenon/AREPL-vscode/issues/82)

Functions no longer appear in variable preview (not much point in showing them and they clutter screen)

## [v1.3](https://github.com/Almenon/AREPL-vscode/milestone/13?closed=1)

### Fixed: 🐛 
arepl would not start if user had no python user packages installed  https://github.com/Almenon/AREPL-vscode/issues/81

### Added: 🚀
ability to execute on keybinding  https://github.com/Almenon/AREPL-vscode/issues/85

## [v1.2](https://github.com/Almenon/AREPL-vscode/milestone/12?closed=1)

### Added: 🚀
Ability to dump local variables and variables at specific points in your program - https://github.com/Almenon/AREPL-vscode/issues/74
Click on errors to google them - https://github.com/Almenon/AREPL-vscode/issues/76

## [v1.1](https://github.com/Almenon/AREPL-vscode/milestone/11?closed=1)

### Added: 🚀
GUI library setting - https://github.com/Almenon/AREPL-vscode/issues/68
default imports - https://github.com/Almenon/AREPL-vscode/issues/67

### Fixed: 🐛 
display of strings - see https://github.com/Almenon/AREPL-vscode/issues/71


## [v1.0](https://github.com/Almenon/AREPL-vscode/milestone/10?closed=1)

### Added: 🚀
Changelog in landing page (see [#58](https://github.com/Almenon/AREPL-vscode/issues/58))

Better landing page with examples (see [#32](https://github.com/Almenon/AREPL-vscode/issues/32))

Better display of variables (see [#63](https://github.com/Almenon/AREPL-vscode/issues/63))

### Fixed:
Relative imports not working (see [#69](https://github.com/Almenon/AREPL-vscode/issues/69))

---

## [v9](https://github.com/Almenon/AREPL-vscode/milestone/9?closed=1)

### Added: 🚀
Added telemetry (see [#50](https://github.com/Almenon/AREPL-vscode/issues/51)).
This is optional and can be turned off in the settings.

Having this turned on helps me analyze how many users I have, what settings are useful to them, and how frequently they use AREPL. It also reports internal errors with AREPL backend to help diagnose bugs.

### Fixed:
Exception stacktrace used to include internal AREPL stacktrace - now the stacktrace only shows info relative to your code (see [#51](https://github.com/Almenon/AREPL-vscode/issues/51))

---

## v8

Fixed too many prints slowing or freezing the preview.  See [#37](https://github.com/Almenon/AREPL-vscode/issues/37)

## v7

Fixing case issue causing error in linux systems

## v6

see https://github.com/Almenon/AREPL-vscode/milestone/6?closed=1

Fixed #47 new arepl session command fails when user does not have doc open

Implemented #33 footer bar with feedback links

## v5:

see https://github.com/Almenon/AREPL-vscode/milestone/5

### Added: 🚀
* Setting to skip landing page
* Setting for print results at top
* Command to execute highlighted code in AREPL
* command for creating new file
* allow user to customize pythonPath and pythonOptions
* allow user to execute on save

## Fixed:
* timing is not sticky
