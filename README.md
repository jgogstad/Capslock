The commit look should be pretty self explanatory, but anyway, here's the fork details:
* Customizations
  * Replaced Karabiner internals for signaling that Caps lock is pressed. Instead of mapping Caps lock
to ⌃⌥⇧⌘, I'm setting an internal variable in Karabiner. This plays nicer with for instance IntelliJ which
gets confused when it sees all those modifier keys
  * Replaced the Bash controls with more window management for SizeUp and TotalSpaces
  * Some minor personal preferences on Shifter (I like it to behave just like shift, e.g. `✱[` should map to `{`)
  * Replaced application shortcuts with applications I use
  * Hyper+Tab `✱↹` simulates Control+Tab `⌃↹` instead of Command+Tab `⌘↹`
* New manipulators:
  * "Disable ⌘H and ⌘⌥H" (after forgetting to push `✱` too many times when reaching for vim-like arrow keys)
  * "Hyper IntelliJ": Use `✱` instead of `⌃` for most commands in IntelliJ

# Capslock

*Make CapsLock Great Again!*  

![](images/trump.jpg)

## Why CapsLock

#### Transform Capslock into hyper key, improve your productivity tremendously!

* Powerful: Make Capslock a great new modifier key: **Hyper(✱)**. 
* Well-Designed:  High-Freq key in hot-area. Bring lots of useful functionalities.
* Compatible: Work well with other modifiers, applications, devices.
* Light-Weight:  Just a small script, carry it everywhere !
* [Design Document](design.md)




## Platforms

- [CapsLock(Mac)](mac/)  via  karabiner-elements
  - macOS High Sierra (10.13)
  - macOS Sierra (10.12)
  - macOS EI Capitan (10.11)


## Install (mac)

