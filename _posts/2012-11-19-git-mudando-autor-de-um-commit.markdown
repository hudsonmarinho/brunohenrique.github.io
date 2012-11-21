---
layout: post
title: Git - Mudando autor de um commit
date: 2012-11-19
categories: git dica pt
---
Ás vezes, por acidente, podemos fazer um commit em nome de outra pessoa, o user.name e user.email podem estar com configurações inesperadas ou você pode estar no computador de outra pessoa e etc, se por algum motivo algum commit estiver com o autor errado, você pode mudar isso.
<!-- more start -->
{% highlight bash linenos %}
➜  git log
commit d3cf3ac3471b78cdcab7080edf57d34f7b0e9679
Author: Bruno Henrique - Garu <squall.bruno@gmail.com>
Date:   Tue Nov 20 13:17:29 2012 -0300

    second commit

commit d55ce29cf22680a077c91bac7ee89efc01f68aa3
Author: Bruno Henrique - Garu <squall.bruno@gmail.com>
Date:   Tue Nov 20 13:12:27 2012 -0300

    first commit
{% endhighlight %}


{% highlight bash linenos %}
➜  git commit --amend --author="Other <other@example.com>"
[master 5ffb088] second commit
 Author: Other <other@example.com>
 0 files changed
 create mode 100644 LICENSE
{% endhighlight %}

{% highlight bash linenos %}
➜  git log
commit 5ffb088dd30c0a1f92460f6538d2c1d73c151b95
Author: Other <other@example.com>
Date:   Tue Nov 20 13:17:29 2012 -0300

    second commit

commit d55ce29cf22680a077c91bac7ee89efc01f68aa3
Author: Bruno Henrique - Garu <squall.bruno@gmail.com>
Date:   Tue Nov 20 13:12:27 2012 -0300

    first commit

{% endhighlight %}
<!-- end more -->
