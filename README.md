Easy IDE Specification
======================

## Why need this?

**Me:** Vim, Emacs, TextMate, Sublime Text and Atom, which one is the best
text editor?

**Me:** Well, I use them all.

**You:** Why?

**Me:** Every editor has its own longs and shorts. I use Emacs for GTD, Atom
for markdown editing and Sublime Text for method jumping. And many more.

**You:** You are crazy! You've learned a ton of skills to editing but not
coding.

**Me:** How about all the text editors have same key bindings, and even when
you're editing a file, you use same key bindings to open the same file in
another editor for its nice editing features. The editors work for you
seamlessly.

**You:** Well, why I would learn another set of key bindings?

**Me:** You won't learn another set of key bindings. It just works for you.
This specification is compatible with emacs default key bindings, vim default
key bindings and Sublime Text like key bindings.

Emacs keys should be consistent across platforms. Vim keys should behave same
as if you're using Vim. Sublime Text keys should play well with operating
system. On OS X, it just works since the operating system uses <kbd>Cmd</kbd>
for shortcut keys and emacs uses <kbd>Ctrl</kbd> for key bindings. On Linux,
we should remap system shortcut keys with <kbd>Windows</kbd> key prefix.

The only caveat is that <kbd>ESC</kbd> is used to toggle between editing
modes. So <kbd>C-g</kbd> is used for cancelling. Basically, Emacs keys work
when emacs mode is on, Vim keys work when vim mode is on, and Sublime Text
keys always works regardless editing mode. So that's why your current skills
just work. You should give this a try.

## Specification

### Installation of the editor configuration

The editor configuration should be version controlled, and user can checkout
it or clone it to the directory which the editor required.

There should be a file in the editor configuration that specifies
dependencies.

After user checkout or clone the editor configuration, user may need run a
command to install all the packages. If user doesn't need to run a command to
install all the dependencies, on first launch, the dependencies should be
installed automatically.

Afterwards, when user installed or removed a package, the package list file
should be updated.

### Launch the editor

User should be able to use system native way to open the editor, e.g. click
an icon on the dock to open the editor.

### System commands

| Command | Emacs key | Vim key | Sublime Text key (OS X) |
|:-------:|:---------:|:-------:|:----------------:|
| Cancelling | C-g |  |  |
| Exit editor| C-x C-c | :q | s-q |
| Restart | C-x C-C |  | C-M-s-w |
| Suspend | C-x C-z |  | s-m |
| Toggle full screen | | | C-s-f |
| Command palette | M-x |  | s-P |
| Open menu bar | M-` |  |  |  |

### Configuration

| Command | Emacs key | Vim key | Sublime Text key (OS X) |
|:-------:|:---------:|:-------:|:----------------:|
| Open configuration UI | C-z c p |  | s-, |
| Goto main conf file | C-z c i |  |  |
| Goto a conf file | C-z c c |  |  |
| Goto key bindings file | C-z c k |  |  |  |

### Get help

| Command | Emacs key | Vim key | Sublime Text key (OS X) |
|:-------:|:---------:|:-------:|:----------------:|
| Get documentation of key | C-h k |  |  |
| Get usage of key | C-h c |  |  |
| Get usage of function | C-h f |  |  |
| Get usage of variable | C-h v |  |  |
| Get commands matching predicate | C-h a |  |  |
| Get everything matching predicate | C-h d |  |  |
| Get all key bindings| C-h b |  |  |
| Get help of current syntax| C-h m |  |  |
| Goto log message buffer | C-h e |  |  |
| Read manual | C-h i |  |  |
| Get help in dash (osx doc app) | C-h D |  |  |  |

### more

WIP

## Implementations

* [emacs-easy-ide](https://github.com/cheunghy/emacs-easy-ide)
* [atom-easy-ide](https://github.com/cheunghy/atom-easy-ide)
* [sublime-text-easy-ide](https://github.com/cheunghy/sublime-text-easy-ide)

TextMate version and Vim version are not implemented.

If you implement your own, feel free to update this section.

## Contribution

Welcome to discuss and improve our code editing environment.

You can open issues or submit pull request.
