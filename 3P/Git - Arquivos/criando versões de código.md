# Primeiro commit
Para criar a primeira versão do recém-criado código, é necessário rodar a seguinte linha de código:

>$ git commit -m "First commit"

Na verdade, o que é passado entre as aspas é uma mensagem sobre o que se trata o commit, logo o que for escrito não altera o funcionamento do comando, mas é importante para a documentação do código.

![First commit](git_commit_inicial.png)

# Subindo para a nuvem
Pela primeira vez, estaremos de fato utilizando o GitHub, pois enviaremos nosso código pra lá. Isso é feito via comando git push. Porém, antes de executar esse comando, é necessário fornecer ao git o link do repositório online para o qual seu código será enviado. Para isso, deve-se rodar o comando:

>$ git remote add origin linkdorepositorio

E depois, para subir a primeira versão do código para a branch master, é executado o comando:

>$ git push --set-upstream origin master

[g](google.com)