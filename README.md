# zjumper

A very simple zsh plugin to bookmark directories and easily cd into them using [fzf](https://github.com/junegunn/fzf).


## Installation

- [Install fzf if not already done](https://github.com/junegunn/fzf#using-git)
- Download the zjumper.zsh file and source it into your config :

```zsh
mkdir -p "$HOME/.config/zsh"
wget --output-document="$HOME/.config/zsh/zjumper.zsh" https://raw.githubusercontent.com/romainchapou/zjumper/main/zjumper.zsh
echo 'source "$HOME/.config/zsh/zjumper.zsh"' >> ~/.zshrc

# Recommended alias
echo 'alias z="zjumper"' >> ~/.zshrc
```


## Usage

- Press ctrl-space or alt-z to open a fzf prompt containing your bookmarked directories. Start typing and press enter to select one. You will then cd into this directory.
- `zjumper add` to add the current directory to the bookmarked directories.
- `zjumper list` (or `zjumper ls`) to list the bookmarked directories.
- `zjumper edit` (or `zjumper ed`) to open the list of bookmarked directories in your `$EDITOR`. You can then remove unwanted entries. (Also note that the first entry will be the one selected by default if no text is entered when using the main command).
