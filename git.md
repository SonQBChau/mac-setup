# How to ignore certain files on local development

1. First, we have to remove it from git tracking

```
$ git rm --cached FILENAME
```

2. Then, we add it to .gitignore
   
3. Repeat step 1 for .gitignore
   
```
$ git rm --cached .gitignore
```

4. Add .gitignore to .git/info/exclude

5. Put back .gitignore

6. Now git won't track any changes to the FILENAME and .gitignore