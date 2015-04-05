This is a small wrapper around git that plays sounds effects (currently from Super Mario Bros (NES) or Zelda (NES)) on common commands.
Heavily inspired by Sean Farley's implementation for mercurial (https://bitbucket.org/seanfarley/smb/src)

# Sounds for commands

## Super Mario Bros

- clone: kick
- checkout: stomp
- add: jump
- rm: fireball
- commit: 1up
- push: vine
- pull: pipe
- tag: pause
- error: die

## Zelda

- clone: fanfare
- checkout: secret
- add: get rupee
- rm: sword shoot
- commit: stairs
- push: magical rod
- pull: get item
- tag: recoders
- error: die

# Installation

## Homebrew

1. Tap my homebrew tap: ```$ brew tap pascaldevink/pascaldevink```
2. Update brew: ```$ brew update```
3. Install git-smb: ```$ brew install git-smb```
4. Bonus: put ```alias git=git-smb``` somewhere in your (ba)(z)(k)sh profile to make the wrapping complete and easy

## Manual

1. Clone or download this repository.
2. Either put the bin folder in your path or create a symlink to it (eg. in /usr/local/bin)
3. You can now use it with ```$ git-smb```
4. Bonus: put ```alias git=git-smb``` somewhere in your (ba)(z)(k)sh profile to make the wrapping complete and easy

# Configuration

Locate the config.json file in either <install_path>/etc/config.json (for manual installations) or in /usr/local/etc/git-smb/config.json.
The only configuration currently is the theme, with the following options:
- smb, for Super Mario Bros themed sounds effects
- zelda, for Legend Of Zelda themed sounds effects