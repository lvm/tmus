# tmus

TMux Upteempth Sessionmanager

## help

```
usage: tmus [-h] [-t TARGET_SESSION] [-c] [-V] [cmd]

positional arguments:
  cmd                   Which command to run: 
                        `ls`, lists sessions / windows; 
                        `load`, loads a single session at a time (requires a session name); 
                        `save`, saves a single session at a time (requires a session name);

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET_SESSION, --target-session TARGET_SESSION
                        Session name
  -c, --current-command
                        Read current command for each (session) window. Pretty useless, tbh.
  -V, --verbose         Show stdout messages

```

## how to

Say you're in a tmux session with a bunch of windows loaded

```
$ tmus save -t name-of-this-session
```

So later you can load it.

```
$ tmus load -t name-of-this-session
```

Even if you don't remember the exact name

```
$ tmus ls
```

## license

See [LICENSE](LICENSE)

