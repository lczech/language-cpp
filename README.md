# Better C/C++ language support in Atom

Adds syntax highlighting and snippets to C/C++ files in Atom.

This is an alternative package for language-c. At the moment, it provides not all features of
the original, but does the ones that are implemented correctly (at least according to my test).

Additional features on top of the original package:

* Special highlighting of documentation comment blocks, starting with `/**`.
* Special meta-tag for `std` functions and classes.
* Correct marking of parenthesis.

Missing features from the original package:

* Specialized preprocessor commands. So far, this package marks all preprocessor directives
  with the same tag, and does not distinguish further between them, e.g. pragmas or disabled
  blocks.
* `libc` functions are not highlighted separatley.
* Resolving function names is very basic so far. Every string follow by an opening parenthesis
  is considert a function. Works for me.

Forked from [atom/language-c](https://github.com/atom/language-c).
Originally [converted](http://atom.io/docs/latest/converting-a-text-mate-bundle)
from the [C TextMate bundle](https://github.com/textmate/c.tmbundle).

Contributions are greatly appreciated. Please fork this repository and open a
pull request to add snippets, make grammar tweaks, etc.
