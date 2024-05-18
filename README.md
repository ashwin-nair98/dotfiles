# Dotfiles Setup Guide

This guide will help you set up a basic development environment with essential tools and custom dotfiles.

## Steps to Setup
Steps to set up your development environment with Xcode, Homebrew, Zsh, Oh My Zsh, Powerlevel10k, and essential tools.

1. **Install Xcode Command Line Tools**:
    ```sh
    xcode-select --install
    ```

2. **Install Homebrew**:
    ```sh
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

3. **Debug Homebrew (Optional)**:
    ```sh
    git -C /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core fetch --unshallow
    git -C /usr/local/Homebrew/Library/Taps/homebrew/homebrew-cask fetch --unshallow
    ```

4. **Install Zsh**:
    ```sh
    brew install zsh
    ```

5. **Install Oh My Zsh**:
    ```sh
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

6. **Install Powerlevel10k Theme**:
    ```sh
    brew install powerlevel10k
    echo "source $(brew --prefix)/share/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
    # Restart your terminal to apply changes
    ```

7. **Install Neovim**:
    ```sh
    brew install neovim
    ```

8. **Install GNU Stow**:
    ```sh
    brew install stow
    ```

9. **Set Up Dotfiles**:
    - Clone your dotfiles repository:
        ```sh
        git clone https://github.com/ashwin-nair98/dotfiles.git ~/dotfiles
        cd ~/dotfiles
        ```
    - Use `stow` to symlink your dotfiles:
        ```sh
        stow .
        ```

10. **Launch Neovim**:
    - Open Neovim and ensure basic features are working as expected:
        ```sh
        nvim
        ```

11. **Install Lazygit**:
    ```sh
    brew install lazygit
    ```

12. **Install Ripgrep**:
    ```sh
    brew install ripgrep
    ```

13. **Enable extras in lazy as needed**

14. **Run in neovim to ensure everything is fine:**
  ```
  :LazyHealth
  ```

With these steps, you will have a well-configured development environment ready to use.
