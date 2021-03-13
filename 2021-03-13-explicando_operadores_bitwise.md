# Explicando operadores Bitwise
## Introdução
Há tempos que eu tentava aprender operadores Bitwise, mas nunca consegui avançar nos estudos por não entendê-los em sua **essência**.

> Os exemplos neste artigo foram feitos utilizando PHP, mas operadores Bitwise existem em praticamente qualquer linguagem de programação.

Operadores Bitwise trabalham com **bits** (nada mais óbvio) e, quando vemos seu retorno em números decimais, acabamo gerando bastante confusão. Por exemplo:
```php
5 ^ 2   // 7
10 & 3  // 2
10 & 4  // 0
5 | 3   // 7
5 << 3  // 40
8 >> 3  // 1
```

**Atenção:** Os operadores bitwise são muito parecidos com os operadores condicionais das principais linguagens de programação, embora seu funcionamento seja um pouco diferente.

O objetivo deste artigo é explicar os principais operadores bitwise da forma em que eu finalmente consegui entendê-los e mostrar o caminho que eu segui para conseguir esclarecê-los em minha mente.

## Um pouco sobre bits e o sistema binário
Antes de explicar como funcionam, é importante que você saiba como trabalhar com números na base 2, também conhecido como números binários.

Um número com base 10 (decimal) significa que cada algarismo pode ir **de 0 até 9**, enquanto números binários, cada algarismo poderá ser **somente 0 ou 1**

Por exemplo:
```
Número decimal: 5
Número 5 binário: 101

Número decimal: 14
Número 14 binário: 1110
```

Neste momento, pretendo explicar somente o essencial sobre números binários para facilitar a compreensão deste artigo.

### Conversão de números decimais para binários

### Conversão de números binários para decimais

## Operadores
A seguir explicarei cada um dos operadores mostrados na seção anterior e você verá que não é tão complicado como parece.

### Operador & (bitwise AND)
### Operador | (bitwise OR)
### Operador ~ (bitwise NOT)
### Operador ^ (bitwise XOR)
### Operador << (bitwise left shift)
### Operador >> (bitwise right shift)

## Conclusão