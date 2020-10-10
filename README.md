## TinyScheme Auto-Complete for Sublime Text

This auto-complete plugin covers Procedures and other constructs available in TinyScheme programming language. Most procedures are available as _One-Liners_. However, some procedures do have _Block-Form_ variant available as well. It is upto you, which variant you pick; the API imposes no restrictions. Completion tags have been set up with consistency and ease-of-use in mind. Simply type some letters of a procedure and press `Enter`. The full procedure name, together with parentheses and arguments (if any) shall appear at cursor location.


### One-Liner Examples

 Text Entered  |  Result
-------------- | -------------------------------------------------
 `lam`         | `(lambda (args) expression)`
 `def`         | `(define (proc) expression)`
 `let`         | `(let ((variable)) expression)`
 `if`          | `(if test expression_true expression_false)`
 `ve`          | `(vector element_a element_b element_n)`
 `veq`         | `(vector? vector)`
 `ves`         | `(vector-set! vector index value)`
 `vet`         | `(vector->list vector)`
 `oif`         | `(open-input-file path_string)`
 `nts`         | `(number->string number)`
 `ste`         | `(string=? string_a string_b)`
 `sts`         | `(string-set! variable index char)`
 `me`          | `(member element list)`
 `pl`          | `(+ number_a number_b)`
 `expt`        | `(expt number_base number_exponent)`
 `max`         | `(max number_a number_b number_n)`
 `cons`        | `(cons element list)`
 `apn`         | `(append list_a list_b)`
 `nlq`         | `(null? list)`
 `zq`          | `(zero? number)`


### Block-Form Examples

`dflb`
```scheme
(define proc
  (lambda (args)
    expressions
  )
)
```

`dfb`
```scheme
(define (proc)
  expressions
)
```

`letb`
```scheme
(let
  (
    (variable)
  )
    expressions
)
```

`ifbb`
```scheme
(if test
  (begin
    expressions_true
  )
  (begin
    expressions_false
  )
)
```

`foeb`
```scheme
(for-each
  proc
  list
)
```


### Tips

* You need to type only a few letters of a procedure's name. Observe the patterns used in examples.
* In the Auto-Complete popup, you'll come across several entries with embedded `_` character. Please note that the `_` character has been added only for better readability. You don't need to type this character.
* All _Block-Form_ tags have a `block` suffix attached. It is intended to help you identify which items have _Block-Form_ variant available.
* Scheme comes with several predicate procedures. Tags for these procedures have a `Q` suffix attached. Again, it's been done for easy identification and quick access.
* You could use `Tab` and `Shift+Tab` to cycle forward and backward through arguments.
* If you accidentally invoke an undesirable completion, performing a simple Undo `ctrl + z` might be a better fix, rather than manually deleting the unwanted bits.


### Installation _ via Sublime Package Control

* Open command palette by using the menu command: _Tools_ → _Command Palette_
* Select: `Package Control: Install Package`
* Search for the package name: `TinyScheme Auto-Complete` and press `Enter`
* After installation completes, you could start using this plugin straight away; no restart required.


### Installation _ Manually

* Download the plugin (or clone this repository).
* After extraction, copy `tinyscheme_autocomplete` folder to Sublime Text's _Packages_ folder.
* You can locate this folder from Sublime Text by using the menu command: _Preferences_ → _Browse Packages_.
* You could start using this plugin straight away; no restart required.


### Notes

* The data is based upon TinyScheme 1.41.
* Most dialects of Scheme strive to be at least `R5RS` compliant; TinyScheme is no exception. This means coders/users from other dialects of Scheme (Chez, Racket, etc) could also consider using this plugin in their projects.
* This plugin is released under ... GNU General Public License (v3).


### Feedback & Comments

* Email:     civanimal@gmail.com
* Twitter:  `civAnimal`


Copyright © 2020 civAnimal
