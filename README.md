gcc-vc4
=======

An experimental port of gcc 4.8.1 to the VideoCore IV.

To build, create an object directory and in it, do:

    $SRCDIR/configure --target=vc4-elf --disable-nls --enable-languages=c --without-headers
    make -j4 all-gcc

To run:

    gcc/cc1 -O test.c

The output file is written to test.s.

