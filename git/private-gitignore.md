TIL: Creating a private .gitignore

Sometimes I want to add some files to ignore that are not relevant to rest of my team.
For example, I needed a ignore rule for a folder that was specific to an editor extension I was using. 

It can be done by editing the .git/info/exclude in the repository folder.

A global gitignore can be used by editing the .gitconfig file in your user directory.
```
[core]       
    excludesfile = /home/<myusername>/.gitexclude 
```
Then adding the exclude patterns to `~/.gitexclude`.

Main source: https://stackoverflow.com/questions/6117109/is-it-possible-to-have-a-custom-gitignore-read-only-access
