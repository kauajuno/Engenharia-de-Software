# Mantendo diferentes versões do código simultaneamente
Em grandes projetos, é comum ver que se trabalha com uma versão de código estável e outras com as quais se faz mais experimentação e tentativas de implementações. Isso é feito por meio das branches.
Cada branch representa uma versão do código que está sendo trabalhado. Geralmente, a branch master seria uma versão estável do código, a mais apta pra uso, na qual só se faz alterações quando há certeza que aquilo não trará problemas de nível major.

## Visualizando as branches
No Git Bash, ao executar o comando:

>$ git branch

Será possível visualizar todas as branches que foram criadas até o momento. Nesse caso, haverá apenas uma branch, que é a branch master.

Entretanto, agora que queremos trabalhar com mais de uma branch, é necessário criar mais uma, à qual daremos o nome de staging. Para isso, vamos rodar o seguinte comando:

>$git branch staging

E ao executarmos o git branch mais uma vez, será possível visualizar as duas branches existentes nesse projeto.

![Branches master e staging](git_branches.png)

Note que a branch master está destacada com um asterisco e em cor verde, isso significa que é a branch na qual qualquer alteração realizada no momento será feita. Para trocar para a branch staging, basta executar o comando:

>$git checkout staging

Em seguida, basta adicionar os arquivos ao versionamento dessa branch, fazer o commit e o push para o GitHub.