1. Download [Karabiner-Elements](https://pqrs.org/osx/karabiner/) and Install

2. Copy URL to your browser to import configuration script.

```bash
# This Repo
karabiner://karabiner/assets/complex_modifications/import?url=https://raw.githubusercontent.com/Vonng/Capslock/master/mac/caps_lock.json

# Karabiner-Elements Official Script Gallery
karabiner://karabiner/assets/complex_modifications/import?url=https%3A%2F%2Fpqrs.org%2Fosx%2Fkarabiner%2Fcomplex_modifications%2Fjson%2Fcaps_lock_enhancement.json
```

3. Open Karabiner, Tab "ComplexModification", Button "Add Item", and enable entries you like.

4. Default conf file path is `$HOME/.config/karabiner/assets/complex_modifications`. Modify it if you like.



## Usage (mac)

![](images/keyboard.png)

### Basic

Hold CapsLock to enable `Hyper` `✱` functionality while press it will emit an `Escape`.

| Origin    | Maps to    | Comment                    |
| --------- | ---------- | -------------------------- |
| `⇪` Press | `⎋` Escape | Single press to escape     |
| `⇪` Hold  | `✱`  Hyper | Enable Hyper Functionality |

### Navigation

- Hold  `✱` Hyper to enable navigators
- Hold additional `⌘` Command for **selection** . (just like holding ⇧shift in normal)

| `✱`+   | Maps to        | Comment                  |
| ------ | -------------- | ------------------------ |
| `H`    | `←` LeftArrow  | cursor left              |
| `J`    | `↓` DownArrow  | cursor down              |
| `K`    | `↑` UpArrow    | cursor up                |
| `L`    | `→` RightArrow | cursor right             |
| `U`    | `⇞` PageUp     | cursor page up           |
| `I`    | `↖` Home       | cursor to line(doc) head |
| `O`    | `↘`  End       | cursor to line(doc) end  |
| `P`    | `⇟` PageDn     | cursor page down         |

### Deletion

| `✱`+      | Maps to                            | Comment             |
| --------- | ---------------------------------- | ------------------- |
| `N`       | `⌥⌫`  Option + ForwardDelete       | Delete a word ahead |
| `M`       | `⌫` ForwardDelete                  | Delete a char ahead |
| `,`       | `⌦` Delete                         | Delete a char after |
| `.`       | `⌥⌦` Option + Delete               | Delete a word after |
| `⌘M`,`⌘N` | `⌘⌥⌫` Command+Option+ForwardDelete | Delete to line head |

### Window Control

| `✱`+             | Maps to                 | Comment                                  |
| ---------------- | ----------------------- | ---------------------------------------- |
| `⇥` Tab          | `⌘⇥` Command+Tab        | Switch Window                            |
| `⌘⇥` Command+Tab | `⌘⇧⇥` Command+Shift+Tab | Switch Window Reversely                  |
| `Q`              | `⌘Q`                    | Close Window                             |
| `W`              | `⌘W`                    | Close Tab                                |
| `R`              | Open Safari             | Open Web Browser                         |
| `⌘R`             | Open Finder             | Open File Browser                        |
| `/`              | `⌥⇧␣`                   | TotalSpaces: Single desktop exposé       |
| `⌘/`             | `⌥⇧⌘␣`                  | TotalSpaces: Instant expose              |
| `C`              | `⌃←`                    | TotalSpaces: Switch to left desktop      |
| `V`              | `⌃→`                    | TotalSpaces: Switch to right desktop     |
| `⌘C`             | `⌃⇧←`                    | TotalSpaces: Switch to left desktop, with current window      |
| `⌘V`             | `⌃⇧→`                    | TotalSpaces: Switch to right desktop, with current window     |
| `E`              | `⌘⇧}`                   | Switch Tab                               |
| `⌘E`             | `⌘⇧{`                   | Swtich Tab Reversely                     |
| `⌘D`             | `F11`                   | Show Desktop                             |
| `D`              | `⌃⌥⌘C`                  | SizeUp: Center Window                    |
| `A`              | ⌃⌥⌘←                    | SizeUp: Left Side                        |
| `S`              | ⌃⌥⌘↑                    | SizeUp: Right Side                       |
| `Z`              | ⌃⌥⌘↓                    | SizeUp: Up Side                          |
| `X`              | ⌃⌥⌘→                    | SizeUp: Down Side                        |
| `⌘A`             | ⌃⌥⇧←                    | SizeUp: Upper Left Side                  |
| `⌘S`             | ⌃⌥⇧↑                    | SizeUp: Upper Right Side                 |
| `⌘Z`             | ⌃⌥⇧↓                    | SizeUp: Lower Left Side                  |
| `⌘X`             | ⌃⌥⇧→                    | SizeUp: Lower Right Side                 |



#### Applications

- Maybe you'd like overwrite these with your own favorite apps.

| `✱`+   | Maps to                 | Comment                                  |
| ------ | ----------------------- | ---------------------------------------- |
| `Y`    | Open OmniOutliner       | Create, collect and organize information |
| `⌘Y`   | Open Typora             | A great WYSIWYG MarkDown editor          |
| `T`    | Open iTerm2             | A better terminal                        |
| `⌘T`   | Open Terminal           | Vanilla terminal                         |
| `F`    | Open Dictionary         | Find API Document                        |
| `⌘F`   | Open SnippetsLab        | Snippets manager                         |
| `G`    | Open Intellij IDEA      | Open IDE                                 |
| `⌘G`   | Open Chrome             | Google Chrome                            |

### Functional

- Use F1,…F12 as standard functional keys, while hold hyper to turn them back.

| `✱`+              | Maps to              | Comment                          |
| ----------------- | -------------------- | -------------------------------- |
| `F1`              | `BrightnessDown`     |                                  |
| `F2`              | `BrightnessUp`       |                                  |
| `F3`              | `ExposeAll`          |                                  |
| `F4`              | `LaunchPad`          |                                  |
| `F5`              | `KeyboardLightDown`  |                                  |
| `F6`              | `KeyboardLightUp`    |                                  |
| `F7`              | `MusicPrev`          |                                  |
| `F8`              | `MusicPlay`          |                                  |
| `F9`              | `MusicNext`          |                                  |
| `F10`             | `Mute`               |                                  |
| `F11`             | `VolumeDown`         |                                  |
| `F12`             | `VolumeUp`           |                                  |
| `F13` PrintScreen | `MusicPrev`          |                                  |
| `F14` ScrollLock  | `MusicNext`          |                                  |
| `F15` Pause       | `MusicPlay`          | Just as it shows                 |
| `Insert`          | `⌥BrightnessUp`      | Fine grained brightness up       |
| `Delete`          | `⌥BrightnessDown`    | Fine grained brightness down     |
| `Home`            | `⌥KeyboardLightUp`   | Fine grained keyboard light up   |
| `End`             | `⌥KeyboardLightDown` | Fine grained keyboard light down |
| `PgUp`            | `⌥VolumeUp`          | Fine grained volume up           |
| `PgDn`            | `⌥VolumeDown`        | Fine grained volume down         |

### Shifter

- A more convient shift for most case

| `✱`+               | Maps to | Comment                  |
| ------------------ | ------- | ------------------------ |
| `1`                | `!`     | Exclamation              |
| `2`                | `@`     | At                       |
| `3`                | `#`     | Sharp                    |
| `4`                | `$`     | Dollar                   |
| `5`                | `%`     | Percent                  |
| `6`                | `^`     | Caret                    |
| `7`                | `&`     | Ampersand                |
| `8`                | `*`     | Star                     |
| `9`                | `(`     | Left Round Bracket       |
| `0`                | `)`     | Right Round Bracket      |
| `-` Minus          | `_`     | Hyphen                   |
| `=` Equal          | `+`     | Plus                     |
| `[` Left Bracket   | `{`     | Left Curly Bracket       |
| `]`  Right Bracket | `}`     | Right Curly Bracket      |
| `\` Back Slash     | `\|`     | Bar                      |
| `;` Semicolon      | `:`     | Colon                    |
| `'` Single Quote   | `"`     | DoubleQuote              |

### Misc

| `✱`+                   | Maps to             | Comment                                  |
| ---------------------- | ------------------- | ---------------------------------------- |
| `~` BackQuote          | `⌃⇧⌘4`              | macOS Area Screenshot to Clipboard       |
| `⌘~` Command+BackQuote | `⌃⇧4`               | macOS Area Screenshot to Desktop File    |
| `⌫` Backspace          | `⌘⌫`                | macOS Delete File                        |
| `↩`  Return            | `⇧↵`                | Shift Return, IDEA interprets this as new line below current |

### Disable ⌘H

macOS will "Hide current window" on ⌘H by default. When you start using hjkl for arrow keys, this behavior
punishes missing hitting the `✱`-key quite much. This rules maps ⌘H to ←

| Original combination   | Maps to             | Comment                                  |
| ---------------------- | ------------------- | ---------------------------------------- |
| `⌘H`                   | `←`  Left arrow     | Map ⌘H to ← |



## Symbol Reference

### Modifiers: Mac

| Sym  | Key     |
| ---- | ------- |
| ✱    | Hyper   |
| ⌃    | Control |
| ⌥    | Option  |
| ⇧    | Shift   |
| ⌘    | Command |

### Modifiers: ⊞Windows

| Sym  | Key     |
| ---- | ------- |
| ✱    | Hyper   |
| ⌃    | Control |
| ⊞    | Windows |
| ⇧    | Shift   |
| ⎇    | Alter   |

### Normal Keys

| GLYPH   | NAME                                   |
| ------- | -------------------------------------- |
|        | Apple                                  |
| ⌘       | Command, Cmd, Clover, (formerly) Apple |
| ⌃       | Control, Ctl, Ctrl                     |
| ⌥       | Option, Opt, (Windows) Alt             |
| ⎇       | Alt                                    |
| ⇧       | Shift                                  |
| ⇪       | Caps lock                              |
| ⏏       | Eject                                  |
| ↩, ↵, ⏎ | Return, Carriage Return                |
| ⌤       | Enter                                  |
| ⌫       | Delete, Backspace                      |
| ⌦       | Forward Delete                         |
| ⎋       | Escape, Esc                            |
| →       | Right arrow                            |
| ←       | Left arrow                             |
| ↑       | Up arrow                               |
| ↓       | Down arrow                             |
| ⇞       | Page Up, PgUp                          |
| ⇟       | Page Down, PgDn                        |
| ↖       | Home                                   |
| ↘       | End                                    |
| ⌧       | Clear                                  |
| ⇥       | Tab, Tab Right, Horizontal Tab         |
| ⇤       | Shift Tab, Tab Left, Back-tab          |
| ␢       | Space, Blank                           |
| ␣       | Space, Blank                           |
| ❘⃝      | Power                                  |
| ⇭       | Num lock                               |
| ?⃝      | Help                                   |
|        | Context menu                           |





## FAQ

- Q： Why using ✱ as symbol of hyper key？

  A：Cause asterisk have the ascii code 42, which is the answer to life, the universe, and everything!  while itself has meaning 'star'. ✱ (Heavy-Asterisk) is a pretty version of `*`(Asterisk). Actually I would choose ☯  if Github could render it properly...

- Q：Why Linux support is missing？

  A：Cause I always use Linux through Terminal of Mac or Windows, so….

- Q:  Why there is some different key bindings between Mac version and Win version?

  A:   Since I don't use windows anymore（Except Steam！）, the win version is no longer matined. I am LAZY…, welcome if you could fix that...  

- Q:  Why there's an old Mac version?

  A:  Because Apple is really capricious. macOS Sierra changes it's kernel architecture, so the old version karabiner is incompatible with macOS higher than 10.12. But now there's a new version of karabiner named karabiner-elements. While karabiner-elements use a new JSON-format conf instead of old XML-format. Still, I'm lazy to maintain old format conf…., embrace the new one please...



## About

Author：Vonng(fengruohang@outlook.com)

License：WTFPL

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/WTFPL_logo.svg/140px-WTFPL_logo.svg.png)

```
do What The Fuck you want to Public License

Version 1.0
Copyright (C) 2000 Feng Ruohang (Vonng).
Everyone is permitted to copy and distribute verbatim copies
of this license document, but changing it is not allowed.

Ok, the purpose of this license is simple
and you just

DO WHAT THE FUCK YOU WANT TO.
```





