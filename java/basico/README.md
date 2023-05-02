## 1. Introdução ao Java

### História e evolução do Java

[...]

### Características e vantagens da linguagem**

Java possui várias características e vantagens que contribuíram para sua popularidade e adoção em larga escala, tais como:

1. **Portabilidade**: Java é independente de plataforma devido à Java Virtual Machine (JVM), que permite que o código seja executado em qualquer sistema operacional que suporte uma JVM.
2. **Orientação a objetos**: Java é uma linguagem fortemente orientada a objetos, o que facilita o gerenciamento de código e a reutilização através de herança, polimorfismo e encapsulamento.
3. **Multithreading**: Java oferece suporte a multithreading, permitindo que os desenvolvedores criem aplicações altamente responsivas e de alto desempenho.
4. **Robustez**: Java possui recursos de tratamento de exceções e gerenciamento de memória automático (garbage collection), o que ajuda a evitar erros e vazamentos de memória.
5. **Segurança**: A linguagem possui recursos de segurança, como o sandbox, que limita o acesso a recursos do sistema e a verificação de tipos em tempo de compilação e execução, minimizando vulnerabilidades.

### Ambiente de desenvolvimento (JDK, JRE, JVM)**

1. **JDK (Java Development Kit)**: O JDK é um conjunto de ferramentas e bibliotecas necessárias para desenvolver, compilar e depurar aplicações Java. Inclui o JRE, o compilador Java (javac) e outras ferramentas, como o JavaDoc e o Java Debugger (jdb).
2. **JRE (Java Runtime Environment)**: O JRE é o ambiente de tempo de execução para aplicações Java. Ele inclui a JVM, bibliotecas Java e outros componentes necessários para executar aplicações Java sem a necessidade das ferramentas de desenvolvimento.
3. **JVM (Java Virtual Machine)**: A JVM é o coração do ambiente de tempo de execução Java. É uma máquina virtual que interpreta e executa o bytecode Java gerado pelo compilador. A JVM é responsável pela alocação de memória, garbage collection e gerenciamento de exceções, além de garantir a portabilidade e segurança da linguagem.


## 2. Sintaxe e Fundamentos

### Estrutura de um programa Java

Um programa Java é composto por uma ou mais classes, e cada classe é um arquivo com a extensão `.java`. Uma classe pode conter variáveis, métodos e construtores. Uma classe Java tem a seguinte estrutura básica:

```java
package com.aulas; // Declaração do pacote (opcional)

import java.util.ArrayList; // Importação de bibliotecas (opcional)

public class ExemploClasse { // Nome da classe (deve começar com letra maiúscula)

    // Variáveis de instância (opcional)
    private int exemplo;

    // Construtor (opcional)
    public ExemploClasse(int exemplo) {
        this.exemplo = exemplo;
    }

    // Métodos (opcional)
    public void setExemplo(int exemplo) {
        this.exemplo = exemplo;
    }

    public int getExemplo() {
        return this.exemplo;
    }

    // Método principal (entry point do programa)
    public static void main(String[] args) {
        // Código do programa
        ExemploClasse obj = new ExemploClasse(10);
        System.out.println("Valor do exemplo: " + obj.getExemplo());
    }
}

```

O método main é o ponto de entrada do programa e deve estar presente em uma das classes. Ele é declarado como public static void main(String[] args).

### **Variáveis e tipos de dados**

Em Java, as variáveis são usadas para armazenar dados. Existem dois tipos de variáveis: primitivas e referências. As variáveis primitivas armazenam valores básicos, enquanto as variáveis de referência armazenam referências a objetos.

**Tipos primitivos:**

1. **`boolean`**: armazena um valor verdadeiro (**`true`**) ou falso (**`false`**).
2. **`byte`**: armazena um valor inteiro de 8 bits (-128 a 127).
3. **`short`**: armazena um valor inteiro de 16 bits (-32.768 a 32.767).
4. **`int`**: armazena um valor inteiro de 32 bits (-2.147.483.648 a 2.147.483.647).
5. **`long`**: armazena um valor inteiro de 64 bits (-9.223.372.036.854.775.808 a 9.223.372.036.854.775.807).
6. **`float`**: armazena um valor decimal de precisão simples de 32 bits.
7. **`double`**: armazena um valor decimal de precisão dupla de 64 bits.
8. **`char`**: armazena um único caractere Unicode de 16 bits.

### **Operadores e expressões**

Os operadores são símbolos que realizam operações sobre os operandos (valores ou variáveis). As expressões são combinações de valores, variáveis e operadores que resultam em um único valor.

**Operadores aritméticos:**

1. **`+`**: adição
2. **``**: subtração
3. **``**: multiplicação
4. **`/`**: divisão
5. **`%`**: resto da divisão (módulo)

**Operadores de comparação:**

1. **`==`**: igualdade
2. `!=`: desigualdade
3. `<`: menor que
4. `>`: maior que
5. `<=`: menor ou igual a
6. `>=`: maior ou igual a

**Operadores lógicos:**

1. `&&`: E lógico (AND)
2. `||`: OU lógico (OR)
3. `!`: NÃO lógico (NOT)

**Operadores de atribuição:**

1. `=`: atribuição simples
2. `+=`: adição e atribuição
3. `=`: subtração e atribuição
4. `=`: multiplicação e atribuição
5. `/=`: divisão e atribuição
6. `%=`: módulo e atribuição

**Operadores unários:**

1. `+`: indica um valor positivo
2. ``: negação (inverte o sinal)
3. `++`: incremento (aumenta o valor em 1)
4. `-`: decremento (diminui o valor em 1)

**Operadores de deslocamento de bits:**

1. `<<`: deslocamento à esquerda
2. `>>`: deslocamento à direita (com sinal)
3. `>>>`: deslocamento à direita (sem sinal)

**Operadores de manipulação de bits:**

1. `&`: E bit a bit (bitwise AND)
2. `|`: OU bit a bit (bitwise OR)
3. `^`: XOR bit a bit (bitwise XOR)
4. `~`: complemento bit a bit (bitwise NOT)

**Operador ternário:**

1. `? :`: operador condicional ternário, que permite escolher entre dois valores com base em uma condição (sintaxe: `condição ? valorSeVerdadeiro : valorSeFalso`)

**Precedência de operadores:**

A precedência de operadores determina a ordem em que as operações são realizadas em uma expressão. Os operadores com maior precedência são avaliados primeiro. A ordem geral de precedência é:

1. Operadores unários
2. Operadores aritméticos
3. Operadores de deslocamento de bits
4. Operadores de comparação
5. Operadores lógicos
6. Operador ternário
7. Operadores de atribuição

Para alterar a ordem de avaliação dos operadores, utilize parênteses `()` para agrupar expressões.
