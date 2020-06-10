# Escondendo Informações Importantes (Senhas/Keys)

<font color = 'red'>obs: Deixe sempre por último essa etapa</font>

### 1-) Add as senhas em um arquivo a parte
### 2-) Add este arquivo no seu .gitignore
### 3-) Agora a Senha está segura...

##### Se os dados estão no gitignore, como heroku irá ter acesso?

### 4-) Para isso, você deve configurar as Variáveis no servidor Heroku.
heroku config:set MINHA_VAR=xxxx 

(dica: Por precaução no script Python use sempre entre str() para o código entender que é uma string...)

ou

Vá na plataforma heroku -> escolha seu repositório -> settings -> Reveal Config Vars

### 5-) Visualizar as confi vars que você add
heroku config

### 6-) No Python, como chamar as variáveis
exemplo:

minha_senha = str(os.environ["MINHA_VAR"])

print(minha_senha)







