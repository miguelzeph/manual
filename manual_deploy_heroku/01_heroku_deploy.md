# Deploy Heroku - Heroku CLI

### 1-) Instalar Heroku
sudo snap install heroku --classic
### 2-) Heroku Login
heroku login (Você precisar ter uma conta no Heroku)
### 3-) Fazer um Repositório no Github
git clone ...link...

### 4-) Criar Ambiente Virtual no Python (ex: python3.6)
virtualenv --python=python3.6 env

* Criamos uma pasta com nome env

### 5-) Crie .gitignore
adicionar a pasta /env/

### 6-) Crie sua Aplicação

### 7-) 4 Arquivos importantes
- runtime.txt: é utilizado para saber qual a versão do python

ex: python-3.6.8

- requirements.txt: mostra as bibliotecas que o sevidor precisa instalar

pip3.6 freeze > requirements.txt

- Procfile: Executa o comando no servidor

ex: web: python nome.py

ex: web: gunicorn nome:app (Flask)

- Pipfile: é uma espécie de nova versão do requirements.txt... não é necessário utilizar quando usar o requirements.txt

dica: crie apenas o <strong>Procfile</strong> e <strong>requirements.txt</strong>

### 8-) Faça o git commit de tudo para o github
git add.

git commit -m "xxxx"

git push

### 9-) Criar um app no Heroku
heroku apps:create NOME

### 10-) Especifique a linguagem utilizada (por garantia)
heroku buildpacks:set heroku/python --app NOME

### OBS: caso já tenha uma aplicação no Heroku e queira usá-la:
heroku git:remote -a NOME

### 11-) Deploy!
git push heroku master

### 12-) Ligar a Aplicação
heroku ps:scale web=1 --app NOME

### 13-) Abrir
heroku open

------------------------------------
### Desligar a Aplicação
heroku ps:scale web=0 --app NOME

### Deixar em modo de manuntenção
heroku maintenance:on --app NOME

### Sair do modo de manuntenção
heroku maintenance:off --app NOME

-------------------------------------






