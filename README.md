# Development Environment for Mac OS

## Mac Settings
<br/>

### **File extensions**
   
 Finder > Preferences > Advanced > Show all filename extensions
 
### **Show hidden files**

Run in Terminal `defaults write com.apple.Finder AppleShowAllFiles true`

### **Navbar**
1. Click battery > Show Percentage
2. Set 24 hour clock

### **General Settings**
1. Desktop & Screensaver > Screen Saver > Hot Corners > Mission Control (top), Launchpad (bl)
2. Trackpad > Scroll & Zoom > disable Scroll direction: Natural
3. Trackpad > Point & Click > Secondary Click > click with 2 fingers


## Homebrew

Run in Terminal `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Run `brew doctor` to verify the installation.

## iTerm2

1. Run in Terminal `brew install --cask iterm2`
2. Preferences > Keys > Hotkey > Show/hide all windows with a system-wide hotkey

## Git

Run in Terminal `brew install git`

## Zsh

1. Run in Terminal `brew install zsh`
2. Add Zsh to default shell with `sudo vim /etc/shells`
3. Press o to append to new line
4. Add `/usr/local/bin/zsh`
5. Press `esc`
6. Save and quit with `:wq`