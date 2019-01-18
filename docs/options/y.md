<!-- TITLE: y -->

#  `y` Yank/paste bytes from/to memory


```
Usage: y[ptxy] [len] [[@]addr] # See wd? for memcpy, same as 'yf'.
```


- `y             `  show yank buffer information (srcoff len bytes)
- `y 16          `  copy 16 bytes into clipboard
- `y 16 0x200    `  copy 16 bytes into clipboard from 0x200
- `y 16 @ 0x200  `  copy 16 bytes into clipboard from 0x200
- `yz [len]      `  copy nul-terminated string (up to blocksize) into clipboard
- `yp            `  print contents of clipboard
- `yx            `  print contents of clipboard in hexadecimal
- `ys            `  print contents of clipboard as string
- `yt 64 0x200   `  copy 64 bytes from current seek to 0x200
- `ytf file      `  dump the clipboard to given file
- `yf 64 0x200   `  copy file 64 bytes from 0x200 from file
- `yfa file copy `  copy all bytes from file (opens w/ io)
- `yfx 10203040  `  yank from hexpairs (same as ywx)
- `yw hello world`  yank from string
- `ywx 10203040  `  yank from hexpairs (same as yfx)
- `yy 0x3344     `  paste clipboard

<p hidden>yz yp yx ys yt ytf yf yfa yy</p>