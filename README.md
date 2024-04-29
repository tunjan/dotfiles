
# Dotfiles Repository

## Structure of the Repository

The repository is structured as follows:

- `.config/`  
  - `alacritty/`: Configuration for the Alacritty terminal emulator.
  - `dunst/`: Dunst notification settings.
  - `fontconfig/`: Font configurations.
  - `gtk-3.0/`: GTK3 settings.
  - `lf/`: Configurations for LF, the terminal file manager.
  - `fcitx5/`: Configurations for Fcitx5 input method.
  - `shell/`: Shell-specific settings.
  - `x11/`: X11 display settings.
  - `zathura/`: Zathura PDF viewer settings.
- `picom.conf`: Configuration file for Picom, a standalone compositor for Xorg.

## Installation Steps

1. **Clone the Repository**
  ```git clone https://github.com/tunjan/dotfiles.git ~/.dotfiles```

2. **Navigate to the Directory**  
  ```cd ~/.dotfiles```

3. **Sync the Files**  
Ideally, use a tool like `chezmoi` to symlink the configuration files, so any changes in the repository can be easily reflected on the system.

## How to Implement using "chezmoi"

1. **Install `chezmoi`**  
Refer to the [official documentation](https://www.chezmoi.io/docs/install/) to install it on your system.

2. **Initialize `chezmoi` with Your Dotfiles Repository**  
```chezmoi init https://github.com/tunjan/dotfiles.git```

3. **Apply the Dotfiles**  
```chezmoi apply```


Now, your configurations should be in place. Whenever you make changes to your dotfiles in the repository, you can pull the changes and run `chezmoi apply` to update your system configurations.

