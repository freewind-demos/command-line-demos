mac下的split不支持`-d`，无法生成number后缀，需要安装`gsplit`：

```
brew install coreutils
gsplit -a 3 -b 1G -d bigfile bigfile_
```
