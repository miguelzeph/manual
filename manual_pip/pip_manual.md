# PIP (Gerenciador de Pacotes)

### Ver versão:
pip --version
### Ver a bibliotecas instaladas pelo pip
pip list ou pip freeze
### Procurar por biblioteca (linux)
pip list | grep -i "nome"
### Instalar
sudo pip install numpy

OBS: não utilizar SUDO quando estiver em uma virtualenv
### Desinstalar
sudo pip uninstall numpy

OBS: não utilizar SUDO quando estiver em uma virtualenv

### Várias Versões de Python
Quando tiver mais de uma versão de python você precisa instalar os pip por elas... quando for chamar os comandos no temrinal: pip3.7 ... pip3.6 ... etc

### Requirements.txt - install
Muitas vezes você clona repositórios que tem um arquivo chamado 'requirements.txt', pode executar o comando abaixo para instalar tudo diretamente

pip install -r requirements.txt

### Requirements.txt - gerar
pip freeze > requirements.txt





