# Cartas de um terráqueo ao planeta Php, Capitulo 2

Olá pessoal, tudo bem!? Espero que sim!
Em nossa segunda carta, vamos falar sobre como se inicia em Php, e de fato do precisamos para "manter contato com ele".
O Php é uma linguagem de programação muito leve e rápida; para você começar a trabalhar com ela não precisa de quase nada, 
nem mesmo um computador muito potente, também não precisa baixar milhares de outros programas e nem pacotes para começar a 
criar seus projetos; vamos ver do que precisamos à seguir:

1 - Baixe a ultima versão do Php para Windows aqui: [PHP 8.2](https://windows.php.net/downloads/releases/php-8.2.8-nts-Win32-vs16-x64.zip)

2 - Para Linux você pode baixar aqui: [PHP 8.2](https://www.php.net/distributions/php-8.2.8.tar.gz)

Dai não precisa de mais nada, ao contrário do que muitos pensam o Php não precisa de mais nada para rodar seus scripts. 
Descompacte os arquivos em local de sua preferencia. Para ficar mais fácil vamos, no caso do Windows adicionar o php às 
variáveis de ambiente, e para isso eu ja criei um artigo que você pode acessar aqui: [Artigo](https://pt.linkedin.com/pulse/php-sem-o-apache-jaelcio-araujo?trk=portfolio_article-card_title). 
Isso vai permitir que o Php seja reconhecido em todo o nosso sistema e dessa maneira possamos 
chamar o comando php em qualquer lugar do nosso sistema. Assim:

![php](assets/php02.png)

E pronto, você já estará pronto para trabalhar com php. Crie uma pasta em qualquer lugar do seu sistema, abra o terminal dentro 
dessa pasta e digite o comando a seguir para iniciar o servidor do php:

~~~php
php -S localhost:8000
~~~

Com isso o php irá inicia o servidor na porta 8000 e mostrara uma mensagem como essa:

~~~php
PHP 8.1.10 Development Server (http://localhost:8000) started
~~~

O terminal deve ficar aberto enquanto trabalha com o Php, para que ele possa interpretar os scripts, quando terminar basta 
teclar CRTL + C para para o servidor e depois fechar o terminal.
Para treinarmos, depois de iniciar o seu servidor, vamos dentro da sua pastar criar um arquivo chamado index.php; dentro dele coloque este código:

~~~php
<?php
phpinfo();
~~~

Salve o arquivo com o nome de index.php, vá no seu navegador de internet e acesso o endereço http://localhost:8000/
Em meu caso eu defini a porta 8000, mas você pode definir outro se for o caso.
A resposta do seu navegador será como esta à seguir:

![php](assets/php03.png)

Isso significa que o php interpretou o seu código corretamente, e para as demais páginas que vamos fazer basta acessar o endereço seguido do nome da pagina.
E é isso pessoal! Escreva outros scripts, busque na internet e divirta-se com Php. Somente com Php você já pode ter um ambiente leve e rápido para trabalhar.
Até a próxima.
