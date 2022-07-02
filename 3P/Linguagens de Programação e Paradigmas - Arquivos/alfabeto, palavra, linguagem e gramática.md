# Alfabeto
Conjunto finito de símbolos ou caracteres.
*São alfabetos:*
- (a, b, c)
- (1, 2, 3, 4, 5, 6, 7, 8)
- (a, b, 0, %)
*Não são alfabetos:*
- (a, b, c, ...)
- (1, 2, 3, 4, ...)

## Alfabetos em Linguagens de Programação
- Letras
- Dígitos
- Símbolos
- Brancos/Espaços

## Alfabeto Binário
Alfabeto extremamente reduzido, com apenas dois itens.

# Palavra
Sequência finita da símbolos utilizados de um alfabeto.

## Elementos de uma palavra
### Prefixo
Qualquer sequência de símbolos iniciais de uma palavra.
### Sufixo
Qualquer sequência final de símbolos de uma palavra.
### Subpalavra
Qualquer sequência contígua de símbolos de uma palavra.
### Comprimento
Quantidade de símbolos em uma palavra

*ex:*
Seja w a palavra **abcb** do alfabeto {a, b, c}
- a, ab, abc, abcb e o conjunto vazio são prefixos dessa palavra.
- b, cb, bcb e abcb são sufixos dessa palavra.
- A união dos sufixos e prefixos forma o subconjunto das subpalavras.
- O comprimento |w| é 4.

## Operações sobre palavras
### Concatenação
- Operação binária sobre duas palavras.
- Associa duas palavras.
- É a justaposição da primeira com a segunda.

*ex:*
Sejam v e w respectivamente as palavras aaab e bb do alfabeto {a, b}
vw = aaabbb
v³ = aaabaaabaaab

## Outras propriedades
Seja Σ um alfabeto, Σ* é o conjunto de todas as palavras possíveis sobre esse alfabeto.

# Linguagem Formal
Uma linguagem formal é um subconjunto de Σ*

## L.F. em programação
- Conjunto de palavras chave de uma linguagem de programação
- Conjunto de programas de uma linguagem de programação

# Gramática de Chomsky
Definida por G = (V, T, P, S)
- V: conjunto finito de símbolos, variáveis ou não-terminais
- T: conjunto finito de símbolos, terminais
- P: produções
- S: elemento diferente de V, variável inicial

## Representação de uma regra de produção
A representação de uma regra de produção simples é dada por:
a -> b
Caso a produza mais de uma variável, t.q. a -> b ou a -> c, é possível reproduzir como
a -> b | c

## Exercício de Gramática de Chomsky
Seja G uma gramática t.q.

V: {D, N}
T: {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}
P: {
	N -> D
	N -> DN
	D -> 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9
}
S: {N}

Derivando o número 345

N ->
DN ->
3N ->
3DN ->
34N ->
34D ->
345







