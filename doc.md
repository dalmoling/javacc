# Documentação Completa da Linguagem ERS

Esta documentação apresenta todos os elementos e comandos da linguagem de programação ERS, projetada para fins didáticos no estudo de compiladores.

---

## 📚 Índice
- [Introdução](#introdução)
- [Sintaxe Geral](#sintaxe-geral)
- [Comentários](#comentários)
- [Tipos de Dados](#tipos-de-dados)
- [Declaração de Variáveis](#declaração-de-variáveis)
- [Identificadores](#identificadores)
- [Comandos de Decisão](#comandos-de-decisão)
- [Estruturas de Repetição](#estruturas-de-repetição)
- [Entrada de Dados](#entrada-de-dados)
- [Saída de Dados](#saída-de-dados)
- [Procedimentos (Funções)](#procedimentos-funções)
- [Exemplo Completo](#exemplo-completo)

---

## 🚀 Introdução

A **linguagem ERS** é uma linguagem simples e didática, criada para demonstrar conceitos fundamentais na construção de compiladores. Ela abrange desde comandos básicos até funções mais complexas dentro das limitações de regras especificas da ordem geral.

---

## 🔖 Sintaxe Geral

A estrutura básica de um programa ERS deve seguir esta ordem geral:

1. Comentários iniciais
2. Decisões (if/else)
3. Repetições (for/while/foreach)
4. Declaração de variáveis
5. Entrada de dados
6. Saída de dados
7. Procedimentos (funções)

---

## 💬 Comentários

Utilizados para documentar ou explicar o código.

**Comentário de linha:**
```java
// Este é um comentário de linha
```

**Comentário de bloco:**
```java
/* 
  Este é um comentário
  em bloco 
*/
```

---

## 🔢 Tipos de Dados

A linguagem ERS suporta dois tipos primitivos:

| Tipo | Descrição                  | Exemplo       |
|------|----------------------------|---------------|
| int  | Número inteiro             | `int x = 10;` |
| text | Texto (string)             | `text nome = "ERS";` |

---

## 📌 Declaração de Variáveis

Sintaxe geral para declarar variáveis:
```java
tipo identificador = valor;
```

Exemplos:
```java
int idade = 25;
text mensagem = "Olá, mundo!";
```

---

## 🏷️ Identificadores

Identificadores devem seguir as seguintes regras:

- Começar por letra (a-z ou A-Z).
- Podem conter letras, números e sublinhado (_).
- Exemplos válidos: `nome`, `total_1`, `mediaFinal`.

---

## 🎯 Comandos de Decisão

Permitem executar comandos com base em condições:

Sintaxe:
```java
if(condicao){
    // comandos verdadeiros
} else {
    // comandos falsos
}
```

Exemplo:
```java
if(idade > 18){
    write("Maior de idade");
} else {
    write("Menor de idade");
}
```

---

## 🔄 Estruturas de Repetição

Permitem executar comandos repetidamente.

### For
```java
for {
    // comandos repetidos
}
```

### While
```java
while {
    // comandos repetidos
}
```

### Foreach
```java
foreach {
    // comandos repetidos
}
```

Exemplo:
```java
for {
    write("Loop infinito");
}
```

---

## 📥 Entrada de Dados

Permite capturar informações do usuário:

| Comando   | Descrição               | Exemplo      |
|-----------|-------------------------|--------------|
| getInt(); | Lê um valor inteiro     | `getInt();`  |
| getText();| Lê uma string (texto)   | `getText();` |

Exemplo:
```java
getInt();
getText();
```

---

## 📤 Saída de Dados

Utilizado para exibir informações ao usuário:

Sintaxe:
```java
write(expressao);
```

Exemplos:
```java
write("Olá, ERS!");
write(123);
```

---

## ⚙️ Procedimentos (Funções)

Funções permitem encapsular e reutilizar código.

Sintaxe:
```java
function nome(tipo parametro1, tipo parametro2){
    // comandos
}
```

Exemplo prático:
```java
function soma(int a, int b){
    int resultado = a + b;
    write(resultado);
}
```

---

## 📃 Exemplo Completo

```java
/* Exemplo completo da linguagem ERS */

// Decisão (if/else)
if(1){
    write("Condição verdadeira");
} else {
    write("Condição falsa");
}

// Estrutura de repetição
for {
    write("Executando loop");
}

// Declaração de variáveis
int ano = 2024;
text saudacao = "Olá, ERS";

// Entrada de dados
getInt();
getText();

// Saída de dados
write("Finalizando programa");

// Procedimento com parâmetros
function multiplicar(int x, int y){
    int resultado = x * y;
    write("Resultado da multiplicação:");
    write(resultado);
}
```

---  

**Criado com ♥ para aprendizado acadêmico.**
