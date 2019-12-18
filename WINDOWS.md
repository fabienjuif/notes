# Windows
## Fonts
- https://www.nerdfonts.com -> hack

## Terminal
- [WSL](https://docs.microsoft.com/fr-fr/windows/wsl/install-win10)
- [Hyper](https://hyper.is)
  * shell config: `shell: 'C:\\Windows\\System32\\wsl.exe'`
  * fontFamily config: `fontFamily: 'Hack, Menlo, "DejaVu Sans Mono", Consolas, "Lucida Console", monospace',`
  * theme: [hyper-material-theme](https://hyper.is/plugins/hyper-material-theme)
  * note that I fall into this issue right now: https://github.com/zeit/hyper/issues/3664#issuecomment-567075446

## VSCode
- Installed from windows
- Plugins
  * [WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)
  * [Icons](https://marketplace.visualstudio.com/items?itemName=emmanuelbeziat.vscode-great-icons)
- **settings.json**
```js
{
    "terminal.integrated.shell.windows": "C:\\Windows\\System32\\wsl.exe",
    "git.autofetch": true,
    "workbench.iconTheme": "vscode-great-icons"
}
```
