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
