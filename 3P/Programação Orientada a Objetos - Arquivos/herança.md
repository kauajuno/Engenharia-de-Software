# Herança
O conceito de herança na programação orientada a objetos se trata também do relacionamento e das [[associações entre classes]]. Se trata de classes que são criadas herdando as características de uma outra classe e também tendo suas próprias características.

## Superclasses e subclasses
A classe da qual está sendo herdada recebe o nome de **superclasse**, enquanto a classe que herda recebe o nome de **subclasse**.
Para facilitar o entendimento do conceito de herança, nada como uma boa abstração:
Imagine que temos uma classe Animal, e existem vários tipos de animais para os quais também podemos criar classes, existe Reptil, Artropode, Mamifero... e todos eles tem características em comum, essas características são as características de um animal, que eles herdam da classe Animal. Nesse caso, a superclasse é a classe Animal, e as subclasses são todas as outras mencionadas. Agora, sabendo da classe Mamifero, podemos criar outras classes para representar mamíferos, como Golfinho, Gato, Cachorro... cada um deles possuem características próprias, mas também tem caracterísitcas em comum, características essas que são herdadas da classe Mamifero. Nesse caso, a superclasse é a classe Mamifero, e as subclasses são as demais citadas.

De forma geral, superclasses tendem a trazer características mais gerais, e subclasses trazem características mais específicas. Toda subclasse pode vir a se tornar uma superclasse para novas classes futuras.

## UML
A representação de superclasses e subclasses é dada da seguinte forma em UML:

![Diagrama de superclasse e subclasses em UML](superclassesubclasse.png)

A diferença da representação da herança para o encapsulamento é que, nesse caso, a ponta da seta é preenchida em branco. Mas da mesma forma, a classe na ponta da seta é a que vai ter suas características "estendidas" na classe do outro lado da seta. São omitidas as características herdadas nas subclasses pois é dedutível pelas setas.