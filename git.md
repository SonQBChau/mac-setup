# How to ignore certain files on local development

1. First, we have to remove it from cache (might want make a copy before **removing** it, but vscode can reverse it easily).

```
$ git rm --cached FILENAME
```

2. Then, we add it to .gitignore.

3. Repeat step 1 for .gitignore.
   
```
$ git rm --cached .gitignore


4. Add .gitignore to .git/info/exclude

