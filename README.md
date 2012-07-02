ColorStack
==========

    Usage: colorstack [<file>]

    This script will read CloudStack log events and colorize interesting things.
    By default it will read stdin.  If a filename is passed as an argument, it will
    read entries from that file instead.

Copy this file to `/usr/local/bin` on your management server(s).

Examples
--------
    $ tail -f /var/log/cloud/management/management-server.log | colorstack
    $ colorstack somefile.log  #same as `colorstack < somefile.log'
    $ zcat management-server.log.2012-05-2?.gz | colorstack | less -R

Hasn't been tested with CloudStack 3.x yet.
