# Add autocorrect to git 

If you want git to correct typos you can set `help.autocorrect`: 

```bash 
$ git config --global help.autocorrect 30
```

You can set `help.autocorrect` to an integer representing the time you have to change your mind before git executes the command(1 = 0.1 seconds).

For example: 

```bash 
$ git comit
Warning: You called a git command named 'comit', which does not exist. Continuing under the assumption that you meant 'commit' in 3 seconds automatically...
``` 

From [**Enki**](https://www.enki.com/) 