### Alacritty installation

This is my Alacritty configuration, clone the repo to configs directory with name `alacritty`: 

```shell
$ cd ~/.config
$ git clone git@github.com:vohonen/alacritty-config.git
```

To install Alacritty on your machine, follow the [installation guide](https://github.com/alacritty/alacritty/blob/master/INSTALL.md). Notice, that for a new machine one might have to also install the dependencies mentioned in the prerequisites.

The `alacritty.yml` file from this repo consists of the Alacritty configuration. It uses the [JetBrains Mono font](https://www.jetbrains.com/lp/mono/), so after cloning make sure you have the font installed. The following commands download and unzip the font family to current user's font directory. (Notice that such a directory may not exist, and in these cases it must be created first)

```shell
$ cd ~/.local/share/fonts
$ wget https://download.jetbrains.com/fonts/JetBrainsMono-2.304.zip 
$ unzip JetBrainsMono-2.304.zip
$ rm JetBrainsMono-2.304.zip
```



