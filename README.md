# Minimal RocksDB

My Second project while learning Zig, based on [A minimal RocksDB example with Zig
](https://notes.eatonphil.com/zigrocks.html).

## Build

```bash
git clone https://github.com/facebook/rocksdb
(cd rocksdb && make shared_lib -j8)
zig build
```

## Run

```bash
./zig-out/bin/main set a 10
./zig-out/bin/main set b 20
./zig-out/bin/main list
a = 10
b = 20
./zig-out/bin/main get a
10
```
