# Sublime Text git Commit Message Syntax

Syntax Highlighting for SublimeText / Text Mate

## Installation

### With Package Control:

1. Run the `Package Control: Install Package` command, find and install the Git Commit Message Syntax plugin.
1. Restart Sublime Text (if required)

### Manually:

1. Clone or download the git repo into your packages folder (in Sublime Text, find Browse Packages… menu item to open this folder)
1. Restart Sublime Text editor (if required)


## How to make commits with Sublime Text
For the following options, you'll need to use the appropriate command from below:
**Note** for Windows, you must have `Build 3065` or lated to have command line support

- Mac / Linux: `subl -w`
- Windows: `subl.exe -w`

### Preferred Method: Edit `.bashrc`
This will allow for more editing options than just the git commit, like editing diffs. This also leaves flexibility as it can be easily overridden, by the `.gitconfig` for example.
Add the following to your `.bashrc`:
On Mac and Linux:

```bash
export EDITOR="subl -w"
```

### Alternate Method: Ammend your `.gitconfig`
You can run the following command to let git update your `.gitconfig`

```bash
git config --global core.editor 'subl -w'
```

Or add the following line manually to your `.gitconfig`
```ini
[core]
    editor = 'subl -w'
```
