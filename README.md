`show` allows you to display images in any terminal that supports the iTerm
image protocol. It is similar to `imgcat`, but with some improvements.

1. There is no dependency on `bash`, `awk`, or `base64`.
   It should be portable to any POSIX system.
2. Running from a symlink named `push` will cause the file to be downloaded
   rather than displayed.
3. Simpler and more efficient than `imgcat` e.g. never needs to decode base64.

Note: This does not work in tmux. See https://github.com/tmux/tmux/issues/1502
and https://gitlab.com/gnachman/iterm2/-/issues/3898#note_126786057
