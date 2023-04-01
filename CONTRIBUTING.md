# Contributing

This repository and extension are open source in part to encourage contributions. This document exists primarily to let others know how to investigate possible bugs.
## Getting Started

1. Clone this repository
1. Open the repository in VS Code
1. Go to `Run` > `Start Debugging` to open a separate debugging window
1. Create a file with one of the supported [file extensions](README.md#filenames)
1. Type/copy-paste something in the file to test
1. Enable scope inspector
   - Through menu options: `View` > `Command Palette` > `Developer: Inspect Editor Tokens and Scopes`
   - Through keybinding:

      ```json
      {
        "key": "cmd+alt+shift+i",
        "command": "editor.action.inspectTMScopes"
      }
      ```

1. Once enabled click text to see how it's being tagged/scoped

## Publishing

Prerequisite: [`vsce`](https://github.com/microsoft/vscode-vsce#usage)

1. Increment `version` in the `package.json` file based on [SemVar spec](https://semver.org)
1. Add version updates to `CHANGELOG.md`
1. Commit changes as "Prepare release of x.y.z"
1. Cut the tag: `git tag x.y.z`
1. Push the tag: `git push origin x.y.z`
1. Package the extension: `vsce package`
1. Publish the extension: `vsce publish`
1. Create the release on GitHub based on the tag, uploading the new package

## Documentation

- [Visual Studio Code | Syntax Highlight Guide](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide)
