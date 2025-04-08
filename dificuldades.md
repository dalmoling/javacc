# Principais Dificuldades na Implementação da Linguagem

## Dificuldades no método SKIP

Uma das dificuldades mais complexas enfrentadas foi ajustar o método `SKIP` dentro do arquivo `ERS.jj`. A finalidade do método é simples: ignorar espaços, quebras de linha, tabulações e outros caracteres em branco. Porém, a implementação inicial falhava repetidamente, causando erros persistentes no reconhecimento dos espaços em branco pelo parser. 

Foram necessárias múltiplas revisões e ajustes minuciosos até alcançar a sintaxe correta, garantindo que caracteres vazios fossem efetivamente ignorados, permitindo ao parser interpretar corretamente os comandos da linguagem.

---

## Implementação da Inclusão de Bibliotecas (`#include`)

Outra dificuldade significativa envolveu a implementação da inclusão de bibliotecas devido ao uso do caractere especial `#`. Inicialmente, o parser tinha dificuldade em distinguir claramente o símbolo de inclusão das outras partes do código, resultando em falhas ao reconhecer corretamente declarações como:

```c
#include <stdio.h>
```

A solução exigiu uma revisão completa da definição dos tokens, criando uma regra específica para o reconhecimento correto da diretiva `#include`. Essa modificação permitiu ao parser identificar corretamente quando uma biblioteca estava sendo declarada, resolvendo definitivamente o problema.

---

## Implementação do Comando `return`

Implementar corretamente o comando `return` também se mostrou desafiador. Inicialmente, o parser não conseguia reconhecer o comando adequadamente, exigindo a criação de uma função específica dentro do arquivo `ERS.jj` para tratar explicitamente o reconhecimento e a interpretação desse comando.

Além disso, foi necessário revisar a estrutura das expressões e a gramática de comandos para permitir a integração correta do `return` em diferentes contextos (como dentro do método `main` ou funções definidas pelo usuário), garantindo que o comando funcionasse de maneira consistente e previsível.

------------------
Outro problema relevante também foi  definir a Hierarquia de Operadores nas Expressões
