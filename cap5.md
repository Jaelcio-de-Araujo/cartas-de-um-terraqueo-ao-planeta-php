# Cartas de um terráqueo ao planeta Php, Capitulo 5: Estrutura de Controle, e de Decisão.

Olá pessoal tudo bem, tudo bem!? Espero que sim!
Hoje iremos falar sobre estruturas de controle; estruturas de controle são uma forma de definir o 
fluxo do nosso programa, ou seja, definir como o programa irá se comportar 
dependendo de uma situação onde ele precise tomar uma decisão; por isso elas também são conhecidas como 
"Estruturas de decisão", porém estruturas de decisão ou controle são coisas distintas.

## Estrutura de controle
Nos permitem executar um bloco de código de forma controlada, ou seja, podemos controlar o fluxo do programa.

~~~php
if ($number % 2 == 0){
  echo "O número é par.";
} else {
  echo "O número é ímpar.";
}
~~~

Estrutura de controle While:
Essa estrutura faz a verificação no inicio da execução, ou seja, vai procurar o valor verdadeiro da 
condição e se logo no começo não encontrar o script para a execução.

~~~php
<?php
$i = 0;
while ($i < 10) {
  echo "$i \n";
  $i++;
}
~~~

Estrutura de controle Do...While:

~~~php
<?php
$i = 0;
do {
  echo $i;
  $i++;
} 
while ($i < 10);
~~~

O Do...While tem praticamente a mesma função do While, porém, ela faz a verificação da condição no final do bloco, dai ela executa o script pelo menos uma vez.
Estrutura de controle For:

~~~php
<?php
for ($i = 0; $i < 10; $i++) {
  echo $i;
}
~~~

Essa estrutura é usada para executar o bloco de código um número expecifico de vezes, todas as vezes que sabemos a quantidade 
de vezes que um bloco deve ser executado usamos o for. Estrutura de controle Foreach:

~~~php
<?php
$array = array(1, 2, 3, 4, 5);
foreach ($array as $value) {
  echo $value;
}
~~~

O foreach é usado para iterar um array. Array é um estrutura de dados que armazena uma quantidade de dados maior que zero; na prática é uma 
lista de elementos de mesmo tipo. Usamos o foreach quando queremos que nosso código percorra essa lista.

## Estrutura de decisão

Estrutura de decisão If:

~~~php
<?php
$number = 5;
if ($number % 2 == 0) {
  echo "O número é par.";
} else {
  echo "O número é ímpar.";
}
~~~

È usado para pode fazer script executar um bloco se uma condição for verdadeira.
Estrutura de decisão Switch:

~~~php
<?php
$diaDaSemana = "segunda-feira";
switch ($diaDaSemana) {
  case "segunda-feira":
    echo "Hoje é segunda-feira.";
    break;
  case "terça-feira":
    echo "Hoje é terça-feira.";
    break;
  case "quarta-feira":
    echo "Hoje é quarta-feira.";
    break;
  case "quinta-feira":
    echo "Hoje é quinta-feira.";
    break;
  case "sexta-feira":
    echo "Hoje é sexta-feira.";
    break;
  case "sábado":
    echo "Hoje é sábado.";
    break;
  case "domingo":
    echo "Hoje é domingo.";
    break;
}
~~~

O switch é usada para selecionar um bloco de código a ser executado com base em um valor. 
Ela é semelhante à estrutura if, mas permite que você selecione um bloco de código com base em um valor, em vez de uma condição.


Agora terminamos!
Copie os códigos e digite, pratique!
Até a próxima!






