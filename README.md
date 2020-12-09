# How_To_Setup_MacOS_Big_Sur_As_Developer_Laptop
1. Install Xcode
2. Start Xcode and allow it to install additional development tools
3. Check if default shell is zsh
   ```sh
   echo $SHELL
   ```
4. Install oh-my-zsh
   ```sh
   sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```
5. Install homebrew
   ```sh
   mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C homebrew
   ```
6. Go to https://github.com/romkatv/powerlevel10k#manual and follow the README to install powerlevel10k
7. Edit ~/.zshrc and add the following line to the top of the file
   ```sh
   source $HOME/.profile
   ```
8. Create .profile in your home directory
   ```sh
   vim ~/.profile
   ```
9. Edit .profile and add the following
   ```sh
   export PATH=$HOME/bin:$HOME/homebrew/bin:$PATH
   ```
10. Update homebrew
   ```sh
   brew update && brew upgrade && brew cask upgrade && brew cleanup
   ```
11. Edit .profile and add the following to set the default editor to vscode
   ```sh
   export EDITOR="code -w"
   ```
12. Install archey
   ```sh
   brew install archey
   ```
13. Edit .profile and add the following
   ```sh
   archey -o
   ```
14. Install vscode
   ```sh
   brew install visual-studio-code
   ```

