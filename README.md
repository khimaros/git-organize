# GIT ORGANIZE

automatically organize git repositories based on their `remote.origin`

## overview

NOTE: git-organize expects the git remote to be named `origin`.

git-organize takes a flat directory structure like this:

```
git-organize/
smart-auto-move/
whisper-large/
stable-diffusion-v1-5/
```

and turns it into this:

```
github.com/
    khimaros/
        git-organize/
        smart-auto-move/

huggingface.co/
    openai/
        whisper-large/
    runwayml/
        stable-diffusion-v1-5/
```

## usage

clone this repository and add it to your path

if you'd like the repositories to be moved somewhere other than `~/src`,
set `$GIT_ORGANIZE_BASE` to another path.

run the following in a directory containing at least one subdirectory
which is a git repository:

```shell
$ git organize .
```

there is also another script `git-cl` which clones to the correct directory.

```shell
$ git cl https://github.com/khimaros/git-organize
```
