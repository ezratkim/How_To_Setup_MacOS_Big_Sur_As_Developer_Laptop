1. Check existing python version
   ```sh
   python --version
   python3 --version
   ```
2. Install Anaconda3 using homebrew
   ```sh
   brew install anaconda
   ```
3. Update .profile with the path for anaconda3/bin
   ```sh
   vim .profile
   export PATH=$HOME/bin:$HOME/homebrew/bin:$HOME/homebrew/anaconda3/bin:$PATH
   ```