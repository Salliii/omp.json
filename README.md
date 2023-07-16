# salliii.omp

## Windows
### install oh-my-posh

```powershell
winget install oh-my-posh
winget install XP8K0HKJFRXGCK
winget upgrade oh-my-posh
oh-my-posh version
```

### clone this theme

```powershell
git clone https://github.com/Salliii/salliii.omp.git
```

### apply this PowerShell theme

Execute the following command. You can replace `notepad` by any code editor.
```powershell
notepad $PROFILE
```
Add the following line to the file and replace `<path_to_file>` with the path to the cloned git repo.
```powershell
oh-my-posh init pwsh --config "<path_to_file>\salliii.omp.json" | Invoke-Expression

```

### install nerd font

To avoid unicode character problems you have to install a nerd font. I recommend the CaskaydiaCove Nerd font.
https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/CascadiaCode.zip