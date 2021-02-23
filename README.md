# Development Environment for Mac OS

## Mac Settings
<br/>

### **File extensions**
   
 Finder > Preferences > Advanced > Show all filename extensions
 
### **Show hidden files**

Run in terminal `defaults write com.apple.Finder AppleShowAllFiles true`

### **Navbar**
1. Click battery > Show Percentage
2. Set 24 hour clock

### **General Settings**
1. Desktop & Screensaver > Screen Saver > Hot Corners > Mission Control (top), Launchpad (bl)
2. Trackpad > Scroll & Zoom > disable Scroll direction: Natural
3. Trackpad > Point & Click > Secondary Click > click with 2 fingers


## Homebrew

Run in terminal `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Run `brew doctor` to verify the installation.

## iTerm2

1. Run in terminal `brew install --cask iterm2`
2. Preferences > Keys > Hotkey > Show/hide all windows with a system-wide hotkey

## Git

Run in terminal `brew install git`

## Zsh

1. Run in terminal `brew install zsh`
2. Add Zsh to default shell with `sudo vim /etc/shells`
3. Press o to append to new line
4. Add `/usr/local/bin/zsh`
5. Press `esc`
6. Save and quit with `:wq`
7. Run `chsh -s /usr/local/bin/zsh` to change default shell to zsh.
8. Restart terminal.
9. Run `echo $SHELL`. It should return the path to zsh (`/usr/local/bin/zsh`).

## VS Code
1. Run `brew install --cask visual-studio-code`
2. Shell command: Install 'code' command in PATH.

## Oh My Zsh
1. Run `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
2. Run `code ~/.zshrc` to open the config file.

## Terminal Font - MesloLGS NF

1. Install fonts: 
- [Regular Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
- [Bold Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
- [Italic Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
- [Bold Italic Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)
- 
2. iTerm2 > Preferences > Profiles > Text > Font

## Oh My Zsh Theme
1. Run `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`
2. Run `code ~/.zshrc` to open change the theme to `ZSH_THEME="powerlevel10k/powerlevel10k"`
3. Run `p10k configure` 
4. Configuration:
   - Classic style 
   - Unicode Character Set
   -  Light Prompt Color
   -  24 hour time format
   -  Angled separators
   -  Sharp head 
   -  Flat tail
   -  Promp Height of 2 lines 
   -  Prompt Connection - Dotted 
   -  Prompt Frame - Left 
   -  Sparse Spacing 
   -  Many Icons 
   -  Fluent Flow 
   -  Transient Script 
   -  Quiet Prompt Mode (Verbose has issues)

## Zsh Plugins
1. Zsh Syntax Highlighting
   - Highlights commands when typed.
   - Install with `brew install zsh-syntax-highlighting`
   - Add `source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh` to `~/.zshrc`

2. Zsh Autosuggestions
   - Suggests commands based on history.
   - Install with `brew install zsh-autosuggestions`
   - Add `source /usr/local/share/zsh-autosuggestions/zsh-autosuggestions.zsh` to `~/.zshrc`
## VS Code Extensions