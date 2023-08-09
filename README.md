# Oh-my-posh

Welcome, this repository is intended to demonstrate how I customized my PowerShell terminal in Windows Terminal and Visual Studio Code.

## Início

Primeiramente você precisará ter instalado o [Windows Terminal](https://aka.ms/terminal), que pode ser encontrado na Microsoft Store. Após a instalação, siga os passos abaixo para configurar o Oh-my-posh.

### Passo 1: Instalar o PowerShell

```markdown
1. Instale o [Powershell](https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D?hl=pt-br&gl=br) através da Microsoft Store.

### Passo 2: Instalar o oh-my-posh

1. Abra o PowerShell no qual você instalou anteriormente.
2. Execute os seguintes comandos para instalar o módulo 'oh-my-posh':

```powershell
Install-Module oh-my-posh -Scope CurrentUser
```

3. Execute o seguinte comando para verificar as fontes disponiveis:

```powershell
get-PoshThemes
```

4. Instale uma fonte de energia (theme) do Oh-my-posh. Por exemplo, para instalar o tema agnoster, execute o seguinte comando:

```powershell
Install-PoshTheme agnoster
```
