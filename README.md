Tock Loader
===========

Tool for programming Tock onto hardware boards.

Install
-------

```
sudo pip3 install tockloader
```

Usage
-----

This tool installs a binary called `tockloader`, which supports several commands:

### `tockloader listen`

Listen to UART `printf()` data from a board.

### `tockloader flash`

Load binaries onto hardware platforms that are running a compatible bootloader.
This is used by the [TockOS](https://github.com/helena-project/tock) Make system
when application binaries are programmed to the board with `make program`.

### `tockloader list`

Print information about the apps currently loaded onto the board.

### `tockloader replace`

Replace an application that is already flashed to the board with a new
binary.

### `tockloader add`

Add an application binary (or binaries) to the list of installed apps.

### `tockloader remove [application name]`

Remove an application from flash by its name.



Upload to PyPI
--------------

Internal note.

    python3 setup.py sdist
    twine upload dist/tockloader-X.X.X.tar.gz