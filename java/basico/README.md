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
