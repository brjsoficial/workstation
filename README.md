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

Para mais informações sobre Node.js: http://brjs.com.br/instalando-node-js-windows-e-linux/ e http://brjs.com.br/node-js-6/
Para quem está usando Node.js no Windows: https://www.youtube.com/watch?v=Hp6jOsoJtHY
Para instalar o Node.js e NPM basta executar os comandos abaixo:

```bash
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
sudo apt-get install -y build-essential
```

Para verificar se a instalação foi realizada com sucesso digite

```bash
node -v
```

# Instalando o MongoDB

Para instalar o MongoDB basta executar os comandos abaixo:

```bash
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
echo "deb http://repo.mongodb.org/apt/ubuntu "$(lsb_release -sc)"/mongodb-org/3.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list
sudo apt-get update
sudo apt-get install -y mongodb-org
```

Para verificar se a instalação foi realizada com sucesso digite: 

```bash
service mongod status
```

# Instalando o Redis

Para instalar o Redis basta executar os comandos abaixo:

```bash
sudo apt-get update
sudo apt-get install tcl8.5
wget http://download.redis.io/releases/redis-stable.tar.gz
tar xzf redis-stable.tar.gz
cd redis-stable
make
make test
sudo make install
cd utils
sudo ./install_server.sh
sudo service redis_6379 start
```

# Instalando o Elastic Search

Para mais informações sobre o Elastic Search: http://brjs.com.br/elastic-search-mongodb-node-js/
Para instalar o Elastic Search basta executar os comandos abaixo: 

```bash
sudo apt-get install openjdk-7-jre
wget https://download.elastic.co/elasticsearch/elasticsearch/elasticsearch-1.7.2.deb
sudo dpkg -i elasticsearch-1.7.2.deb
sudo update-rc.d elasticsearch defaults
sudo service elasticsearch start
cd /usr/share/elasticsearch
sudo bin/plugin --install com.github.richardwilly98.elasticsearch/elasticsearch-river-mongodb/1.6.0
sudo bin/plugin --install elasticsearch/elasticsearch-mapper-attachments/1.6.0
sudo bin/plugin --install mobz/elasticsearch-head
sudo bin/plugin --install lukas-vlcek/bigdesk
sudo service elasticsearch restart
```

# Instalando o Phonegap

Para mais informações sobre o Phonegap: http://brjs.com.br/app-em-20min-com-phonegap/
Para instalar o Phonegap basta executar os comandos abaixo: 

```bash
npm install -g phonegap@latest
```

# Instalando o NW.JS

Para instalar o NW.JS basta executar os comandos abaixo: 

```bash
npm i -g nwjs
```

# Instalando o Git

Para instalar o Git basta executar os comandos abaixo: 

```bash
sudo apt-get install git
```


