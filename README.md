# bitcoin original sources

archive of original bitcoin material

On Sat, 01 Nov 2008 16:16:33 -0700 Satoshi Nakamoto posted the whitepaper bitcoin.pdf. (md5sum d56d71ecadf2137be09d8b1d35c6c042).

On Thu Jan 8 14:27:40 EST 2009 the first version was released. (md5sum dca1095f053a0c2dc90b19c92bd1ec00 ). http://www.metzdowd.com/pipermail/cryptography/2009-January/014994.html.

Announcing the first release of Bitcoin, a new electronic cash
system that uses a peer-to-peer network to prevent double-spending.
It's completely decentralized with no server or central authority.

See bitcoin.org for screenshots.

Download link:
http://downloads.sourceforge.net/bitcoin/bitcoin-0.1.0.rar

**Windows only for now.  Open source C++ code is included.**

- Unpack the files into a directory
- Run BITCOIN.EXE
- It automatically connects to other nodes

If you can keep a node running that accepts incoming connections,
you'll really be helping the network a lot.  Port 8333 on your
firewall needs to be open to receive incoming connections.

The software is still alpha and experimental.  There's no guarantee
the system's state won't have to be restarted at some point if it
becomes necessary, although I've done everything I can to build in
extensibility and versioning.

You can get coins by getting someone to send you some, or turn on
Options->Generate Coins to run a node and generate blocks.  I made
the proof-of-work difficulty ridiculously easy to start with, so
for a little while in the beginning a typical PC will be able to
generate coins in just a few hours.  It'll get a lot harder when
competition makes the automatic adjustment drive up the difficulty.
Generated coins must wait 120 blocks to mature before they can be
spent.

There are two ways to send money.  If the recipient is online, you
can enter their IP address and it will connect, get a new public
key and send the transaction with comments.  If the recipient is
not online, it is possible to send to their Bitcoin address, which
is a hash of their public key that they give you.  They'll receive
the transaction the next time they connect and get the block it's
in.  This method has the disadvantage that no comment information
is sent, and a bit of privacy may be lost if the address is used
multiple times, but it is a useful alternative if both users can't
be online at the same time or the recipient can't receive incoming
connections.

Total circulation will be 21,000,000 coins.  It'll be distributed
to network nodes when they make blocks, with the amount cut in half
every 4 years.

first 4 years: 10,500,000 coins
next 4 years: 5,250,000 coins
next 4 years: 2,625,000 coins
next 4 years: 1,312,500 coins
etc...

When that runs out, the system can support transaction fees if
needed.  It's based on open market competition, and there will
probably always be nodes willing to process transactions for free.



In november 2008 some sources were distributed privately

"This is the Bitcoin sources from November 16, 2008 - a few months before the current blockchain began.". "I was on the Metzdowd cryptography list at that time.", https://bitcointalk.org/index.php?topic=382374.0 

the private november 2008 version is in the nov08 folder.

the study folder contains the main files of the 0.1 version, roughly 7000 LOC.

*  2660 ./main.cpp
*  1127 ./script.cpp
*  1020 ./net.cpp
*   604 ./db.cpp
*   554 ./sha.cpp
*   373 ./util.cpp
*   265 ./irc.cpp
*  6603 total
