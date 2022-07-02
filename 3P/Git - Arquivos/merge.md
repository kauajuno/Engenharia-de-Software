# Unindo branches
O processo de união de duas branches é importante para quando a versão do código de uma branch é estável e deseja-se que seja implementada à branch master. Nesse caso, utiliza-se o que chamamos de merge.
Para realizar o merge, primeiro precisamos voltar para a branch que sofrerá alterações, que no caso é a branch master:

>$git checkout master

Em seguida, basta executar o comando merge com o nome da branch que deve ser implementada no lugar da master:

>$git merge staging

Em seguida, basta fazer o push.
