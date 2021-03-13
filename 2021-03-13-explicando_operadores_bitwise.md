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

Se você não sabe como fazer conversão de números decimais para binário, recomendo ler algum artigo sobre isso antes de prosseguir na leitura.

## Operadores
A seguir explicarei cada um dos operadores mostrados na seção anterior e você verá que não é tão complicado como parece.

Antes de prosseguirmos com a explicação, é necessário ter em mente que tudo tem a ver com **bits**, 0 e 1, logo, os operadores trabalham em cima de números binários.

### Operador & (bitwise AND)
Este operador compara dois bits e retorna **1** se **ambos os bits forem 1**

Exemplo:
```php
5 & 3  // 1

// 5 em binário = 101
// 3 em binário = 011

  101   // 5
& 011   // 3
= 001   // 1
```

### Operador | (bitwise OR)
Este operador compara dois bits e retorna **1** se **um ou outro bit for 1**

Exemplo:
```php
5 | 3  // 7

// 5 em binário = 101
// 3 em binário = 011

  101   // 5
| 011   // 3
= 111   // 7
```
### Operador ^ (bitwise XOR)
Este operador compara dois bits e retorna **1** se **os bits comparados forem diferentes**

Exemplo:
```php
5 ^ 3  // 6

// 5 em binário = 101
// 3 em binário = 011

  101   // 5
^ 011   // 3
= 110   // 6
```
### Operador << (bitwise left shift)
### Operador >> (bitwise right shift)

## Conclusão
Existem muitas utilidades para operadores Bitwise, algumas delas possibilita você ganhar desempenho em suas aplicações e reduzir o espaço de armazenamento de informações, como por exemplo, permissões em sistemas Unix em que, com apenas **3 bits**, consegue identificar se o usuário tem permissão de escrita, leitura e/ou execução.