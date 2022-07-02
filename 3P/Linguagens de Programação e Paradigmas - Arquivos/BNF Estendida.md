# Problemas da BNF
Apesar da utilidade inicialmente proporcionada pela BNF para a construção de gramática, existem dois _major issues_ nela:
- Muita repetição para acrescentar itens opcionais
- Muita repetição para colocar diversas opções

## Colchetes
Indicam uma parte opcional de algum termo:
![](BNF_colchetes.png)

## Parênteses
Evitam a necessidade constante de recursão e de repetir trechos já escritos:
![](BNF_parenteses.png)

## Chaves
Indicam uma sequência de zero ou mais itens do que estiver especificado dentro da chave:
![](BNF_chaves.png)
