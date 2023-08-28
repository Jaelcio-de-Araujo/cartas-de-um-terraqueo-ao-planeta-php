# Cartas de um terráqueo ao planeta Php, Capitulo 6: Funções

Olá pessoal, tudo bem!? Espero que sim!
Hoje vamos aprender sobre funções em PHP, é algo muito importante, mas não é complicado até certo nível.
As funções são blocos de código que podem ser reutilizados em várias partes do nosso programa, também ajudam a 
tornar nosso código modular e organizado; as funções nos ajudam a evitar ter que digitar o mesmo código para executar uma tarefa várias vezes.

Veja a seguir a sintaxe de uma função:

~~~php
<?php
function nomeDaFuncao(parametro1, parametro2) {
    // Bloco de código da função
    return resultado;
}
~~~

Dentro das funções existe a possibilidade de passarmos parâmetros para o nosso programa por referencia ou valor.
Quando você passa um valor por valor para uma função, uma cópia do valor é criada e trabalhada dentro da função. 
Qualquer alteração feita dentro da função não afetará o valor original fora dela.

Passagem por Valor:

~~~php
<?php
function dobrarValor($numero) {
    $numero *= 2;
    return $numero;
}

$valorOriginal = 5;
$valorDobrado = dobrarValor($valorOriginal);

echo "Valor original: $valorOriginal \n";
echo "Valor dobrado: $valorDobrado";
~~~

Neste exemplo, a função dobrarValor recebe um número como parâmetro, dobra-o dentro da função e retorna o novo valor. 
No entanto, o valor original da variável $valorOriginal permanece inalterado.

Passagem por Referência:

~~~php
<?php

function triplicarValor(&$numero) {
    $numero *= 3;
}

$valorReferencia = 7;
triplicarValor($valorReferencia);

echo "Valor após triplicar: $valorReferencia";
~~~

Neste exemplo, a função triplicarValor recebe uma referência para uma variável (&$numero) e multiplica o valor por 3 dentro da função. 
Isso altera diretamente o valor da variável $valorReferencia fora da função.
Em resumo, a diferença entre passagem por valor e passagem por referência está na forma como os valores são tratados dentro da função e como eles afetam os valores originais fora da função.
Continue estudando, teste os códigos e os melhorem.

Se não tiver como fazer isso em seu computador, aqui está um site para você usar como plataforma: [Online PHP Compiler (programiz.com)](https://www.programiz.com/php/online-compiler/)

Até a próxima.
