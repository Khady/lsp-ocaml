# lsp-ocaml
[![MELPA](http://melpa.org/packages/lsp-ocaml-badge.svg)](http://melpa.org/#/lsp-ocaml)
[![MELPA Stable](http://melpa-stable.milkbox.net/packages/lsp-ocaml-badge.svg)](http://stable.melpa.org/#/lsp-ocaml)

OCaml/Reason support for lsp-mode using [ocaml-language-server](https://github.com/freebroccolo/ocaml-language-server).

## Installation

### From MELPA

Install the package `lsp-ocaml`

### From source

Clone this repository and [lsp-mode](https://github.com/emacs-lsp/lsp-mode) to
suitable paths, and add them to your load path:

```emacs-lisp
(add-to-list 'load-path "<path to lsp-mode>")
(add-to-list 'load-path "<path to lsp-ocaml>")
```

## Enabling `lsp-ocaml`

```emacs-lisp
(require 'lsp-mode)
(require 'lsp-ocaml)

(add-hook 'tuareg-mode-hook #'lsp-ocaml-enable)
(add-hook 'caml-mode-hook #'lsp-ocaml-enable)
(add-hook 'reason-mode-hook #'lsp-ocaml-enable) ;; for Reason support
```

You also need
[ocaml-language-server](https://github.com/freebroccolo/ocaml-language-server)
installed and on your PATH:

```bash
npm i -g ocaml-language-server
```

(`sudo` may be necessary depending on how you have
[npm](https://www.npmjs.com/) setup)
