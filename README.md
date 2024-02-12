# Comandos para atualização em geral por Terminal

<br
/>

## Clique na seta para abrir os comandos

<details
>
  <summary
  ><strong
  >
    Ubuntu & pacotes de sistemas</strong></summary>

<br
  />

## Atualizar os pacotes do sistema *** __Usar Este__ ***

    sudo apt install ubuntu-restricted-extras

<br
/>

## Atualizar os pacotes do sistema

    sudo apt-get update && sudo apt-get dist-upgrade

<br
/>

## Baixar e Atualizar os pacotes do sistema

<p
  >Atualização Full</p>

    sudo apt update && sudo apt full-upgrade --install-recommends

<br
  />
  
  ## Instalar ou Atualizar um pacote (Vscode ou qualquer outro)

<p
  >Simulando Atualização do vscode</p>

    sudo dpkg -i
    
<p> 

  Exemplo: sudo dpkg -i code_1.77.3-1681292746_amd64.deb o código foi baixado no diretorio especifico e dentro do diretorio coloquei o comando

</p>

<br
  />

## Comando abaixo vai reinicializar sua máquina

> <p
> >sudo reboot</p>

<br
  />

## Comando abaixo vai instalar na sua máquina o update-manager-core

> <p
> >sudo apt-get install update-manager-core</p>

<br
  />

## Comando abaixo vai editar o arquivo /etc/update-manager/release-upgrades

<h4
>Faça uma cópia de segurança antes</h4>
  
  > <p
  > >sudo apt-get install update-manager-core</p>

<br
  />

## Visualize o arquivo /etc/update-manager/release-upgrades, antes de editá-lo

> <p
> >cat /etc/update-manager/release-upgrades</p>

    Se aparecer [Prompt=never] na ultima linha quer dizer que ele nunca vai atualizar sozinho, se quiser que atualize utilize o comando abaixo.

<br
  />

## Comando abaixo vai atualizar seu prompt

<h5
>Normal</h5>
  
  > <p
  > >sudo sed -i 's/Prompt=normal/Prompt=lts/g' /etc/update-manager/release-upgrades</p>

<br
  />

<h5
>Never</h5>
  
  > <p
  > >sudo sed -i 's/Prompt=normal/Prompt=lts/g' /etc/update-manager/release-upgrades</p>

<br
  />

## Iniciar o processo de atualização

> <p
> >sudo do-release-upgrade -d</p>

<br
  />

## Reconfigurar para ABNT2 o Teclado Americano 104 teclas

> <p
> >setxkbmap -model abnt2 -layout br</p>

<br
  />

## Reconfigurar o bash para o teclado

> <p
> >

setxkbmap -model pc104 -layout us_intl

  </p>

<br
  />

## Verificar a versão do Ubuntu

> <p
> >

lsb_release -a</p>

<br
  />

</details>

<hr
/>

<br
/>

<details
>
  <summary
  ><strong
  >
    Discos Bootaveis</strong></summary>

<br
  />

# Atenção este procedimento vai apagar e formatar o seu Pen Drive

## Baixar o pacote da Balena

#### Etcher (oficialmente chamado balenaEtcher) é uma ferramenta que condensa todo o processo de gravação de imagens de disco em unidades USB ou SD externas em um único local.

##### Salve onde achar mais apropriado

    https://etcher.balena.io/#download-etcher

<br
/>

## Deixe o arquivo executável

#### Entre no diretório salvo e em seguido digite o comando abaixo

    chmod +x balenaEtcher-1.18.11-x64.AppImage

<br
/>

## Executar o balenaEtcher

    ./balenaEtcher-1.18.11-x64.AppImage

<br
/>


## Após isso baixe a iso do sistema operacional que quer utilizar e siga os passos que o programa indica:

#### 1. Selecionar a imagem iso baixada pelo:
### Flash from file

<br
/>

#### 2. Escolher o lacal que vai salvar (USB)
## Este programa vai apagar tudo do pen driver ou qualquer outro local que você vai fazer. 

#### 3. Vai inicializar o programa

<br
/>
