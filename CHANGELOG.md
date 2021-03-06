## HEAD

## 0.25

* Fixed a regression in the handling of the 'cw' command
* Made the replace operator work with multiple cursors

## 0.24

* Fixed the position of the cursor after certain yank operations.
* Fixed an issue where duplicate vim states were created when an editors were
  moved to different panes.

## 0.23

* Made motions, operators and text-objects work properly in the
  presence of multiple cursors.

## 0.22

* Fixed a stylesheet issue that caused visual glitches when vim-mode
  was disabled with the Shadow DOM turned on.

## 0.21

* Fix issue where search panel was not removed properly
* Updated the stylesheet for compatibility with shadow-DOM-enabled editors

## 0.20
* Ctrl-w for delete-to-beginning-of-word in insert mode
* Folding key-bindings
* Remove more deprecated APIs

## 0.19.1
* Fix behavior of ctrl-D, ctrl-U @anvyzhang
* Fix selection when moving up or down in visual line mode @mdp
* Remove deprecated APIs
* Fix interaction with autocomplete

## 0.19
* Properly re-enable editor input after disabling vim-mode

## 0.17
* Fix typo

## 0.16
* Make go-to-line motions work with operators @gittyupagain
* Allow replacing text with newlines using `r` @dcalhoun
* Support smart-case in when searching @isaachess

## 0.14
* Ctrl-c for command mode on mac only @sgtpepper43
* Add css to status bar mode for optional custom styling @e-jigsaw
* Implement `-`, `+`, and `enter` @roryokane
* Fix problem undo'ing in insert mode @bhuga
* Remove use of deprecated APIs

## 0.11.1
* Fix interaction with autocomplete-plus @klorenz

## 0.11.0
* Fix `gg` and `G` in visual mode @cadwallion
* Implement `%` @carlosdcastillo
* Add ctags keybindings @tmm1
* Fix tracking of marks when buffer changes @carlosdcastillo
* Fix off-by-one error for characterwise puts @carlosdcastillo
* Add support for undo and repeat to typing operations @bhuga
* Fix keybindings for some OSes @mcnicholls
* Fix visual `ngg` @tony612
* Implement i{, i(, and i" @carlosdcastillo
* Fix off by one errors while selecting with j and k @fotanus
* Implement 'desired cursor column' behavior @iamjwc

## 0.10.0
* Fix E in visual mode @tony612
* Implement `` @guanlun
* Fix broken behavior when enabling/disabling @cadwallion
* Enable search in visual mode @romankuznietsov
* Fix end-of-line movement @abijr
* Fix behavior of change current line `cc` in various corner cases. @jcurtis
* Fix some corner cases of `w` @abijr
* Don't hide cursor in visual mode @dyross

## 0.9.0 - Lots of new features
* Enable arrow keys in visual mode @fholgado
* Additional bindings for split pane movement @zenhob
* Fix search on invalid regex @bhuga
* Add `s` alias to visual mode @tony612
* Display current mode in the status bar @gblock0
* Add marks (m, `, ') @danzimm
* Add operator-pending mode and a single text object (`iw`) @nathansobo, @jroes
* Add an option to start in insert mode @viveksjain
* Fix weird behavior when pasting at the end of a file @msvbg
* More fixes for corner cases in paste behavior @SKAhack
* Implement * and # @roman
* Implement ~ @badunk
* Implement t and T @udp

## 0.8.1 - Small goodies
* Implement `ctrl-e` and `ctrl-y` @dougblack
* Implement `/`, `?`, `n` and `N` @bhuga
* Registers are now shared between tabs in a single atom window @bhuga
* Show cursor only in focused editor @tony612
* Docs updated with new methods for entering insert mode @tednaleid
* Implement `r` @bhuga
* Fix `w` when on the last word of a file @dougblack
* Implement `=` @ciarand
* Implement `E` motion @tony612
* Implement basic `ctrl-f` and `ctrl-b` support @ciarand
* Added `+`, `*` and `%` registers @cschneid
* Improved `^` movement when already at the first character @zenhob
* Fix off-by-one error for `15gg` @tony612

## 0.8.0 - Keep rocking
* API Fixes for Atom 0.62 @bhuga
* Add `$` and `^` to visual mode @spyc3r
* Add `0` to visual mode @ruedap
* Fix for yanking entire lines @chadkouse
* Add `X` operator @ruedap
* Add `W` and `B` motions @jcurtis
* Prevent cursor left at column 0 when switching to insert mode @adrianolaru
* Add pane switching shortcuts see #104 for details @dougblack
* Add `H`, `L` and `M` motions @dougblack

## 0.7.2 - Full steam ahead
* Leaving insert mode always moves cursor left @joefiorini
* Implemented `I` command @dysfunction
* Restored `0` motion @jroes
* Implemented `}` motion to move to previous paragraph @zenhob
* Implement `gt` and `gT` to cycle through tabs @JosephKu
* Implement visual linewise mode @eoinkelly
* Properly clear selection when return to command mode @chadkouse

## 0.7.1 - User improvements
* `ctrl-[` now activates command mode @ctbarna
* enter now moves down a line in command mode @ctbarna
* Documentation links now work on atom.io @michaeltwofish
* Backspace now moves back a space in command mode @Tarrant
* Fixed an issue where cursors wouldn't appear in the settings view.

## 0.7.0 - Updates for release
* Update contributing guide
* Update package.json
* Require underscore-plus directly

## 0.6.0 - Updates
* Implemented `.` operator, thanks to @bhuga
* Fix putting at the end of lines, thanks to @bhuga
* Compatibility with Atom 0.50.0

## 0.5.0 - Updates
* Switches apm db to buttant from iriscouch

## 0.4.0 - Updates
* Compatibilty with Atom 26

## 0.3.0 - Visual and Collaborative
* Compatiblity with atom 0.21
* Characterwise visual-mode!
* System copy and paste are now linked to the `*`
* Implement `A` operator
* Bugfixes concerning `b` and `P`

## 0.2.3 - Not solo anymore

* Major refactoring/cleanup/test speedup.
* Added `S` command.
* Added `C` operator.
* Proper undo/redo transactions for repeated commands.
* Enhance `G` to take line numbers.
* Added `Y` operator.
* Added `ctrl-c` to enter command mode.

## 0.2.2

* Added `s` command.
* Added `e` motion.
* Fixed `cw` removing trailing whitepsace
* Fixed cursor position for `dd` when deleting blank lines

## 0.2.1

* Added the `c` operator (thanks Yosef!)
* Cursor appears as block in command mode and blinks when inserting (thanks Corey!)
* Delete operations now save deleted text to the default buffer
* Implement `gg` and `G` motions
* Implement `P` operator
* Implement `o` and `O` commands

## 0.2.0

* Added yank and put command with support for registers
* Added `$` and `^` motions
* Fixed repeats for commands and motions, ie `d2d` works as expected.
* Implemented `D` to delete through the end of the line.
* Implemented `>>` and `<<` indent and outdent commands.
* Implemented `J`.
* Implemented `a` to move cursor and enter insert mode.
* Add basic scrolling using `ctrl-u` and `ctrl-d`.
* Add basic undo/redo using `u` and `ctrl-r`. This needs to be improved so it
  understands vim's semantics.

## 0.1.0

* Nothing changed, used this as a test release to understand the
  publishing flow.

## 0.0.1

* Initial release, somewhat functional but missing many things.
