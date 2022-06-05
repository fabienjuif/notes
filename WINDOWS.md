# Windows
## Utils
- [shell_menu_view](https://www.nirsoft.net/utils/shell_menu_view.html) remove items from the right click context
- [add administrator apps at startup](https://superuser.com/questions/929225/how-to-run-a-program-as-an-administrator-at-startup-on-windows-10)

## Microphone
This section show how to have a clear microphone in all your app (discord/hangout/games/etc)

You have to install these apps and follow this video tutorial for configuration: [video from  VancityGames ](https://www.youtube.com/watch?v=J3fBx2ftaBs)
- [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) Mixer with some good plugins
- [Plugins VST](https://www.reaper.fm/reaplugs/)

My app configuration is in the repositiory and you can found yours in `C:\Program Files\EqualizerAPO\config\config.txt`

## WSL2
- Enable WSL: `dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`
- Enable Virtual machine feature: `dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart`
- WSL 2 as default: `wsl --set-default-version 2`
- Install needed features: `wsl --install`
- _restart_
- Install distribution: `wsl --install -d Ubuntu`

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
  * [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)
  * [Palenight Theme](https://marketplace.visualstudio.com/items?itemName=whizkydee.material-palenight-theme)
  * [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
- **settings.json**
```js
{
    "git.autofetch": true,
    "workbench.iconTheme": "vscode-great-icons",
    "workbench.colorTheme": "Palenight Theme",
    "editor.tabSize": 2,
    "javascript.updateImportsOnFileMove.enabled": "never",
    "window.zoomLevel": 1
}
```

## Drivers
For the HUION 610PRO I use these drivers [H610PRO(2048)](https://www.huion.com/index.php?m=content&c=index&a=lists&catid=16&down_title2=H610PRO).
