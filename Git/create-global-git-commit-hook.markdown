# Create a global git commit hook 

Set up templates: 

```bash 
git config --global init.templatedir '~/.git-templates'
```

Make a directory to hold the global hooks: 

```bash 
mkdir -p ~/.git-templates/hooks/pre-commit
```

Write a hook and make sure the hook is executable: 

```bash 
chmod a+x ~/. git-templates/hooks/pre-commit
```

Run `git init` on your repository to include the global hooks. 


From [**Enki**](https://www.enki.com/) 