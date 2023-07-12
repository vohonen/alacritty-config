### Alacritty installation

This is my Alacritty configuration, clone the repo to configs directory with name `alacritty`: 

```shell
cd ~/.config
git clone git@github.com:vohonen/alacritty-config.git alacritty
```

To install Alacritty on your machine, follow the [installation guide](https://github.com/alacritty/alacritty/blob/master/INSTALL.md). Notice, that for a new machine one might have to also install the dependencies mentioned in the prerequisites, and the third section "Post Build" is also important for complete features.

To set Alacritty as the default terminal, run

```shell
sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator $(which alacritty) 50
sudo update-alternatives --config x-terminal-emulator
```

Sometimes above doesn't work, i.e. even with the highest priority Alacritty is not preferred as the terminal emulator. If this happens, run the following:

```shell
gsettings set org.gnome.desktop.default-applications.terminal exec cmd_to_open_terminal_of_choice
```

This is equivalent to working from the GUI `dconf-editor > org > gnome > desktop > application > terminal` and setting `alacritty` as the custom value.

The `alacritty.yml` file from this repo consists of the Alacritty configuration. It uses the [JetBrains Mono font](https://www.jetbrains.com/lp/mono/), so after cloning make sure you have the font installed. The following commands download and unzip the font family to current user's font directory. (Notice that such a directory may not exist, and in these cases it must be created first)

```shell
cd ~/.local/share/fonts
wget https://download.jetbrains.com/fonts/JetBrainsMono-2.304.zip 
unzip JetBrainsMono-2.304.zip
rm JetBrainsMono-2.304.zip
```



