# brew-path-zsh
Steps to resolve Homebrew global npm path issues if using **zsh** instead of bash.

## Issue

npm i -g <any_cli_tool>

<any_cli_tool> installs successfully. 

`<cli_tool> --version`
Returns
`zsh: command not found: <cli_tool>`

## Solution

Add
`export PATH="$HOME/.npm-packages/bin:$PATH"`

To your ~/.zshrc file.

### Example

`code ~/.zshrc` paste and save `export PATH="$HOME/.npm-packages/bin:$PATH"`
