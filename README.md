Welcome to tmux!

[![Build Status](https://travis-ci.org/ThomasAdam/tmux.svg?branch=master)](https://travis-ci.org/ThomasAdam/tmux)

tmux is a "terminal multiplexer", it enables a number of terminals (or windows)
to be accessed and controlled from a single terminal. tmux is intended to be a
simple, modern, BSD-licensed alternative to programs such as GNU screen.

This release runs on OpenBSD, FreeBSD, NetBSD, Linux, OS X and Solaris.

tmux depends on libevent 2.x. Download it from:

	http://www.monkey.org/~provos/libevent/

To build tmux from a release tarball, do:

	$ ./configure && make
	$ sudo make install

To get and build the latest from version control:

	$ git clone git://git.code.sf.net/p/tmux/tmux-code tmux
	$ cd tmux
	$ sh autogen.sh
	$ ./configure && make

For more information see https://sourceforge.net/scm/?type=git&group_id=200378
and http://git-scm.com. Patches should be sent by email to the mailing list at
tmux-users@googlegroups.com.

For documentation on using tmux, see the tmux.1 manpage. It can be viewed from
the source tree with:

	$ nroff -mdoc tmux.1|less

Some common questions are answered in the FAQ file and a more extensive (but
slightly out of date) guide is available in the OpenBSD FAQ at
http://www.openbsd.org/faq/faq7.html#tmux. A rough todo list is in the TODO
file and some example configurations and a Vim syntax file are in the examples
directory.

For debugging, running tmux with -v or -vv will generate server and client log
files in the current directory.

tmux mailing lists are available. For general discussion and bug reports:

	https://groups.google.com/forum/#!forum/tmux-users

And for Git commit emails:

	https://groups.google.com/forum/#!forum/tmux-git

Bug reports, feature suggestions and especially code contributions are most
welcome. Please send by email to:

	tmux-users@googlegroups.com

This file and the CHANGES, FAQ and TODO files are licensed under the ISC
license. Files under examples/ remain copyright their authors unless otherwise
stated in the file but permission has been received to distribute them with
tmux. All other files have a license and copyright notice at their start.

-- Nicholas Marriott <nicholas.marriott@gmail.com>
