**Baseado em C: Como Programar de Deitel**
O Conteúdo a seguir é uma reescrita dos capitulos do livro de deitel adaptados para a linguagem Dart

# Introdução à Programação 
Antes de começarmos, temos que entender que tanto no computador quanto na vida, utilizamos lógica e algoritimos em tudo! mas o que é um algorítmo?
 - É uma linguagem intermediária entre a linguagem humana e as linguagens de programação
 - É a especificação de uma sequência ordenada de instruções, finitas e não-ambíguas, que deve ser seguida para a solução de um determinado problema, garantindo a sua repetibilidade

Complicado né? Um algoritmo é um conjunto de instruções lógicas. É como uma receita de bolo: você segue as etapas na ordem correta e obtém o resultado desejado. Nos computadores, os algoritmos são usados para realizar várias tarefas, desde somar números até navegar na internet. Eles são a base de tudo o que os computadores fazem!

Sabendo disso, não é interessante utilizarmos linguagens intermediárias para entendermos esse conceito, por isso estaremos já seguindo com uma linguagem de programação, o Dart.

O Dart usa algumas notações que podem parecer estranhas às pessoas que não programaram computadores. Começamos examinando um programa simples em Dart. Nosso primeiro exemplo imprime uma linha de texto.



```dart
// Primeiro Programa em Dart!

void main() {
  print('Bem vindo ao Dart!');
}
```

SAIDA DO PROGRAMA (O QUE APARECERÁ QUANDO O PROGRAMA FOR EXECUTADO, TAMBÉM CHAMADO DE OUTPUT): **Bem-vindo ao Dart!**

Apesar de este programa ser muito simples, ele ilustra muitos aspectos importantes da linguagem Dart. Agora vamos examinar detalhadamente cada linha do programa.

A linha: _**// Primeiro Programa em Dart!**_ 
Começa com // indicando que é um comentário. Os programadores inserem comentários para documentar os programas e melhorar sua legibilidade. Os comentários não fazem com que o computador realize qualquer ação quando o programa é executado. Os comentários são ignorados pelo Dart e não fazem com que seja gerado nenhuma saída (quando o programa é executado, aquela linha de comentário não executa nenhuma ação). O comentário Primeiro programa em Dart descreve simplesmente o objetivo do programa. Os comentários também servem de auxílio para outras pessoas lerem e entenderem seu programa, mas muitos comentários podem tornar um programa difícil de ler.

