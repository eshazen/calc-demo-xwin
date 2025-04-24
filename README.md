# calc-demo-xwin
## X-Windows calculator demo application

This is a simple X-Windows application using the old XForms library
to experiment with various calculator UI features.  It is certainly
usable as-is.

See `https://github.com/eshazen/hex-calc` for a hardware implementation.


To build:
```
  $ cd src
  $ make clean
  $ make
```

Also see [macOS instructions](README-MacOS.md).

What works:

* Value entry with various word sizes and hex/bin/dec radix
* Conversion between sizes with sign-extension
* Negate with CHS
* Twos compliment arithmetic
* Stack ops similar to HP: Enter, Drop, exchange, clear

Very early screenshot below

[![early_screenshot.jpg](pix/early_screenshot.jpg)]

## Todo

* ENTER should duplicate X but set flag to over-type _(done)_
* Fix decimal entry so digits roll off in a sensible way _(done)_
* What to do if you enter a value above unsigned max in decimal? _(done)_
* check arithmetic behavior vs word size
* add some more functions and hot-keys
* add hot-key menu somewhere
* use a bigger font for the display
