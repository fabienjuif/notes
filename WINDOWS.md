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
- Install it
  - Enable WSL: `dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`
  - Enable Virtual machine feature: `dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart`
  - WSL 2 as default: `wsl --set-default-version 2`
  - Install needed features: `wsl --install`
  - Install https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package
  - Install distribution: `wsl --install -d Ubuntu`
  - Making sur the distribution is in wsl2: `wsl -l -v`
- Update it
  - `sudo apt update`
  - `sudo apt upgrade`
- Install docker ([source](https://nickymeuleman.netlify.com/blog/linux-on-windows-wsl2-zsh-docker))
  - `sudo apt install apt-transport-https ca-certificates curl software-properties-common`
  - `curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`
  - `sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"`
  - `sudo apt update`
  - `sudo apt install docker-ce`
  - `sudo service docker start`
  - `sudo docker run hello-world`
  - Adding your current user to docker group: `usermod -a -G docker $(whoami)`
  - Restart your wsl: `wsl --shutdown` then `wsl`
- Install docker-compose ([source](https://nickymeuleman.netlify.com/blog/linux-on-windows-wsl2-zsh-docker))
  - `sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
  - `sudo chmod +x /usr/local/bin/docker-compose`
  - `docker-compose --version`
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
