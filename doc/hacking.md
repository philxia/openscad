# Coding Style

The OpenSCAD coding style is encoded in `.uncrustify.cfg`.

Coding style highlights:

* Use 2 spaces for indentation
* Use C++11 functionality where applicable. Please read Scott Meyer's Effective Modern C++ for a good primer on modern C++ style and features: http://shop.oreilly.com/product/0636920033707.do

## Beautifying code

Code to be committed can be beautified by installing `uncrustify`
(https://github.com/uncrustify/uncrustify) and running
`scripts/beautify.sh`. This will, by default, beautify all files that
are currently changed.

Alternatively, it's possible to beautify the entire codebase by running `scripts/beautify.sh --all`.
This is not recommended except in special cases like:
* We're upgrading uncrustify to fix rules globally
* You're bringing an old branch to life and want to minimize conflict cause by the large coding style update

Note: Uncrustify is in heavy development and tends to introduce breaking changes from time to time.
OpenSCAD has been tested against uncrustify commit d32ed2c65c0f826fb0fbde00416eaf3e15eea28e (Feb 14 2018).

# Regression Tests

See `testing.txt`

# How to add new function/module

* Implement
* Add test
* Modules: Add example
* Document:
   * wikibooks
   * cheatsheet
   * Modules: tooltips (editor.cc)
   * External editor modes
   * Add to RELEASE_NOTES.md
