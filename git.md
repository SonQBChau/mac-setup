# How to ignore certain files on local development

1. First, we have to remove it from cache (might want make a copy before **removing** it, but vscode can reverse it easily).
2. 
```
$ git rm --cached FILENAME
```

2. Then, we add it to .gitignore.

3. Repeat step 1 for .gitignore.

4. Add .gitignore to .git/info/exclude

