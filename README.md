FunKarma integration/staging tree
================================

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2015 FunKarma Developers

What is FunKarma?
----------------

FunKarma is a fork of Litecoin using scrypt as a proof-of-work algorithm.
This will never end up on an exchange and hopefully with never have any financial value.
 - 2 minute block targets
 - ~1 million total coins

The rest is the same as Bitcoin.
 - 5000 coins per block

License
-------

FunKarma is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./FunKarma-qt_test

