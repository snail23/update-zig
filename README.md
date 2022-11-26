# Zig Updater
Fetch the latest Zig master branch build easily with one command. `update-zig` will automatically parse https://ziglang.org/download/index.json, download the latest `x86_64-linux` archive, and unpack the contents to `$HOME/.zig`. You can run the command again and nothing will happen if a new build is not available so feel free to spam it however you like.

## Running
`update-zig`

## Prerequisites
Make sure the following extra packages are installed if any issues arise on your system:
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
