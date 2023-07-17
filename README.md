# salliii.omp


## Install <a href="https://ohmyposh.dev/docs/installation/windows">oh-my-posh</a>
First, you have to install <a href="https://ohmyposh.dev/docs/installation/windows">oh-my-posh</a> on your local machine.

### Windows PowerShell
```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```

### Linux
```bash
brew install jandedobbeleer/oh-my-posh/oh-my-posh
```

<br>

## Install Nerd Font
You have to install a Nerd font, otherwise, you might encounter character issues.
For that, oh-my-posh can be used:
```bash
oh-my-posh font install
```
Choose one of the displayed fonts and wait until the installation is completed.
After that, you need to set the desired font in your console settings. Visit <a href="https://ohmyposh.dev/docs/installation/fonts#configuration">oh-my-posh</a> for further information.

<br>

## Change Prompt
To use the desired theme, you need to make a few changes to the console's profile files.
Visit <a href="https://ohmyposh.dev/docs/installation/prompt">oh-my-posh</a> for the full configuration options.

### Windows PowerShell
Open the PowerShell profile script using the following command. You can replace notepad with any other text editor of your choice.
```powershell
notepad $PROFILE
```

Insert the following line into the script and replace <path_to_file> with the path to the file or with "$env:POSH_THEMES_PATH."
```powershell
oh-my-posh init pwsh --config "<path_to_file>\salliii.omp.json" | Invoke-Expression
```

Reload the shell by executing the following command.
```powershell
. $PROFILE
```

### Linux
Open the .bashrc file using the following command. You can replace notepad with any other text editor of your choice.
```bash
notepad ~/.bashrc
```

Insert the following line into the script and replace <path_to_file> with the path to the file
```bash
eval "$(oh-my-posh init bash --config "<path_to_file>\salliii.omp.json")"
```

Reload the terminal by executing the following command.
```bash
exec bash
```