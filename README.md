markdownfmt
===========

Fork of github.com/shurcooL/markdownfmt that targets following additions:

* [Goldmark](https://github.com/yuin/goldmark) used instead of [Blackfriday](https://github.com/russross/blackfriday) to render from parsed markdown AST.
* Full info string support for Fenced Code Block (see [issue](https://github.com/shurcooL/markdownfmt/issues/58)).
* Hash-based headers only.
* Full [Github Flavored Markdown](https://github.github.com/gfm) support.

[![Build Status](https://github.com/Kunde21/markdownfmt/actions/workflows/go.yml/badge.svg?query=branch%3Amaster)](https://github.com/Kunde21/markdownfmt/actions/workflows/go.yml?query=branch%3Amaster)
[![GoDoc](https://godoc.org/github.com/Kunde21/markdownfmt?status.svg)](https://godoc.org/github.com/Kunde21/markdownfmt)

Like `gofmt`, but for Markdown.

![Markdown Format Demo](https://github.com/shurcooL/atom-markdown-format/blob/master/Demo.gif?raw=true)

Note that `markdownfmt` works with pure Markdown files. If you want to use it with Markdown files that have front matter, consider one of [alternatives](#alternatives) that supports that.

Installation
------------

```bash
go get -u github.com/Kunde21/markdownfmt
```

Add `$GOPATH/bin` to your `$PATH` or copy `$GOPATH/bin/markdownfmt` to your `$PATH`.

Usage
-----

```
usage: markdownfmt [flags] [path ...]
  -d=false: display diffs instead of rewriting files
  -l=false: list files whose formatting differs from markdownfmt's
  -w=false: write result to (source) file instead of stdout
```

Editor Plugins
--------------

- [vim-markdownfmt](https://github.com/moorereason/vim-markdownfmt) for Vim.
- [emacs-markdownfmt](https://github.com/nlamirault/emacs-markdownfmt) for Emacs.
- Built-in in Conception.
- [markdown-format](https://atom.io/packages/markdown-format) for Atom (deprecated).
- Add a plugin for your favorite editor here?

Alternatives
------------

- [`mdfmt`](https://github.com/moorereason/mdfmt) - Fork of `markdownfmt` that adds front matter support.
- [`tidy-markdown`](https://github.com/slang800/tidy-markdown) - Project with similar goals, but written in JS and based on a slightly different [styleguide](https://github.com/slang800/markdown-styleguide).

License
-------

- [MIT License](https://opensource.org/licenses/mit-license.php)
