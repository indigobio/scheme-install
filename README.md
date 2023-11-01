# Quick Chez Scheme Installations

As of version 10, [Chez Scheme](https://github.com/cisco/ChezScheme) takes a long time to
install because it no longer includes boot files for the various supported platforms. This
repository caches boot files to make installations much faster for non-threaded arm64 and
x86_64 Linux and macOS systems.

## Usage

```
./setup
cd ChezScheme
./configure --force --nothreads # <option> ...
make kernel
sudo make install
```

## Updating

After updating the ChezScheme submodule, run `make-bootfiles`. It assumes your system has
a compatible version of Chez Scheme installed.
