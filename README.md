# uuidgen static 2.31.1

Fully static build of old version of uuidgen 2.31.1

In Ubuntu 18.04 was used old version of uuidgen which produces uuid not fully compatible with RFC4122. 
In the newer version [it was fixed](https://github.com/util-linux/util-linux/commit/d6ddf07d31dfdc894eb8e7e6842aa856342c526e), but that broke applications which used old uuidgen.

This project builds fully static uuidgen using alpine linux musl docker image.

After cloning project change to the `uuidgen_old_static` directory and run:
```
sh runme.sh
```

The `uuidgen` binary will be in the current directory

Author: Dilshod Mukhtarov (dilshodm@gmail.com)
