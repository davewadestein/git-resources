# git-resources

## Git alias for creating a random commit; useful for Git courses

`git config --global.alias rand = "!set $1; echo fixing $1 > $1.txt && git add . && git commit -m \"Adding $1.txt\"; true"`

Or discard git command and add `rand = ...` to `~/.gitconfig` in `[alias]` section.

Then test with `git rand`.

## Colors for git prompt

Put these directly into your `~/.gitconfig` file.

```
[color]
    branch = auto
    diff = auto
    status = auto
[color "branch"]
    current = yellow reverse
    local = yellow
    remote = blue
[color "diff"]
    meta = yellow bold
    frag = magenta bold
    old = red bold
    new = green bold
[color "status"]
    added = yellow
    changed = green
    untracked = green
```
