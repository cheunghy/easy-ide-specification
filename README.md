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

WIP

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
