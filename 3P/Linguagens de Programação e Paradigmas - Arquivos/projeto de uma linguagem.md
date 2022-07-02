# Projeto de uma linguagem
Ao se projetar uma linguagem, vários aspectos devem ser levados em conta, dentre eles:
- Arquitetura das máquinas
- Portabilidade
	- Sistemas Legado
	- Máquinas diferentes
- Redigibilidade e legibilidade
	- "Qualquer tolo pode escrever um código que o computador pode entender. Bons programadores escrevem códigos que humanos podem entender" -Kent Beck
- Confiabilidade
- Suporte
- Abstração

Vamos dar uma breve aprofundada em cada um desses aspectos.

## Arquitetura das máquinas
Um aspecto que costumava ser mais levado em conta antigamente e que explica a razão pela qual a maioria das primeiras linguagens de programação a serem criadas são de paradigma procedural. Isso se dá em razão da arquitetura de Von Neumann, que operava sequencialmente com as instruções que recebia, modelo que casava muito bem com o paradigma de programação procedural.

## Portabilidade
Portabilidade diz respeito à capacidade de uma linguagem de programação de rodar em uma variedade de dispositivos e sistemas diferentes.

### Sistemas Legado
Em linguagens de programação, é muito difícil remover alguma ferramenta construída pois é necessário promover o funcionamento de sistemas construídos em versões anteriores daqueal linguagem de programação. Portanto, é importante que uma linguagem de programação, ao longo de seu desenvolvimento, evite remover recursos de versões anteriores e façam adições que de fato façam sentido e não se tornem rapidamente obsoletas.

## Máquinas diferentes
Na era da informação, existe um infinidade de dispositivos diferentes, e é muito importante para uma linguagem popular que ela tenha sua utilidade em cada um deles e possa rodar sem maiores empecilhos.

## Redigibilidade e legibilidade
Um código deve ser entendido pelas máquinas, mas não menos importante que isso ele deve ser preferivelmente fácil de produzir (redigibilidade) e de ser compreendido (legibilidade), visto que a parte mais importante do ciclo de vida de um software é sua manutenção.

## Confiabilidade
Uma linguagem confiável é aquela que sempre entrega as mesmas saídas para suas respectivas entradas independente de outros aspectos variáveis tais como sistema operacional, dispositivo, etc.

## Suporte
Linguagens de programação com bom suporte são aquelas que podem ser facilmente instaladas em um dispositivo, possuem uma quantidade razoável de documentação e tutoriais disponíveis bem como uma comunidade de programadores relativamente grande e que dominam a linguagem em questão.

## Abstração
A abstração é um aspecto das linguagens de programação que fazem a aproximação do código ao mundo real, de forma que a compreensão do código não depende de uma imersão teórica dificultada, bastando um pensamento em alto-nível que agiliza bastante o processo de produção e manutenção do código.