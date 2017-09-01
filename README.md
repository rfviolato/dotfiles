# 1. Install essential code stuff
* Go to [strap](https://github.com/mikemcquaid/strap) repo to download personalized script and follow instructions. Installation may take a while.
**Note: Close Apple App Store because strap may need to update your OS and it may crash the script if update is being downloaded**

# 2. Generate SSH Key
* Open terminal
* Copy/paste and press enter: `$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
* After the key is generated, enter this command: `$ pbcopy < ~/.ssh/id_rsa.pub`
* Go to [Github Profile Keys](https://github.com/settings/keys) and paste the key

For any more help go to this [Github guide](https://help.github.com/articles/connecting-to-github-with-ssh/).

# 3. Install Brewfile
In order to install al the contents of a `Brewfile` you need to install Homebrew `bundle` tap.
* To install the tap, in the terminal enter this command: `$ brew tap Homebrew/bundle`
* Clone this repo: `git@github.com:rfviolato/dotfiles.git`
* Enter repo folder and enter this command: `$ brew bundle`.

# 4. Display hidden files in Finder
* In the terminal, enter the this command: `defaults write com.apple.finder AppleShowAllFiles YES`
* Relaunch Finder, to do so hold the 'Option/alt' key, then right click on the Finder icon in the dock and click Relaunch.

# 5. Hyperterm theming
* NPM install [pure theme](https://github.com/sindresorhus/pure): `npm install --global pure-prompt`
* Install Oh-my-zsh by entering this command
```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

* Be sure you have opened Hyper once to generate a hyper.js file
* Copy both _.zshrc_ and _.hyper.js_ file contents and replace the orignal content in each file in the root of your User folder
* Inside the _.zshrc_ file, replace _rfviolato_ entries with the macbook username.

# 6. Git config
* Copy/paste the contents of this repo _.gitconfig_ file into the OS user root original file.

# 7. Setting up VSCode
* Launch VS Code
* Open the Command Palette (⇧⌘P (Windows, Linux Ctrl+Shift+P)) and type 'shell command' to find the Shell Command: Install 'code' command in PATH command
* Press ⌘ + `,` for settings
* Copy/paste _.vscode/settings.json_ content into the right column.
