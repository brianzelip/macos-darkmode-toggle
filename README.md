# macOS System Preferences dark mode toggle

> Toggle dark/light mode appearance across all apps with one command.

Provided herein is ToggleDarkMode.workflow/, a basic application created with the [Automator app](https://support.apple.com/guide/automator/welcome/mac) on macOS that toggles the System Preferences Appearance between Light and Dark modes.

This is intended to be invoked via the command line using a shell alias instead of manually opening up System Preferences, clicking on Appearance, etc.

## Usage

Clone this repo locally, then update your shell config file with an alias calling `automator` that points to the absolute path of the workflow. For example:

```sh
# .zshrc
alias dark='automator "/Users/${USER_NAME}/Library/Services/ToggleDarkMode.workflow"'
alias light='dark'
```

Then set individual app appearance preferences to 'automatic' to follow your system wide appearance setting. This allows you to toggle appearance across all apps with one command.

## Author

[Brian Zelip](https://zelip.me)
