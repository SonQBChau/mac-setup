# How to ignore certain files on local development

1. First, we have to remove it from cache (might want make a copy before **removing** it, but github desktop can reverse it easily).

```
$ git rm --cached FILENAME
```

2. Then, we add it to .gitignore.
   
3. Restore the file by copying the file back or by using github desktop reverse changes.

4. Repeat step 1 for .gitignore.
   
```
$ git rm --cached .gitignore
```

5. Add .gitignore to .git/info/exclude

6. Put back .gitignore
