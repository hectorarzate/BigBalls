Bigballs integration/staging tree
================================

http://www.bigballscoin.com

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2021-2069 BigBalls Developer

What is BigBalls?
----------------

Bigballs is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 1 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~690 million total coins

The rest is almost the same as Bitcoin.
 - 69 coins per block

License
-------

Bigballs is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development of the BigBalls
-------------------

The developer did this because, someday he will do some bug fixes if necesary.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bigballs-project/bigballs/tags) are created
regularly to indicate new official, stable release versions of Bigballs.

Testing the BigBalls
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
    ./bigballs-qt_test

