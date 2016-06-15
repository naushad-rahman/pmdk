---
title: libvmmalloc
layout: nvml
---

#### The libvmmalloc library

**libvmmalloc** interposes the traditional _malloc_/_free_ interfaces and,
in a way fully transparent to the program, substitutes the system heap
with a volatile memory pool built on memory-mapped file.  Such memory pool
works in a similar manner as the memory pools provided by **libvmem**,
except that it is created and destroyed automatically for each process
that uses **libvmmalloc**.

The typical usage of **libvmmalloc** is to load it before all other libraries
by setting the environment variable **LD_PRELOAD**.

The [libvmmalloc man page](libvmmalloc.3.html) contains a list of the
interfaces provided.

#### libvmmalloc Examples

**More Detail Coming Soon**

<code data-gist-id='krzycz/3946013194219da6b8f0' data-gist-file='manpage.sh' data-gist-line='37-40' data-gist-highlight-line='40' data-gist-hide-footer='true'></code>