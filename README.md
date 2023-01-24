# Zig Updater
Fetch the latest Zig master branch build easily with one command. `update-zig` will automatically parse https://ziglang.org/download/index.json, download the latest `x86_64-linux` archive, and unpack the contents to `$HOME/.zig`.

You can run the command again and nothing will happen if a new build is not available so feel free to spam it however you like.

![](https://user-images.githubusercontent.com/1566759/204081392-5d8659db-139f-43a6-9cad-fd145d8d1e9c.png)

Note: `dialog` colors may be different on your machine.

## Running
`update-zig`

## Prerequisites
Make sure the following packages are installed if any issues arise on your system:
- `gawk`
- `dialog`
- `jq`
- `pv`
- `wget`
- `xz-utils`

## Installing
```
git clone https://github.com/snail23/update-zig $HOME/.zig
chmod +x $HOME/.zig/update-zig
````

Optionally, run `update-zig` on login as well as add `$HOME/.zig` to `PATH`:
```
echo 'PATH="$PATH:$HOME/.zig"' >> $HOME/.profile
echo update-zig >> $HOME/.profile
```

# License
```
MIT License

Copyright (c) 2023 Snail

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
