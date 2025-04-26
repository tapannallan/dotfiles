# Dotfiles

This repository contains configuration files (dotfiles) for setting up and customizing your development environment. These dotfiles can be managed and installed using [GNU Stow](https://www.gnu.org/software/stow/), a symlink manager.

## Installation

1. Clone this repository to your home directory at `~/dotfiles`
    ```bash
    git clone https://github.com/your-username/dotfiles.git ~/dotfiles
    cd ~/dotfiles
    ```

2. Use `stow` to create symlinks for the desired configuration. For example:
    - To install the `zsh` configuration:
      ```bash
      stow zsh
      ```
    - To install the `vim` configuration:
      ```bash
      stow vim
      ```

3. The symlinks will be created in your home directory, pointing to the files in this repository.

## Example Commands

- Install all configurations:
  ```bash
  stow *
  ```

- Uninstall a specific configuration (e.g., `zsh`):
  ```bash
  stow -D zsh
  ```

- Preview changes before applying:
  ```bash
  stow -n zsh
  ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.