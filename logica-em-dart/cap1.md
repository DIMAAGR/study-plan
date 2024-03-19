**Baseado em C: Como Programar de Deitel**
O Conteúdo a seguir é uma reescrita dos capitulos do livro de deitel adaptados para a linguagem Dart

# Introdução à Programação 
Antes de começarmos, temos que entender que tanto no computador quanto na vida, utilizamos lógica e algoritimos em tudo! mas o que é um algorítmo?
 - É uma linguagem intermediária entre a linguagem humana e as linguagens de programação
 - É a especificação de uma sequência ordenada de instruções, finitas e não-ambíguas, que deve ser seguida para a solução de um determinado problema, garantindo a sua repetibilidade

Complicado né? Um algoritmo é um conjunto de instruções lógicas. É como uma receita de bolo: você segue as etapas na ordem correta e obtém o resultado desejado. Nos computadores, os algoritmos são usados para realizar várias tarefas, desde somar números até navegar na internet. Eles são a base de tudo o que os computadores fazem!


### Primeiro Programa em Dart

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
 - Começa com // indicando que é um comentário. Os programadores inserem comentários para documentar os programas e melhorar sua legibilidade. Os comentários não fazem com que o computador realize qualquer ação quando o programa é executado. Os comentários são ignorados pelo Dart e não fazem com que seja gerado nenhuma saída (quando o programa é executado, aquela linha de comentário não executa nenhuma ação). O comentário Primeiro programa em Dart descreve simplesmente o objetivo do programa. Os comentários também servem de auxílio para outras pessoas lerem e entenderem seu programa, mas muitos comentários podem tornar um programa difícil de ler.

A linha _**void main( )**_
 - É uma parte de todos os programas em Dart. Os parênteses após a palavra main indicam que main é um bloco de construção do programa chamado função. Os programas em Dart contêm uma ou mais funções, e uma delas deve ser main. Todos os programas em Dart começam a ser executados pela função main.

A chave esquerda, {, deve começar o corpo (ou o texto propriamente dito) de todas as funções. Uma chave direita equivalente deve terminar cada função. Este par de chaves e a parte do programa entre elas também é chamado um bloco. O bloco é uma unidade importante dos programas em Dart.

A linha _**print("Bem-vindo ao C!\n");**_
 - manda o computador realizar uma ação, especificamente imprimir na tela a string de caracteres limitada pelas aspas. Algumas vezes, uma string é chamada uma string de caracteres, uma mensagem ou um valor literal. A linha inteira, incluindo print, seus argumentos dentro dos parênteses e o ponto-e-vírgula (;), é chamada uma instrução Todas as instruções devem terminar com um ponto-e-vírgula (também conhecido como marca de fim de instrução). Quando a instrução print anterior é executada, a mensagem Bem-vindo ao Dart! é impressa na tela. Normalmente os caracteres são impressos exatamente como aparecem entre as aspas duplas ou simples na instrução print.

Dissemos que print faz com que o computador realize uma ação. Durante a execução de qualquer programa, são realizadas várias ações e o programa toma decisões. No final deste capítulo, analisaremos a tomada de decisões. No próximo capítulo, explicaremos mais este modelo ação/decisão de programação.

A chave direita, }, indica que o fim de main foi alcançado.

A função print pode imprimir Bem-vindo ao Dart! de várias maneiras. Observe que os caracteres **\n** não são impressos na tela. A barra invertida (ou backslash, \) é chamada _caractere de escape_. Ele indica que print deve fazer algo diferente do normal. Ao encontrar a barra invertida, print verifica o próximo caractere e o combina com a barra invertida para formar uma seqüência de escape. A seqüência de escape **\n** significa nova linha e faz com que o cursor se posicione no início da nova linha na tela. Observe o resultado abaixo:

```dart
// Primeiro Programa em Dart!

void main() {
  print('Bem\nVindo\nAo\nDart!');
}
```

