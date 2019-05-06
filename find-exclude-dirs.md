find . -name "8.js" -not -path "*/node_modules/*" -not -path "*/dist/*" | xargs grep 'http://'
