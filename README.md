# salliii.omp

## Windows
### install oh-my-posh

```powershell
winget install oh-my-posh
winget install XP8K0HKJFRXGCK
winget upgrade oh-my-posh
oh-my-posh version
```

### clone omp theme

```powershell
git clone https://github.com/Salliii/salliii.omp.git
```

### apply the PowerShell theme

Execute the following command. You can replace `notepad` by any code editor.
```powershell
notepad $PROFILE
```
Add the following line to the file and replace `<path_to_file>` with the path to the cloned git repo.
```powershell
oh-my-posh init pwsh --config "<path_to_file>\salliii.omp.json" | Invoke-Expression

```