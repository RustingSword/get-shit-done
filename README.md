# get-shit-done

Originally from https://github.com/leftnode/get-shit-done.

## Usage
Just move `work` and `play` to `/usr/bin` and run them as root.

Remember to change `ini_local` in `work` to an appropriate path.

## What's the difference
1.  This script is for *Linux* with `nscd` installed.
[`nscd`](http://linux.die.net/man/8/nscd) will monitor configuration files
including `/etc/hosts`, so you don't need to manually flush DNS cache after
updating the hosts file.
2. I split the python version into two seperate files just to save some keystrokes...
3. The format of config file (see the example `sites.conf`):
* One site per line, because this is more readable, and easy to add new sites in
the middle, which helps keeping the config file organized.
* Allow comments starting with '#'.

Some simple sanity checks are also added.

If you are using other platforms, you should make some modifications accordingly.
