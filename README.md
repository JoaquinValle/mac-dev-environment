# Development Environment for Mac OS
  - [Mac Settings](#mac-settings)
    - [**File extensions**](#file-extensions)
    - [**Show hidden files**](#show-hidden-files)
    - [**Navbar**](#navbar)
    - [**General Settings**](#general-settings)
  - [Homebrew](#homebrew)
  - [iTerm2](#iterm2)
  - [Git](#git)
  - [Zsh](#zsh)
  - [VS Code](#vs-code)
  - [VS Code Settings](#vs-code-settings)
  - [VS Code Plugins](#vs-code-plugins)
  - [Oh My Zsh](#oh-my-zsh)
  - [Terminal Font - MesloLGS NF](#terminal-font---meslolgs-nf)
  - [Oh My Zsh Theme](#oh-my-zsh-theme)
  - [Zsh Plugins](#zsh-plugins)
  - [Oh My Zsh Plugins](#oh-my-zsh-plugins)
  - [Node](#node)
  - [Yarn](#yarn)
  - [Firebase](#firebase)
  - [Applications](#applications)
  - [Github](#github)
  - [TODO](#todo)

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


## [Homebrew](https://brew.sh/)

Run in terminal `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Run `brew doctor` to verify the installation.

## [iTerm2](https://iterm2.com/)

1. Run in terminal `brew install --cask iterm2`
2. Preferences > Keys > Hotkey > Show/hide all windows with a system-wide hotkey

## [Git](https://git-scm.com/)
Run in terminal `brew install git`

## [Zsh](https://www.zsh.org/)
1. Run in terminal `brew install zsh`
2. Add Zsh to default shell with `sudo vim /etc/shells`
3. Press o to append to new line
4. Add `/usr/local/bin/zsh`
5. Press `esc`
6. Save and quit with `:wq`
7. Run `chsh -s /usr/local/bin/zsh` to change default shell to zsh.
8. Restart terminal.
9. Run `echo $SHELL`. It should return the path to zsh (`/usr/local/bin/zsh`).

## [VS Code](https://code.visualstudio.com/)
1. Run `brew install --cask visual-studio-code`
2. Shell command: Install 'code' command in PATH.

## VS Code Settings
1. [Fira Code Font](https://github.com/tonsky/FiraCode/releases/download/5.2/Fira_Code_v5.2.zip)
2. Font family -> `"editor.fontFamily": "Fira Code"`
3. Font ligatures -> `"editor.fontLigatures": true`

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
    - Add `ZSH_DOTENV_FILE=.env` before Oh my zsh sourcing.
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


## [Oh My Zsh](https://ohmyz.sh/)
1. Run `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
2. Run `code ~/.zshrc` to open the config file.

## Terminal Font - [MesloLGS NF](https://github.com/hayamiz/meslog)

1. Install fonts: 
- [Regular Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
- [Bold Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
- [Italic Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
- [Bold Italic Font](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)
- 
2. iTerm2 > Preferences > Profiles > Text > Font

## Oh My Zsh Theme - [PowerLevel10k](https://github.com/romkatv/powerlevel10k)
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

## Oh My Zsh Plugins
- The plugins should be defined as so: 
  >plugins=(alias-finder git brew copydir copyfile dotenv npm nvm osx z zsh-syntax-highlighting zsh-autosuggestions history-substring-search zsh-completions zsh_reload)
- Do not include any plugins you do not want to install.

1. [Zsh Syntax Highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
   - Highlights commands when typed.
   - Install with git clone `https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`
2. [Zsh Autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
   - Suggests commands based on history.
   - Install with `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
3. [Zsh Substring History Search](https://github.com/zsh-users/zsh-history-substring-search)
   - Search substrings in history.
   - Install with `git clone https://github.com/zsh-users/zsh-history-substring-search ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-history-substring-search`
4. [alias-finder](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/alias-finder)
   - Searches for defined aliases.
5. [brew](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/brew)
   - Brew alias commands.
6. [copydir](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/copydir)
   - Copies current path to clipboard.
7. [copyfile](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/copyfile)
   - Copies file to clipboard.
8.  [dotenv](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/dotenv)
   - Loads .env variables when in root folder.
11. [npm](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/npm)
   - Adds aliases.
11. [nvm](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/nvm)
   - Adds aliases.
11. [osx](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/osx)
   - Adds aliases and utilities.
11. [z](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/z)
   - Tracks most visited directories. 
12. [zsh_reload](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/zsh_reload)
    - Reloads terminal with `src`

## [Node](https://nodejs.org/en/)
1. Run `brew install node`
2. To install nvm run `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash`

## [Yarn](https://yarnpkg.com/)
1. Run `npm install -g yarn`

## [Firebase](https://firebase.google.com/)
1. Run `npm install -g firebase-tools`
2. Run `firebase login` to login using the UI.

## Applications
1. [Google Chrome](https://www.google.com/chrome/)
   - brew `brew install --cask google-chrome`
2. [Firefox](https://www.mozilla.org/en-US/firefox/new/)
   - `brew install --cask firefox`
3. [Rectangle](https://rectangleapp.com/)
   - Run `brew install --cask rectangle`
   - Useful to arrange windows.
   - Create macros.
4. [Numi](https://numi.app/)
   - Run `brew install --cask numi`
   - Better calculator
5. [Telegram](https://telegram.org/)
   - Run `brew install --cask telegram`
   - Better messaging application.
6. [Insomnia](https://insomnia.rest/download/#mac)
   - Run `brew install --cask insomnia`
   - Testing API endpoints.
7. [Insomnia Designer](https://insomnia.rest/download/#mac)
   - Run `brew install --cask insomnia-designer`
   - API design.

## Chrome Extensions
1. [The Great Suspender](https://github.com/aciidic/thegreatsuspender-notrack/archive/7.1.11-notrack.zip)
   - The original extension was flagged as malware and removed; therefore, building the extension from source is required.
   - Click this link [Chrome Extensions](chrome://extensions/)
   - Turn on developer mode.
   - Load unpacked extension.
   - Select src folder.
2. [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm/related)
   - Used to add CSS development tools.
3. [Code Cola](https://chrome.google.com/webstore/detail/code-cola/lomkpheldlbkkfiifcbfifipaofnmnkn/related)
   - Visually edit CSS code. 
4. [Alexa Traffic Ranking](https://chrome.google.com/webstore/detail/alexa-traffic-rank/cknebhggccemgcnbidipinkifmmegdel/related)
   - Check page statistics and traffic.

## [Github SSH Key](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)

1. 
   >`ssh-keygen -t ed25519 -C "your_email@example.com`"           
   >`eval "$(ssh-agent -s)"`     
   >`pbcopy < ~/.ssh/id_ed25519.pub`
2. Add key in Github

## Github Logins
1. Run `git config --global user.name "JoaquinValle"`
2. Run `git config --global user.email "email@example.com"`
3. Run `git config --global pull.ff only`
   
***Add key to keychain if passcode is added.**

## Databases
1. [MongoDB](https://docs.mongodb.com/mongocli/master/configure/#std-label-mcli-configure)
   - Run `brew install --cask mongodb-compass`
   - Run `brew install mongodb/brew/mongodb-community-shell`
   - >`brew tap mongodb/brew`       
     >`brew install mongocli`

2. [MySQL](https://www.mysql.com/)
3. [FaunaDB](https://docs.fauna.com/fauna/current/start/cloud#signup)
   - Run `brew install fauna-shell`
   - Run `fauna cloud-login`
   - Get secret from Database > Security > Keys (If logged suing Github)
4. [GraphQL](https://graphql.org/)
   - Run `npm i -g graphql-cli graphql` to install cli

## Extra Applications
1. [Godot](https://godotengine.org/)
   - Run `brew install --cask godot`

## TODO
- Add databases
- Other VS Code extensions
- Other mac applications
- CLI Tools

