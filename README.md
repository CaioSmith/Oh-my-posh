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

## Caso o seu terminal oh-my-posh não esteja esteticamente atraente, faltando ícones ou etc, siga os seguintes passos
## Passo 1: Realizar download da fonte

1. Acesse [Nerd Fonts](https://www.nerdfonts.com/)
2. Ao entrar no site, clique em Download.
3. Selecione a fonte na qual deseja e clique em Download, recomendo instalar CaskadyaCove Nerd Font.
4. Ao instalar a fonte, extraia o arquivo na qual você a instalou.
5. Após extrair, selecione todos os arquivos presente, menos os arquivos LICENSE.md e readme.md
6. Com os arquivos selenionados, clique com o botão direito do mouse e clique em "instalar".

### Passo 2: Configurar a fonte no Windows Terminal

1. Abra as configurações do seu terminal Windows:

![iamgem_config](https://github.com/CaioSmith/Oh-my-posh/blob/526d4acf8b55034183c80ee40b3cb97289017cda/image_git.png)

2. Clique em "Abrir o arquivo json"

![imagem_config](https://github.com/CaioSmith/Oh-my-posh/blob/b4d1013252249b50fc92ada0c07f1e289e23371b/image_config_pwsh.png)

3. Agora procure por "defaults" e coloque as seguintes linhas:

```json
"defaults": {
            "font": 
            {
                "face": "CaskaydiaCove Nerd Font",
                "size": 10
            }
}
```

## Feito isso seu terminal estará pronto. Agora vamos ver como alterar o tema oh-my-posh!

1. Primeiro digite o seguinte comando para visualizar a variedade de temas disponiveis: 
```powershell
get-PoshThemes
```

1.1 Ou se vá no próprio site do [oh-my-posh](https://ohmyposh.dev/docs/themes) para visualizar os temas liberados!

2. Ao encontrar um tema atraente, altere o arquivo de perfil do powershell para setar o tema no qual você se interessou:
```bash
oh-my-posh init pwsh --config='$env:POSH_THEMES_PATH/jandedobbeleer.omp.json' | Invoke-Expression
```

2.1 Altere "jandedobbeleer.omp.json" pelo tema que você quer!

## Configurar o terminal no Visual Studio Code

### Passo 1: Abrir arquivo "settings.json" do Visual Studio Code

1. No VSCode, digite o comando "Ctrl + Shift + P"
2. Pesquise por "settings.json":

![Image_config_vscode](https://github.com/CaioSmith/Oh-my-posh/blob/ee638773a927f499e7a0be81f3bb8a132d3149bb/config_vscode.png)

3. no arquivo json, digite a seguinte linha ao final do arquivo:

```json
"terminal.integrated.fontFamily": "CaskaydiaCove Nerd Font"
```

#### Feito isso, agora tanto o Windows Terminal quanto o Visual Studio Code e estarão configurados para utilizar o oh-my-posh!

## Configurar Temas de ícones
#### Se você estiver no Windows, digite o comando "dir" no seu terminal, verá os arquivos que estão presentes no seu diretório atual, existe uma forma de personalizar a aparência dos ícones, vamos ver!

### Passo 1: 

