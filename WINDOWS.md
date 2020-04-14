# Windows
## Utils
- [shell_menu_view](https://www.nirsoft.net/utils/shell_menu_view.html) remove items from the right click context
- [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) I can boost my microphone with this

## WSL2
- [Tutorial on how to install WSL2 with docker](https://nickymeuleman.netlify.com/blog/linux-on-windows-wsl2-zsh-docker)
- [Tutorial on how to use Cypress (or other X window) with WSL2](https://nickymeuleman.netlify.com/blog/gui-on-wsl2-cypress/)
- This alias is useful to now WSL2 IP address (which is dynamic atm): 
  * `alias copip='hostname -I | awk "{print \$1}" | awk "{print \$0}" | clip.exe'`

## Fonts
- https://www.nerdfonts.com -> hack

## Terminal
- [WSL 2](https://docs.microsoft.com/fr-fr/windows/wsl/wsl2-index)
- [Windows Terminal](https://www.microsoft.com/en-us/p/windows-terminal-preview/9n0dx20hk701?activetab=pivot:overviewtab)

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