```
OUTPUT (SAÍDA): Bem
                Vindo
                Ao
                Dart!
```

Algumas outras seqüências de escape comuns junto com a descrição de para o que ele serve estão listadas abaixo.

<html>
<table>
  <tr>
    <th>Sequencia de escape</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>\n</td>
    <td>Nova linha. Posiciona o cursor no inicio da nova linha.</td>
  </tr>
    <tr>
    <td>\t</td>
    <td>Tabulação horizontal. Move o cursor para a próxima marca parada de tabulação.</td>
  </tr>
    <tr>
    <td>\r</td>
    <td>Carriage return (CR). Posiciona o cursor no inicio da linha atual; não avança para a próxima linha.</td>
  </tr>
    <tr>
    <td>\a</td>
    <td>Alerta. Faz soar a campainha (Bell), do sistema.</td>
  </tr>
    <tr>
    <td>\$</td>
    <td>Cifrão. Imprime um caractere cifrão em uma instrução <b>print</b>.</td>
  </tr>
    <tr>
    <td>\\</td>
    <td>Barra invertida (backslash). Imprime um caractere de barra invertida em uma instrução <b>print</b>.</td>
  </tr>
    <tr>
    <td>\”</td>
    <td>Aspas duplas. Imprime um caractere de aspas duplas em uma instrução <b>print</b>.</td>
  </tr>
    <tr>
    <td>\'</td>
    <td>Aspas simples. Imprime um caractere de aspas simples em uma instrução <b>print</b>.</td>
  </tr>
</table>
</html>

As três últimas sequências de escape podem parecer estranhas. Como a barra invertida tem um significado especial para print, e, print a reconhece como um caractere de escape em vez de um caractere a ser impresso, usamos duas barras invertidas (\\) para indicar que uma única barra invertida deve ser impressa. Imprimir aspas duplas ou simples também constitui um problema para print porque esta instrução supõe normalmente que as aspas duplas indicam o limite de uma string e que as aspas duplas em si não devem ser realmente impressas. Usando a seqüência de escape \" ou \' dizemos a print para imprimir aspas duplas ou simples.

### Outro Programa Simples em Dart: Somar Dois Números Inteiros

O Programa a seguir usa a função (usa o comando) **stdin.readlinesync()** da biblioteca de entrada e saída para obter dois números inteiros digitados pelo usuário, calcular a soma desses valores e imprimir o resultado usando **print**. O programa e sua saída são mostrados abaixo. O comentário _**// Programa de soma**_ indica o objetivo do programa. Observe o código abaixo

```dart
import 'dart:io';

void main(List<String> arguments) {
  int inteiro1, inteiro2, soma;

  print('Digite o primeiro número: '); // Imprime o o texto
  inteiro1 = int.parse(stdin.readLineSync() ?? ''); // Lê o inteiro

  print('Digite o segundo número: '); // Imprime o o texto
  inteiro2 = int.parse(stdin.readLineSync() ?? ''); // Lê o inteiro

  soma = inteiro1 + inteiro2; // Faz a soma
  print('\nO resultado de $inteiro1 + $inteiro2 é $soma'); // Imprime o resultado
}
```
```md
  **Exemplo de Resultado:**

  Digite o primeiro número: 
  21
  Digite o segundo número:
  29

  O resultado de 21 + 29 é 50
```

Vamos agora destrinchar o código por completo de linha em linha:

A linha **import 'dart:io';** 
- É um comando dado ao programa, uma diretiva, que diz a o programa que os comandos dentro do arquivo **io.dart** poderão ser usados pelo programa. Esta linha em particular diz ao compilador para incluir o conteúdo do arquivo **io.dart** dentro do programa final.

Como mencionamos anteriormente, a execução de todos os programas começa com **void main()**. A chave esquerda { marca o início do corpo de **void main()** e a chave direita correspondente marca o fim de **void main()**.

