# install

Make sure you have XCode 9 selected:

`xcode-select -s /Applications/Xcode9.app/Contents/Developer`

## distcc slaves

1. `brew install aubonbeurre/homebrew-tap/distcc`
2. `distccd --no-detach --daemon --allow 192.168.0.0/16 --allow 127.0.0.1 --log-stderr --verbose`

## distcc master

`~/.distcc/hosts` example:

```
#Laptop
192.168.0.42/10
#Henry
#192.168.0.48/10
#PC
192.168.0.47/18
#127.0.0.1/2,cpp,lzo
```
