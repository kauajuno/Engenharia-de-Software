# Status
Uma vez inicializado o repositório, podemos começar a adicionar os arquivos com os quais trabalhamos. Feito isso, ao rodar o Bash de novo e executar o comando:

>$ git status

Será informado que ainda não foi realizado commit algum e que os arquivos não estão sendo monitorados:

![Repositório git com um único arquivo](git_repo.png)

![Git Bash após rodar o git status pela primeira vez](git_status_intro.png)

Para adicionar, basta fazer como o próprio Bash informa e rodar o comand git add com o nome do arquivo em seguida, que nesse caso é:

>$ git add "Intro.txt"

![Adicionando arquivo ao versionamento de código](git_add.png)

Entretanto, na grande maioria das vezes se trabalha com muitos arquivos, o que acaba inviabilizando adicionar um de cada vez. Portanto, para adicionar todos os arquivos daquele repositório ao controle de código, basta rodar o comando git add da seguinte forma:

>$ git add .

![Novos arquivos no repositório](git_novos_arquivos.png)

![Adicionando vários arquivos](git_add_all.png)
