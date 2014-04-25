# Markdown Test Suite

Inspired by questions on [W3C Markdown Community Group](http://www.w3.org/community/markdown).

Pull Requests are welcome. See the [CONTRIBUTING Guidelines](https://github.com/karlcow/markdown-testsuite/blob/master/CONTRIBUTING.md)

## Test Scripts

Markdown Test Suite already includes tests for many important markdown engines.

Install script dependencies with:

    sudo pip install -r requirements.txt

To see what the scripts do run:

    ./cat-all.py -h
    ./run-tests.py -h

To configure the scripts do:

	cp config_local.py.example config_local.py

and edit `config_local.py`. It is already gitignored.

Sample output from `run-tests.py`:

<<<<<<< HEAD
	gfm           |FF     F     F   FFFF  F    F                        FFFF   FF               FF   F       F           | 262.88s  102   20  19%
	kramdown      |      FFF     FF       FF       FF FFFFFFFFFFFFF                       F                              |  30.69s  102   23  22%
    marked        |              F                 FFFFFFFFFFFFFFFF                      F F                             |   6.22s  102   19  18%
	multimarkdown |      FFF    FF   F            FFF FFFFFFFFFFFFF     FFFF         F                                   |   0.58s  102   27  26%
	pandoc        |FF           F F FFFF  FFFFF    FF FFFFFFFFFFFFF     FFFF     FF            FFF FFF                  F|   1.11s  102   41  40%
	redcarpet     |                                                                                                      |  21.49s  102    0   0%

	Extensions:

	gfm           |F |   2.37s    2    1  50%
	kramdown      |  |   0.62s    2    0   0%
    marked        |F |   0.13s    2    1  50%
	multimarkdown |F |   0.01s    2    1  50%
	pandoc        |F |   0.02s    2    1  50%
	redcarpet     |  |   0.42s    2    0   0%
=======
	gfm           |FF.....F.....F...FFFF..F....F........................FFFF...FF...............FF...F.......F...........| 262.88s  102   20  19%
	kramdown      |......FFF.....FF.......FF.......FF.FFFFFFFFFFFFF.......................F..............................|  30.69s  102   23  22%
	multimarkdown |......FFF....FF...F............FFF.FFFFFFFFFFFFF.....FFFF.........F...................................|   0.58s  102   27  26%
	pandoc        |FF...........F.F.FFFF..FFFFF....FF.FFFFFFFFFFFFF.....FFFF.....FF............FFF.FFF..................F|   1.11s  102   41  40%
	redcarpet     |......................................................................................................|  21.49s  102    0   0%

	Extensions:

	gfm           |F.|   2.37s    2    1  50%
	kramdown      |..|   0.62s    2    0   0%
	multimarkdown |F.|   0.01s    2    1  50%
	pandoc        |F.|   0.02s    2    1  50%
	redcarpet     |..|   0.42s    2    0   0%
>>>>>>> b60e1176d0f1be90902e117e6bb45b712024ade0

Where `F` indicates a failing test.
