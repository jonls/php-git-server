
PHP Git server
==============

This is an implementation of the simple Git HTTP protocol in PHP.
It allows you to serve Git repositories from a simple PHP-enabled server
in situations where the `git` command is not available.

Git is _not_ required to be installed on the server. There is no dependency
on the `git` command, thus it can be installed on a server where `git`
is not available.

It serves most files directly from the files system, and also generates
the files `/info/refs` and `/objects/info/packs`, without the need for
executing `git update-server-info` on the server.
