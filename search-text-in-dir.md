```
brew install ag
```

```
~/.a/shims $ ag '0.11.0'
yarnpkg
3:exec /opt/homebrew/Cellar/asdf/0.11.0/libexec/bin/asdf exec "yarnpkg" "$@" # asdf_allow: ' asdf '

ts-node-script
3:exec /opt/homebrew/Cellar/asdf/0.11.0/libexec/bin/asdf exec "ts-node-script" "$@" # asdf_allow: ' asdf '
```

```
~/.a/shims $ ag '0.11.0' -l
yarnpkg
http-server
grunt
ts-node-cwd
ts-node-script
pnpm
fast
n
ts-node
pnpx
yarn
ts-script
pretty-quick
ts-node-transpile-only
near
corepack
npx
ts-node-esm
```

替换

```
~/.a/shims $ ag '0.10.2' -l | xargs sed -i '' 's/0.10.2/0.11.0/g'
```

注意 `sed -i`后有一个空白的字符串`''`