# Set a Git identity based on the working directory

Many developers have separate accounts and Git identities for their personal projects and work-related stuff. To minimize the hassle with switching identities, you
can set a Git identity based on the directory you are in. In the following example you set a work-identity for all repositories located under `~/src/github.com/work_org/`.

In `.gitconfig`:

```
[user]
    name = Me Myself
    email = personal@example.com
    signingkey = D34DB44F

[includeIf "gitdir:~/src/github.com/work_org/"]
    path = ~/.gitconfig_work
```

Then in `~/.gitconfig_work`:

```
[user]
    name = Me Myself
    email = work@example.com
    signingkey = D34DC0D4
    
[core]
    sshCommand = ssh -i ~/.ssh/work_ed25519
```

[Source](https://news.ycombinator.com/item?id=22672491)
