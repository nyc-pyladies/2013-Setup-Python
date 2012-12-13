To build pandas from source, one needs to have a C compiler. De\
pending on your version of Mac OS, there are different ways to \
get it.

## First, find out if you have a compiler

Open up a Terminal and enter this command:

<pre>cc --version</pre>

If you see a "command not found" message, then you'll need to follow the instructions on this page.

If you are *lucky* you will see a version number message like:
<pre>
cc (Mac OS) 4.7.2
Copyright (C) ...
(and so on)
</pre>

In that case, you're already done! Congratulations! You can skip this step!

## If you need a compiler, identify your version of Mac OS

For the rest of this guide, you'll need to know what version of Mac OS you have.

If you need help figuring that out, ask a staffer.

## For Lion or Mountain Lion

For OS X Lion 10.7, use this download link and install this package:

* http://acm.jhu.edu/~paulproteus/tmp/xcode452cltools10-10-8.dmg

For OS X Lion 10.7, use this download link and install this package:

* http://acm.jhu.edu/~paulproteus/tmp/xcode452cltools10-10-7.dmg

Download and install the .pkg file in those.

## For other versions of Mac OS

Note that these instructions are untested, but we think they will work.

For Mac OS 10.6, use this download link and install this package:

* https://github.com/downloads/kennethreitz/osx-gcc-installer/GCC-10.6.pkg

For Mac OS 10.5, use this download link and install this package:

* http://acm.jhu.edu/~paulproteus/tmp/xcode-3.1.4.dmg

## Test it

Open up a Terminal, and enter:

<pre>
cc --version
</pre>

You should get a version number and copyright information message.

If you get "command not found," then speak to a staffer.

## Back to laptop setup

[&laquo; Back to laptop setup](laptop setup)