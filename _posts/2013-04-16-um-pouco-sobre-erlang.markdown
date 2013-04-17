---
layout: post
title: Um pouco sobre Erlang
date: 2013-04-16
description: Fazia algum tempo que eu estava querendo começar a estudar alguma linguagem funcional, já tinha visto alguma coisa, lido alguns artigos mas nada aprofundado. Agora resolvi começar os estudos e a linguagem escolhida foi Erlang, muitos podem não conhecer mas é uma linguagem bem interessante.
categories: erlang pt
---
Fazia algum tempo que eu estava querendo começar a estudar alguma linguagem funcional, já tinha visto alguma coisa, lido alguns artigos mas nada aprofundado. Agora resolvi começar os estudos e a linguagem escolhida foi Erlang, muitos podem não conhecer mas é uma linguagem bem interessante.
<!-- more start -->

Diz a lenda que o nome Erlang vem de “Ericsson language” mas o nome foi uma homenagem ao matemático Agner Krarup **Erlang**, ela surgiu na década de 80 por causa de uma necessidade que nenhuma outra linguagem da época conseguia suprir, essa necessidade era para sistemas de telecomunicação (onde geralmente o sistemas são críticos, não podem parar de forma alguma) como foi o caso do AXD301 ATM Switch que em seu core tinha 1,5 milhões de linhas de código escritas em Erlang e mais meio milhão em C/C++ (para protocolos de baixo nível e drivers).

Atualmente algumas grandes empresas adotaram a linguagem Erlang, como:

**Facebook**, para seu sistema de chat com 100 milhões de usuários ativos.

**Delicious**, que tem mais de 5 milhões de usuarios e mais 150 milhões de bookmarks.

**Amazon**, em seu serviço de dados o SimpleDB.

**Github**, no sistema de backend lidando com milhares de transações concorrentes.

**37Signals**, em seu serviço poller do Campfire que lida com 240 milhões de HTTP responses, em média de 1200-1500 requests por segundo em períodos de pico. Esse serviço substituiu um que era escrito em C, que precisava de 240 processos e agora usa 3.

Motorola, CouchDB, RabbitMQ, Ejabbed, entre outros.

Para quem só está acostumado com programação orientada a objeto(como eu) a linguagem Erlang pode parecer estranha mas ele é bem expresiva (ainda mais quando falamos matemáticamente), exemplo: 

{% highlight erlang linenos %}

-module(fac).
-export([fac/1]).
 
fac(0) -> 1
fac(N) when > 0, is_integer(N) -> N * fac(N -1)
 
{% endhighlight %}

Agora para começar a brincadeira de verdade precisamos fazer a instalação, vamos lá:

{% highlight bash linenos %}
# Linux
 
$ sudo apt-get install erlang erlang-doc
 
# Mac OSX
 
$ brew install erlang
 
# Ou via source no site http://www.erlang.org/download.html
 
$ tar -xzf otp_src_XXXX-X.tar.gz # onde XXXX-X é a versão do Erlang
$ cd otp_src_XXXX-X
$ ./configure
$ make
$ sudo make install
 
# Também podemos usar uma solução da Erlang Soluctions https://www.erlang-solutions.com/downloads/download-erlang-otp
# e por fim temos CEAN(The Comprehensive Erlang Archive Network)
# http://cean.process-one.net/downloads/
{% endhighlight %}

Nem sempre a versão que está nos pacotes do apt-get ou brew são as mais recentes, então se você vai colocar o código em produção é legal que você faça a instalação direto do source.

Pretendo fazer mais alguns posts no futuro para consolidar meu conhecimento e documentar meu aprendizado, por enquanto é só isso :)

<!-- end more -->
