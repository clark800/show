`show` allows you to display images in any terminal that supports the iTerm
image protocol. It is similar to `imgcat`, but with some improvements.

1. There is no dependency on `bash`, `awk`, or `base64`.
   It should be portable to any POSIX system.
2. It fixes a `tmux` issue where the prompt gets drawn over the image. In `tmux`
   the screen will be cleared and the image will be displayed with a fixed
   height that can be configured with the `SHOW_HEIGHT_TMUX` environment
   variable.
3. Running from a symlink named `push` will cause the file to be downloaded
   rather than displayed.
4. Simpler and more efficient than `imgcat` e.g. never needs to decode base64.
