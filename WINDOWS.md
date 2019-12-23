# Windows
## Utils
- [shell_menu_view](https://www.nirsoft.net/utils/shell_menu_view.html) remove items from the right click context
- [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) I can boost my microphone with this

## Fonts
- https://www.nerdfonts.com -> hack

## Terminal
- [WSL](https://docs.microsoft.com/fr-fr/windows/wsl/install-win10)
- [Hyper](https://hyper.is) - take a canary version not to fall in the issue below
  * shell config: `shell: 'C:\\Windows\\System32\\wsl.exe'`
  * fontFamily config: `fontFamily: 'Hack, Menlo, "DejaVu Sans Mono", Consolas, "Lucida Console", monospace',`
  * theme: [hyper-material-theme](https://hyper.is/plugins/hyper-material-theme)
  * note that I fall into this issue right now: https://github.com/zeit/hyper/issues/3664#issuecomment-567075446
  * **canary version works** : https://github.com/zeit/hyper/issues/3664#issuecomment-567082287

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

## Drivers
For the HUION 610PRO I use these drivers [H610PRO(2048)](https://www.huion.com/index.php?m=content&c=index&a=lists&catid=16&down_title2=H610PRO).
