---
layout: post
title: Koans – introdução
date: 2011-11-03
categories: koans pt  
---
Estou meio sem tempo, mas estou tentando postar toda semana, hoje quero falar sobre os  grandes koans, que muita gente não conhece e acho um bom caminho para quem esta começando ou quer se aprofundar em alguma linguagem. Então vamos ao que interessa…^^

###A Filosofia dos Koans

O koan é uma maneira utilizada desde a antiguidade pelos mestres orientais para transmitir seus ensinamentos aos seus discípulos, visando abrir os olhos do indivíduo à sua própria consciência. Um dos primeiros koans de que se tem conhecimento nos indaga “Qual a imagem do seu rosto antes de nascer?” “Você consegue vê-la?”. Essa indagação se propõe a exercitar a mente, a buscar a resposta. Ao aceitar o koan, passamos a questionar tudo o que até então aceitaríamos como impossibilidade lógica, como verdade absoluta, e passamos a compreender que a maneira pela qual enxergamos as coisas ao nosso redor nem sempre é correta ou única.  
O koan força o indivíduo a assumir uma atitude inquisitória até praticamente chegar à beira de um precipício mental. Propõe colocar a mente em um estado de total esforço até encontrar a resposta. Ao abandonar a racionalidade, transformam-nos na própria questão, tornando-nos capazes de ver a nítida imagem da “face original”.

###O que isso tem a ver com programação?

O conceito de aprendizado gradual não é novo. Na década de 1960 a 70, a inovação na área de programação de computadores foi marcada por dois [paradigmas](http://pt.wikipedia.org/wiki/Paradigma_de_programa%C3%A7%C3%A3o): [procedural](http://pt.wikipedia.org/wiki/Programa%C3%A7%C3%A3o_procedural) (inperative) do qual a linguagem [Fortran](http://en.wikipedia.org/wiki/Fortran) foi a mais utilizada e o funcional (declarative) onde o [LISP](http://pt.wikipedia.org/wiki/Lisp) foi a mais comum. Muitos livros foram escritos com a finalidade de explicar minuciosamente cada paradigma e linguagem, mas esses livros eram bastante complicados de se ler .No final dos anos 80 que um livro chamado [The Little LISPer](http://www.amazon.com/Little-LISPer-Third-Daniel-Friedman/dp/0023397632)  introduziu uma nova forma  de aprender [programação funcional](http://pt.wikipedia.org/wiki/Programa%C3%A7%C3%A3o_funcional), o livro seguia um formato de uma conversa onde uma pergunta era feita e, em seguida, a resposta era dada.

|                                                 |                                                                        |
|-------------------------------------------------|------------------------------------------------------------------------|
| Is it true that this is an atom? turkey         | Yes, because turkey is a string of characters beginning with a letter. |
| Is it true that this is a list?(atom turkey or) | Yes, because it is a collection of atoms enclosed by parenthesis.      |

Este formato era bem mais simples de ser seguido, isso então forneceu uma base para que pudéssemos pegar ideias complexas e dividir  em varias ideias menos complexas, dessa maneira vimos que também era um ótima forma de ensinar sintaxe e detalhes de varias linguagens. E se prestarmos atenção a ideia de propor uma verdade e em seguida verificar a sua veracidade, é a essência de um teste. Mais especificamente os famosos e clássicos testes unitários.
Pretendo fazer  mais alguns posts mostrando o koans na prática, comecei com esse porque não queria começar a falar de uma coisa sem antes falar um pouco de suas origens.Esse post contem alguns resumos de meus estudos e algumas traduções de artigos sobre o assunto.
Abordarei os koans em algumas linguagens (ruby, javascript e python), mas saiba que esse mesmo conceito se aplica as outras linguagens.

>We are what we think. All that we are arises with our thoughts. With our thoughts, we make our world. “Buda”

referências: [http://sett.ociweb.com/](http://sett.ociweb.com/), [http://www.clinicacomciencia.com/](http://www.clinicacomciencia.com/)