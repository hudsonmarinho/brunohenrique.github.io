---
layout: post
title: Tools [#1] - MailCatcher, um simples servidor smtp para desenvolvimento
date: 2013-07-22
description:
categories: tools tip pt
---

<!-- more start -->
Geralmente quando estamos desenvolvendo aplicações que necessitam do envio de email precisamos configurar um servidor smtp localmente ou só testar no ambiente de produção (por favor, não façam isso).

Essa situação é bem comum em PHP e ainda mais quando não usamos framework algum. Com o Ruby on Rails a coisa muda um pouco de figura já que o Rails ultiliza 3 ambientes diferentes (test, development e production) podemos fazer configurações especificas para cada um.

No ambiente de teste (test) o Rails nos fornece ***ActionMailer::Base.deliveries***, que é um array para onde os email são enviados nesse contexto. Em produção (production), configuramos realmente nosso método de envio smtp, sendmail e file. E em desenvolvimento (development), ele faz o log de todo o envio no output do servidor para que possamos vizualizar esse envio.

Mesmo com todas essas facilidades ainda existem alguns momentos em que é necessário visualizar o email e é nesse momento em que entra o ***Mailcatcher***. Ele é um simples servidor smtp para podermos usar em desenvolvimento e além, de ser um servidor, possui um interface web onde captura o email e mostra em uma "inbox" própria.

### Usando:

Para instalar é bem simples:

{% highlight bash %}
  $ gem install mailcatcher
{% endhighlight %}

Depois de instalado, faz-se a configuração no seu ```config/environments/development.rb```

{% highlight ruby %}
  config.action_mailer.delivery_method = :smtp
  config.action_mailer.smtp_settings = { :address => "localhost", :port => 1025 }
{% endhighlight %}


Para configurar no PHP é só adicionar a seguinte configuração de email no seu php.ini:

{% highlight php %}
  sendmail_path = /usr/bin/env catchmail -f some@from.address
{% endhighlight %}

ou no htaccess:

{% highlight php %}
  php_value sendmail_path "/usr/bin/env catchmail -f some@from.address"
{% endhighlight %}

Agora é só "levantar" o servidor usando mailcatcher via linha de comando:

{% highlight bash %}
  $ mailcatcher
  Starting MailCatcher
  ==> smtp://127.0.0.1:1025
  ==> http://127.0.0.1:1080
  *** MailCatcher runs as a daemon by default. Go to the web interface to quit.
{% endhighlight %}

Agora se você acessar no browser http://127.0.0.1:1080 haverá uma tela parecida com está:
![mailcatcher web interface](http://screencloud.net/img/screenshots/f77cd7c626b0158de0e650681f9d1c93.png)

### Bônus
Para configurar no Django também é bem simples, basta adicionar no settings.py o seguinte código:

{% highlight python %}
  if DEBUG:
    EMAIL_HOST = '127.0.0.1'
    EMAIL_HOST_USER = ''
    EMAIL_HOST_PASSWORD = ''
    EMAIL_PORT = 1025
    EMAIL_USE_TLS = False
{% endhighlight %}

<!-- end more -->
