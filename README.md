# libtxref-client

This is a simple client application for testing the [libtxref library.](https://github.com/dcdpr/libtxref)

## Building libtxref-client

To build libtxref-client, you will need:

* cmake
* g++, clang or Visual Studio (community edition)

libtxref-client uses a pretty standard cmake build system. If you have already built and installed [libtxref](https://github.com/dcdpr/libtxref) you should be able to execute:

```
mkdir build
cd build
cmake ..
make
```

If you have installed libtxref to some special location you can try:

```
mkdir build
cd build
cmake -DCMAKE_PREFIX_PATH=/tmp/txref-install ..
make
```

You can then run the simple application:

```
> ./libtxref_client 
mainnet, extended txref for (blockHeight = 10000, transactionIndex=2, txoIndex=3):
tx1:yq3n-qqzq-qrqq-9z4d-2n
```
