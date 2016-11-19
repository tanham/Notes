# Custom color options 

You can change the default color options for the console text. 

For example, to set the color of changed files to **magenta foregound**, **white background** and **bold text**:

```bash 
$ git config --global color.status.changed "magenta white bold"
```

If you run `git status` git wil display any changed files in the new color setting. 

The other `color.*` options are `ui`, `branch.*`, `diff.*`, and `interactive.*`. 

From [**Enki**](https://www.enki.com/)  