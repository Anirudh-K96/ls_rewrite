# ls-in-c

A minimal rewrite of the Unix `ls` command in C. Implements default directory listing and the `-a` flag in ~30 lines, no external dependencies.

## Usage

```bash
gcc -Wall -Wextra -o myls ls.c
./myls
./myls /etc
./myls -a
./myls -a /etc
```

## What's implemented

- Default listing — hides dot files
- `-a` flag — shows everything including hidden files
- Error handling for invalid paths
- Defaults to current directory if no path is given

## What's not implemented

The real `ls` is ~5000 lines. This covers none of that. If you want to go further, look into `stat()` for implementing `-l`.

## Video

[Watch on YouTube](https://www.youtube.com/watch?v=ecW9xK9dtX8)
