flymake-json.el
===============

An Emacs flymake handler for syntax-checking JSON using `jsonlint`.

Installation
=============

First install `jsonlint`, e.g. via `npm`:

    npm install jsonlint -g

If you choose not to use one of the convenient packages in
[Melpa][melpa] and [Marmalade][marmalade], you'll need to add the
directory containing `flymake-json.el` to your `load-path`, and then
`(require 'flymake-json)`. You'll also need to install
[flymake-easy](https://github.com/purcell/flymake-easy).

Usage
=====

Add the following to your emacs init file:

    (require 'flymake-haml) ;; not required if installed from a package

Then, if you're using `json-mode':

    (add-hook 'json-mode 'flymake-json-load)

or, if you use `js-mode' for json:

    (add-hook 'js-mode-hook 'flymake-json-maybe-load)

otherwise:

    (add-hook 'find-file-hook 'flymake-json-maybe-load)

[marmalade]: http://marmalade-repo.org
[melpa]: http://melpa.milkbox.net

<hr>

[![](http://api.coderwall.com/purcell/endorsecount.png)](http://coderwall.com/purcell)

[![](http://www.linkedin.com/img/webpromo/btn_liprofile_blue_80x15.png)](http://uk.linkedin.com/in/stevepurcell)

[Steve Purcell's blog](http://www.sanityinc.com/) // [@sanityinc on Twitter](https://twitter.com/sanityinc)
