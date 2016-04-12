gomdb
=====

Low level Go wrapper for OpenLDAP Lightning Memory-Mapped Database (LMDB).
Read more about LMDB here: http://symas.com/mdb/
For a high level go wrapper (highly suggested), see https://github.com/libreoscar/lmdb

GoDoc available here: http://godoc.org/github.com/libreoscar/gomdb

Build
=======

`go get github.com/libreoscar/gomdb`

There is no dependency on LMDB dynamic library.

On FreeBSD 10, you must explicitly set `CC` (otherwise it will fail with a cryptic error), for example:

`CC=clang go test -v`

TODO
======

 * write more documentation
 * write more unit test
 * benchmark
 * figure out how can you write go binding for `MDB_comp_func` and `MDB_rel_func`
 * Handle go `*Cursor` close with `txn.Commit` and `txn.Abort` transparently

