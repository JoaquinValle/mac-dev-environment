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

## VS Code Plugins
1. change-case
   - Quickly change cases.
2. Code Spell Checker
   - Grammar check in code.
3. Debugger for Chrome
   - Debug code running in Chrome from VS code. 
4. EditorConfig for VS Code
   - Override workspace settings with custom config.
5. ES7 React/Redux/GraphQL/React Native Snippets
   - Adds most used snippets.
6. ESLint
   - Linting support.
7. Markdown All in one
   - Support and features
8. Node.js Modules Intellisense
   - Autocomplete imports.
9. npm
   - Support to run scripts defined in `package.json`
10. npm Intellisense
   -  Autocomplete imports.
11. Partial Diff
    - Compare selections
12. Path Intellisense
    - Autocomplete paths.
13. Prettier
    - Code formatter.
14. Settings Sync
    - Able to get settings from other computers.
15. Tailwind CSS IntelliSense
    - CSS class intellisense for Tailwind.
16. Visual Studio IntelliCode
    - AI-assisted development
17. XML Tools
    - Formatting and support.
18. YAML
    - Formatting and support.
19. :emojisense
    - Adds emoji support.
20. Auto Close Tag
    - Adds closing tags.
21. Auto Rename Tag
    - Changes appropriate tag when edited.
22. Better Comments
    - Styling support in comments
23. Bracket Pair Colorizer
    - Adds color to bracket pairs.
24. Color Info
    - Previews color when typed.
25. DotENV
    - Support and syntax
26. gi
    - Create .gitignore files faster.
27. HTML CSS Support
    - Attribute completion and support.
28. Import Cost
    - Shows package sizes.
29. Live Server
    - Local server for testing
30. Live Share
    - Real-Time collaborative development support.
31. Material Icon Theme
    - Better icons.
32. Material Theme
    - Better editor themes.
33. Polacode
    - Take better screenshots.
34. Project Manager
    - Easily change projects


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
  
3. Zsh Substring History Search
   - Search substrings in history.
   - Install with `brew install zsh-history-substring-search`
   - Add `source /usr/local/share/zsh-history-substring-search/zsh-history-substring-search.zsh` to `~/.zshrc`
   - Bind UP and DOWN keys with bindkey `'^[OA' history-substring-search-up` and `bindkey '^[OB' history-substring-search-down`

## Oh My Zsh Plugins
1. Alias-finder
   - Searches for defined aliases.
2. brew
   - Brew alias commands.
3. copydir
   - Copies current path to clipboard.
4. copyfile
   - Copies file to clipboard.
5. dotenv
   - Loads .env variables when in root folder.
6. npm
   - Adds aliases.
7. nvm
   - Adds aliases.
8. osx
   - Adds aliases and utilities.
9. z
   - Tracks most visited directories. 

## Node
1. Run `brew install node`
2. To install nvm run `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash`

## Yarn
1. Run `npm install -g yarn`

## Firebase
1. Run `npm install -g firebase-tools`
2. Run `firebase login` to login using the UI.

## Applications
1. Rectangle
   - Run `brew install --cask rectangle`
   - Useful to arrange windows.
   - Create macros.
2. Numi
   - Run `brew install --cask numi`
   - Better calculator
3. Telegram
   - Run `brew install --cask telegram`
   - Better messaging application.
4. Insomnia
   - Run `brew install --cask insomnia`
   - Testing API endpoints.
5. Insomnia Designer
   - Run `brew install --cask insomnia-designer`
   - API design.

## TODO
- Add databases