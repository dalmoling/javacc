# Documentação da Linguagem ERS

## Índice
1. [Organização Geral do Programa](#organização-geral-do-programa)
2. [Inclusão de Bibliotecas](#inclusão-de-bibliotecas)
3. [Comentários](#comentários)
4. [Declaração de Variáveis Globais](#declaração-de-variáveis-globais)
5. [Método Main](#método-main)
6. [Estruturas de Controle](#estruturas-de-controle)
7. [Entrada e Saída](#entrada-e-saída)
8. [Expressões e Operadores](#expressões-e-operadores)
9. [Return Statement](#return-statement)
10. [Definição de Funções/Procedimentos](#definição-de-funçõesprocedimentos)
11. [Ordem de Execução](#ordem-de-execução)
12. [Exemplos de Código Fonte](#exemplos-de-código-fonte)

---

## Organização Geral do Programa

Elementos obrigatórios e ordem:
1. Inclusões e Comentários (opcional)
2. Declaração de Variáveis Globais (opcional)
3. Método Main (obrigatório)
4. Definição de Funções/Procedimentos (opcional)

---

## Inclusão de Bibliotecas

```c
#include <nome_da_biblioteca>
```

Exemplo:
```c
#include <stdio.h>
```

---

## Comentários

- Linha única:

```c
// Comentário de linha única
```

- Bloco:

```c
/* Comentário
   de bloco */
```

---

## Declaração de Variáveis Globais

```c
tipo identificador [= Expressao];
```

Exemplos:
```c
int idade = 30;
text nome = "ERS";
```

---

## Método Main

```c
int main(int argc, char *argv[]){
    // Corpo do main
    return 0;
}
```

---

## Estruturas de Controle

### if/else

```c
if (Expressao) {
    // comandos
} else {
    // comandos
}
```

### for

```c
for {
    // comandos
}
```

### while

```c
while {
    // comandos
}
```

### foreach

```c
foreach {
    // comandos
}
```

---

## Entrada e Saída

### Entrada

```c
getInt();
getText();
```

### Saída

```c
write(Expressao);
```

Exemplo:
```c
write("Olá, ERS!");
```

---

## Expressões e Operadores

- Atribuição: `=`
- Igualdade: `==`
- Soma/Subtração: `+`, `-`
- Multiplicação/Divisão: `*`, `/`

Exemplos:
```c
x = x + 1;
5 + 3 * 2;
```

---

## Return Statement

```c
return Expressao;
```

Exemplo:
```c
return 0;
```

---

## Definição de Funções/Procedimentos

```c
function nomeDaFuncao(tipo param1, tipo param2){
    // comandos
}
```

Exemplo:
```c
function soma(int a, int b){
    int resultado = a + b;
    write(resultado);
}
```

---

## Ordem de Execução

1. Inclusões e Comentários
2. Declaração de Variáveis Globais
3. Método Main
4. Definição de Funções/Procedimentos

---

## Exemplos de Código Fonte

### Exemplo 1

```c
#include <stdio.h>
/* Programa simples com variável global e main */
int globalVar = 10;
text saudacao = "Olá, Mundo!";

int main(int argc, char *argv[]){
    if( 1 == 1 ){
        write(globalVar);
    } else {
        write(0);
    }
    for {
        write(saudacao);
    }
    getInt();
    getText();
    return 0;
}
```

### Exemplo 2

```c
#include <stdio.h>
int num1 = 5;
int num2 = 15;

int main(int argc, char *argv[]){
    write(num1);
    write(num2);
    return 0;
}

function soma(int a, int b){
    int resultado = a + b;
    write(resultado);
}
```

### Exemplo 3

```c
#include <stdio.h>
text mensagem = "Teste";
int contador = 0;

int main(int argc, char *argv[]){
    if( contador == 0 ){
        write("Iniciando contagem");
    } else {
        write("Contagem inválida");
    }
    while {
        write(contador);
        contador = contador + 1;
    }
    getInt();
    getText();
    return 0;
}

function imprimirTexto(text txt){
    write(txt);
}
```

---

