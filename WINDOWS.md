# Windows
## Utils
- [shell_menu_view](https://www.nirsoft.net/utils/shell_menu_view.html) remove items from the right click context
- [Equalizer APO](https://sourceforge.net/projects/equalizerapo/) I can boost my microphone with this

## Microphone
This section show how to have a clear microphone in all your app (discord/hangout/games/etc)

You have to install these apps and follow screenshots for configuration
- [Reaper](https://www.reaper.fm/download.php) Mixer with some good plugins
- [ASIO4ALL](http://www.asio4all.org/) Audio drivers
- [Virtual cable](https://www.vb-audio.com/Cable/) Audio virtual cables to plug the real microphone to a fake one
<p align="center">
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277400-04e6dc00-7eaa-11ea-9515-0bfa33e0fbd4.png" />
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277447-21831400-7eaa-11ea-9de2-e7e214386cf9.png" />
</p>

<p align="center">
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277628-79217f80-7eaa-11ea-8281-94152e957de4.png" />
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277581-6018ce80-7eaa-11ea-9054-43cbeeff91da.png" />
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277503-3bbcf200-7eaa-11ea-8f3e-124dad833d1a.png" />
</p>

<p align="center">
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277520-437c9680-7eaa-11ea-919c-4a6328390415.png" />
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277538-4b3c3b00-7eaa-11ea-88bf-52cc78b1590e.png" />
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277700-99e9d500-7eaa-11ea-87c1-957ff512467c.png" />
</p>


`control /name Microsoft.Sound`

<p align="center">
<img width=300 src="https://user-images.githubusercontent.com/17828231/79277737-ae2dd200-7eaa-11ea-8444-b23a54f55abb.png" />
</p>


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
