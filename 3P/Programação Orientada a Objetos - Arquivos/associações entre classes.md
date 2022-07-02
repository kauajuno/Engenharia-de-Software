# Associações entre classes
## UML
A associação entre uma classe e outra classe em UML é representada por uma seta. Vamos nos referenciar aos dois extremos da seta como base e ponta. A classe conectada à base da seta tem como atributo um objeto da classe para qual a ponta da seta está apontando. Isso dispensa a explicitação de que a classe que está contida seja escrita na classe que a contém.

![Digrama em UML representando uma associação entre duas classes](diagrama_UML_introducao.png)

Também é possível representar o nome utilizado para nomear o objeto daquela classe filha na classe mãe:

![Diagrama UML representando associação de classes](diagrama_UML_introducao2.png)

Nesse caso, caso uma conta tivesse vários clientes, seria possível representar isso colocando um asterisco ao lado da classe Cliente para a qual a classe Conta está apontando.