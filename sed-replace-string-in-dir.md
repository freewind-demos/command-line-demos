https://stackoverflow.com/questions/905144/sed-beginner-changing-all-occurrences-in-a-folder

```
find . -type f -exec sed -i "s/foo/bar/g" {} \;
```

最后的`\;`是转义符，是用来告诉`-exec`命令的结束位置。
由于`;`会被shell抢先识别，所以需要一个`\;`转义。

