# Workstation

Todos os comandos e links para montar nosso workstation

# Virtualbox

Para quem não utiliza Linux como sistema operacional primário, faça download do Virtual Box pelo link https://www.virtualbox.org/

# Ubuntu 14.04

Para nosso workshop iremos utilizar o Linux Ubuntu 14.04 disponível para download em http://www.ubuntu.com/desktop/developers iremos usar a versão para desenvolvedores, faça download do arquivo .iso x64 ou x32 de acordo com a arquitetura do seu computador.

# Atualização/fix de resolução do Ubuntu no VirtualBox

Para quem estiver usando o Ubuntu no VirtualBox será necessário corrigir o problema de resolução, para isso basta utilizar os comandos abaixo no terminal.

```bash
sudo apt-get update
sudo apt-get install virtualbox-guest-utils virtualbox-guest-x11 virtualbox-guest-dkms
```

Caso ocorra erro de dependência do virtualbox-guest-x11 digite o seguinte comando abaixo:

```bash
sudo apt-get remove libcheese-gtk23
sudo apt-get install xserver-xorg-core
sudo apt-get install -f virtualbox-guest-utils virtualbox-guest-x11 virtualbox-guest-dkms
```

Após a instalação reinicie a maquina virtual

# Instalando o Node.js 6 e NPM

Para instalar o Node.js e NPM basta executar o comando abaixo:

```bash
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y build-essential
```

Para verificar se a instalação foi realizada com sucesso digite

```bash
node -v
```

