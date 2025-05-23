# voiceConvergence

```
git clone https://github.com/Wadym/voiceConvergence.git
```

Switching remote URLs from HTTPS to SSH
Open Terminal.

Change the current working directory to your local project.

List your existing remotes in order to get the name of the remote you want to change.
```
git remote -v

```

```
origin  https://github.com/Wadym/voiceConvergence.git (fetch)
origin  https://github.com/Wadym/voiceConvergence.git (push)
```




Change your remote's URL from HTTPS to SSH with the git remote set-url command.

```
git remote set-url origin git@github.com:Wadym/voiceConvergence.git
```

```
git remote -v
```
```
origin  git@github.com:Wadym/voiceConvergence.git (fetch)
origin  git@github.com:Wadym/voiceConvergence.git (push)
```

If:

```
git push
```

```
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```
Then:

Start SSH agent in the background.
```
 eval "$(ssh-agent -s)"
 ```

```
Agent pid 977
```

