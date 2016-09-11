# maildir

Email every file in the current working directory from the command line.

```sh
usage: maildir [-h] [-r FROM-ADDR] [-c CC-ADDR] to-addr

Mail files in a directory.

positional arguments:
  to-addr       The recepient address

optional arguments:
  -h, --help    show this help message and exit
  -r FROM-ADDR  Sets the from address
  -c CC-ADDR    Sets the cc address
```

### Install

`maildir` is a python script that works with Python 2.7 and up.

```sh
$ git clone https://github.com/zhaorz/maildir.git
$ cd maildir
$ chmod +x maildir
$ cp ./maildir ~/bin              # or your favorite bin

# if path is not set
$ export PATH="$PATH:~/bin"
```

### Mail

To mail everything in `./` to example@foo.bar with reply address baz@bar.foo

```sh
$ maildir -r baz@bar.foo example@foo.bar
```
