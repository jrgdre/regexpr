# Collection of (hopefully) useful regular expressions

## File-Path

While far from being perfect, these are my solutions for finding file-path and
file-name strings and separate one from the other.

### Windows

`/(?'path'(?:(?:\.{1,2}|[^*?:<>|\\]+|[a-z]:)(?=\\)\\|^\\(?!\\))*)(?'file'[^*?:<>|\\]*|)/i`

Try it on [regex101.com](https://regex101.com/r/1kNz3l/1)

### Lunix

`/(?'path'(?:(?:\/.{1,2}|[^*?:<>|\/]+|[a-z]:)(?=\/)\/|^\/(?!\/))*)(?'file'[^*?:<>|\/]*|)/i`

Try it on [regex101.com](https://regex101.com/r/T5IYfn/1)
