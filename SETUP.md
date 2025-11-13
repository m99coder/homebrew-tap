# How to create and maintain a tap

- <https://docs.brew.sh/How-to-Create-and-Maintain-a-Tap>
- <https://github.com/Homebrew/homebrew-cask/blob/main/Casks/a/alacritty.rb>

```shell
# create tap
brew tap-new m99coder/homebrew-tap
brew install gh
gh repo create m99coder/homebrew-tap --push --public --source "$(brew --repository m99coder/homebrew-tap)"

# create formula or cask
brew create https://github.com/alacritty/alacritty/releases/download/v0.16.1/Alacritty-v0.16.1.dmg --tap m99coder/homebrew-tap --set-name m99coder-alacritty

# or rather copy from the original formula and
# remove the `disable!` line
```
