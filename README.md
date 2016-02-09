Acme::Cow [![Build Status](https://travis-ci.org/hankache/Acme-Cow.svg?branch=master)](https://travis-ci.org/hankache/Acme-Cow)
=========
A Perl 6 implementation of cowsay.

Installation
------------
To install with Panda:

```
panda update
panda install Acme::Cow
```

Examples
--------
```Perl6
use Acme::Cow;

# Default
Cow::cow.new(initial-text => "Hello World!").display;

# Custom face
Cow::cow.new(initial-text => "Hello World!").set-face("stoned").display;

# Custom template
Cow::camelia.new(initial-text => "Hello World!").display;

# Custom template & Custom face
Cow::www.new(initial-text => "Hello World!").set-face("stoned").display;
```

Using the binary
----------------
```
cow-say --help
cow-say --about
cow-say --message='...'
cow-say --message='...' --face='...'
cow-say --message='...' --template='...'
```

To Do
-----
* Enhance the text formatter
* Add more templates
* Use Terminal::ANSIColor to make the output more appealing

Author
------
Naoum Hankache <naoum88@gmail.com>

License
-------
Artistic License 2.0
