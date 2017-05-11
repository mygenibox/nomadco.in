# nomadco.in
NOMADCOIN IMPLEMENTATION BETA 0.1.1 RELEASE

Nomadcoin.
---------------------------------------------

Mainnet:
---------

- RPC Port: 5555
- P2P Port: 5556

Testnet:
---------

- RPC Port: 15555
- P2P Port: 15556

Specifications:
---------------

- Short: NOM
- Total coin: 250 Million coin cap.
- X11 hashing algorithm
- Block time: 1 minute
- diff. retarget 15 blocks
- 100 coin reward halving every 129600 Block, the end of POW is after 3 block halvings.
- Stake Interest: 3%
- Minimum Stake Age, 24 hours, One Year Max age

License
-------

Nomadcoin is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the NomadCoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions or are controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/mygenibox/nomadco.in) are created
regularly to indicate new official, stable release versions of Nomadcoin.

BETA Release
-------

Testing and code review and test on short notice. BETA  Release on client side. Manually, any large changes should have a beta release path map and should be applied at client side rather then nomadcoin or nomadco.in server side.

Translations are converted to nomadcoin and nomadco.in server side periodically.

TODO
-------

Run configure with the --enable-debug option, then make. Or run configure with
CXXFLAGS="-g -ggdb -O0" or whatever debug flags you need. Error and debugging messages are written in the debug.log and -debug=... command-line option controls debugging; -debug will turn
on all categories (and give you a very large debug.log file).

The Qt code routes qDebug() output to debug.log under category "qt": run with -debug=qt
to see it.

Run with the -testnet option to run with "play creditbits" on the test network, if you
are testing multi-machine code that needs to operate across the internet.

If you are testing something that can run on one machine, run with the -regtest option.
In regression test mode, blocks can be created on-demand; see qa/rpc-tests/ for tests
that run in -regtest mode.

Compiling with -DDEBUG_LOCKORDER (configure CXXFLAGS="-DDEBUG_LOCKORDER -g") inserts run-time checks for the debug.log file for inconsistencies when bugs or deadlocks tracking is being done on a multithread application.
