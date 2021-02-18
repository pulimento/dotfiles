# PowerShell prompt theming and customization

- [MS docs](https://docs.microsoft.com/en-us/windows/terminal/tutorials/powerline-setup#customize-your-powershell-prompt)
- [oh-my-posh docs](https://ohmyposh.dev/docs/installation)

## TL,DR on setup powerline

````
Install-Module posh-git -Scope CurrentUser
Install-Module oh-my-posh -Scope CurrentUser
Install-Module -Name PSReadLine -Scope CurrentUser -Force -SkipPublisherCheck
````

## Customize PS profile

````
notepad $PROFILE
````
Profile:
````
Import-Module posh-git
Import-Module oh-my-posh
Set-PoshPrompt -Theme Agnoster
````

Set font on terminal profile. Key: fontFace.
Oh-my-posh requires Nerd fonts with PowerLine support. Can be found [here](https://www.nerdfonts.com/font-downloads)

I have a custom theme on this repo, that can be set using
````
Set-PoshPrompt -Theme ~/.OhMyPuliTheme.omp.json

````
