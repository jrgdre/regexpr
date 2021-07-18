# Collection of (hopefully) useful regular expressions

## File-Path

While far from being perfect, these are my solutions for finding file-path and
file-name strings and separate one from the other.

### Windows

`/(?:(?'drive'[a-z]\:\\))?(?'path'(?:(?:\.{1,2}|[^*?:<>|\\]+)(?=\\)\\|^\\(?!\\))*)(?'file'[^*?:<>|\\]*|)/i`

Try it on [regex101.com](https://regex101.com/r/bH5cVs/1)

### Linux

`/(?'path'(?:(?:\/.{1,2}|[^*?:<>|\/]+)(?=\/)\/|^\/(?!\/))*)(?'file'[^*?:<>|\/]*|)/i`

Try it on [regex101.com](https://regex101.com/r/P9Ido4/1)
