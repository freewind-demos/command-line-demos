```
brew install grep
```

will install gnu grep as `ggrep`.

```
ggrep -oP ':\Kread(?= only)' file.txt
```

其中：

- `o`: 只显示匹配的整个表达式而非整行
- `P`: 使用perl语法，支持`\K`和`(?=...)`

为什么要使用gnu grep? 因为mac自带的grep不支持`P`选项。


