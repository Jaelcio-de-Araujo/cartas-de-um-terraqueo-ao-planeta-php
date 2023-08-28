# Cartas de um terráqueo ao planeta Php, Capitulo 3: Variáveis.

Olá pessoal, tudo bem!? Espero que sim!
Em nossa terceira carta, vamos falar sobre como se tratamos variáveis em php.
Antes de mais nada é preciso entender o que é uma variável...A variável é uma forma de guardar valores dentro da execução de um programa, 
elas servem para guardar um valor, e este valor poderá ser usado no decorrer do nosso programa, podendo alterar a direção e as domadas de 
decisão do nosso código, em suma, as variáveis são um nome que usamos para guardar um valor, o qual poderemos usar durante a execução do nosso código.
No Php quando falamos de variáveis, também temos que falar em "tipos de dados", ou seja, os tipos de informações possíveis de serem guardando em um 
nome de variável. Abaixo você pode verificar os tipos comuns de dados.

TIPO      | DESCRIÇÃO                 | EXEMPLO
--------- | --------------------------|-------------
INTEGER   | NÚMERO INTEIRO            | 10, 20, -10
FLOAT     | NḾERO DO PONTO FLUTUANTE  | 10.5, -2.5 
STRIMG0   | SEQUENCIA DE CARACTERES   | "OLÁMUNDO", "123456789"
BOOLEAN   | VERDADEIRO OU FALSO       | TRUE, FALSE
ARRAY     | LISTA DE VALORES          | [1, 2, 3], ["A", "B", "C"]
OBJETO    | OBJETO                    | new stcClass(), new User()
NULL      | VALOR NÚLO                | NULL

Os tipos de dados definem o formato de informação que poderá ser guardado dentro de uma variável. Antigamente o não era preciso definir 
o tipo de dados em declaração de varáveis em Php, porém agora é uma prática muito bem avaliada pela comunidade, pois definir o tipo de dado 
que a variável vai receber, pode evitar muitos bugs, brechas e falhas.

No Php usamos o símbolo de "$" para iniciar uma variável, os nomes de variável não podem ter acentos nem caracteres especiais, tipo "ç"; 
também não podem ter espaços. Abaixo você vai ver como usamos as variáveis dentro do Php:

~~~php
<?php

// Intege
$integer = 10;
echo gettype($integer); // int

// Float
$float = 10.5;
echo gettype($float); // float

// String
$string = "Olá, mundo!";
echo gettype($string); // string

// Boolean
$boolean = true;
echo gettype($boolean); // boolean

// Array
$array = [1, 2, 3];
echo gettype($array); // array

// Object
$object = new stdClass();
echo gettype($object); // object

// Null
$null = null;
echo gettype($null); // NULL
~~~

Não preocupe-se com os códigos agora, mais adiante vamos entender isso bem melhor, até você apenas entender que cada variável guarda um valor, 
e que o tipo de valor que ela vai guardar pode ser definido na sua criação, coo a seguir:


~~~php
<?php
$integer = (int) 10;
echo gettype($integer); // int
~~~

Neste exemplo, estamos criando uma variável chamada integer e atribuindo a ela o valor 10. Estamos também usando o operador (int) para 
definir o tipo da variável como int. O operador (int) converte seu operando para um número inteiro.

## Exercício

Vamos cria um exemplo bem simples para você poder entender melhor tudo isso.
Dentro do seu ambiente que nós já criamos, crie um novo arquivo e dê o nome de execicio01.php, dentro dele digite o código a seguir:

~~~php
<?php

$_nome              = (string) "Jaelcio Araujo";
$_idade             = (int) 34;
$_peso              = (float) 80.5;
$_fumante_sn        = (bool) false;

echo "Nome: " .     $_nome . "\n";
echo "Idade: " .    $_idade . "\n";
echo "Peso: " .     $_peso . "\n";
echo "Fumante: " .  $_fumante_sn . "\n";
~~~

Neste exemplo você acessar o navegador, depois de ter ativador o servidor interno do Php e ver o resultado:

![php](php04.pnj)

Ou tambem pode ver direto no terminal:

![php](php05.pnj)

E terminamos por aqui a estão inicial de variáveis.
Espero sinceramente que isso te ajude, pois não serve ssomente para php, mas todas as linguagens.
Abraços e até a próxima!


















