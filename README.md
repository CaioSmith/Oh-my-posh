# Oh-my-posh

Welcome, this repository is intended to demonstrate how I customized my PowerShell terminal in Windows Terminal and Visual Studio Code.

## Início

Primeiramente você precisará ter instalado o [Windows Terminal](https://aka.ms/terminal), que pode ser encontrado na Microsoft Store. Após a instalação, siga os passos abaixo para configurar o Oh-my-posh.

### Passo 1: Instalar o PowerShell

1. É recomendável instalar o [Powershell](https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D?hl=pt-br&gl=br) através da Microsoft Store.

### Passo 2: Instalar o oh-my-posh

1. Abra o PowerShell no qual você instalou anteriormente.
2. Execute os seguintes comandos para instalar o módulo 'oh-my-posh':

```powershell
Install-Module oh-my-posh -Scope CurrentUser
```

### Passo 3: Configurar o oh-my-posh

1. Crie o arquivo de perfil do Powershell:

```powershell
if (!(Test-Path -Path $PROFILE )) { New-Item -Type File -Path $PROFILE -Force }
```
2. Agora digite o comando:

```powershell
./notepad $PROFILE
```

3. Cole o seguinte comando para inicializar o oh-my-posh no seu terminal:

```powershell
oh-my-posh init pwsh | Invoke-Expression
```

Pronto, com isso o oh-my-posh já vai estar configurado no seu terminal!

### Passo 4: Instalar uma fonte

# Caso o seu terminal oh-my-posh não esteja esteticamente atraente, faltando ícones ou etc, siga os seguintes passos

1. Acesse [Nerd Fonts](https://www.nerdfonts.com/)
2. Ao entrar no site, clique em Download.
3. Selecione a fonte na qual deseja e clique em Download, recomendo instalar CaskadyaCove Nerd Font.
4. Ao instalar a fonte, extraia o arquivo na qual você a instalou.
5. Após extrair, selecione todos os arquivos presente, menos os arquivos LICENSE.md e readme.md
6. Com os arquivos selenionados, clique com o botão direito do mouse e clique em "instalar".

### Passo 1.1: Configurar a fonte no Windows Terminal