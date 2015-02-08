# Sublime Text git Commit Message Syntax

Syntax Highlighting for SublimeText / Text Mate

## How to make commits with Sublime Text
For the following options, you'll need to use the appropriate command from below:
**Note** for Windows, you must have `Build 3065` or lated to have command line support

- Mac / Linux: `subl -w`
- Windows: `subl.exe -w`

### Preferred Method: Edit `.bashrc`
This will allow for more editing options than just the git commit, like editing diffs. This also leaves flexibility as it can be easily overridden, by the `.gitconfig` for example.
Add the following to your `.bashrc`:
On Mac and Linux:

```
export EDITOR="subl -w"
```

### Alternate Method: Ammend your `.gitconfig`
You can run the following command to let git update your `.gitconfig`

```
git config --global core.editor 'subl -w'
```

Or add the following line manually to your `.gitconfig`
```
[core]
    editor = 'subl -w'
```
