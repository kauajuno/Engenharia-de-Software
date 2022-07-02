# Navegando entre versões do código
Por ser uma ferramenta de versionamento de código, nada melhor do que poder navegar entre as versões mais antigas e mais atuais de seu código, e no git de fato é possível fazer isso.
Ao executar o comando:

>$ git reflog

Serão exibidos todas as versões pela qual o código passou, cada qual com seu respectivo ID em hexadecimal. Para que seu código volte a alguma dessas versões, use o comando:

>$ git reset --hard "ID"

Sendo que em ID se coloca o ID da versão que se deseja acessar.