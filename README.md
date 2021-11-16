
```shell
$ git clone -b 0.5.6 https://github.com/kendryte/kendryte-standalone-sdk.git
$ git clone --recursive https://github.com/tuupola/k210_gfx.git
$ cd k210_gfx/build
$ cmake .. -DSDK=../kendryte-standalone-sdk -DTOOLCHAIN=/opt/riscv/bin
$ make VERBOSE=1
$ kflash -B dan -t firmware.bin
```