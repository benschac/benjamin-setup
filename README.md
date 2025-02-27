# Benjamin Machine Setup

## TODO

create a command that replaces settings.json and keybindings.json if changed (symlink the files)

## Config

```bash
touch ~/.zshrc
```

## Apple OSX Specific

https://vimforvscode.com/enable-key-repeat-vim
then close and reopen app

## Oh My ZSH

https://ohmyz.sh/#install
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Git Config

```bash
touch ~/.gitconfig
```

```bash
cp .gitconfig ~/.gitconfig
```

## Brew Install

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Reference
https://gist.github.com/ChristopherA/a579274536aab36ea9966f301ff14f3f
https://github.com/Homebrew/homebrew-bundle

run `brew bundle install`
Install homebrew (https://brew.sh/)

### Ray Cast

Open Ray CAst

Open system settings

- Keyboard > Spotligth > uncheck `cmd + space`
- Raycast set command `cmd + space`
- order fallback commands using command + k to order your preferences (search first)

### Fonts

### Dank Mono

### Android Emulator Steps

https://docs.expo.dev/workflow/android-studio-emulator/

### Chrome extensions

- React DevTools
- Vimium
- 1password

### Github

- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

`ssh-keygen -t ed25519 -C "benschac@gmail.com"`

`eval "$(ssh-agent -s)"`

`touch ~/.ssh/config`

## TODO

revisit git config

## XCode

expo - common issue: https://github.com/expo/expo/issues/21727#issuecomment-1471621054


## Key Repeat

```bash
defaults write -g InitialKeyRepeat -int 10 # normal minimum is 15 (225 ms)
defaults write -g KeyRepeat -int 1 # normal minimum is 2 (30 ms)
```

Disable press and hold
```bash
defaults delete -g ApplePressAndHoldEnabled    # Unset globally
```

```bash
defaults write -g ApplePressAndHoldEnabled -bool false
```
