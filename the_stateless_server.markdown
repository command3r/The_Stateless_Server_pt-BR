







THE STATELESS SERVER
====================

1. Programação Funcional
2. Node.js
3. The Stateless Server















PROGRAMAÇÃO FUNCIONAL
=====================

Observação de software pelas *funções* que
desempenha em *estruturas de dados* *imutáveis
e sem estado*.












FUNÇÕES QUE DESEMPENHA
----------------------

# Orientação à Objetos:

*Atores* em *contexto* performando *ações* que
alteram o seu estado e seu contexto.

        ,---------------,            __
        |               '_____      ('') 
        |      ,,,      ,----/\    /(  )\
        |     ('-')     |   /__\    //\\
        |   o=(   )=o   |    ||
        |     // \\     |____||   __
        |               |-----'  ('') 
        '---------------'       /(  )\
                                 //\\









# Funcional:
   
*Processamento* de *entradas* e retorno de *saídas*.
      
                       /////----       
             |\,      //////-----         |:\  
         ----'  \    +++++++------    ===='::\ 
         ----, ,/     ++++++/////     ====,::/ 
             |/        +++++////          |:/    
         
      




# Exemplo:

Balanço de uma venda, levando
em consideração taxas do contrato
relacionado.

Balanço é a soma do custo da venda e
as taxas contratuais, menos o que já
está pago.

:e [account.rb](https://github.com/rafaelbandeira3/The_Stateless_Server_pt-BR/blob/master/account.rb) [account_stateless.rb](https://github.com/rafaelbandeira3/The_Stateless_Server_pt-BR/blob/master/account_stateless.rb)





ESTRUTURAS DE DADOS
-------------------

Tudo é tratado como dados, inclusive funções,
que podem ser usadas como entrada e saída de 
dados.

      
                    **********     /////----       %%%%%%%      
             |\,    ##########    //////-----    %%%%&&&%%%%       |:\  
         ----'  \   **********   +++++++------   %%%&&&&&%%%   ===='::\ 
         ----, ,/   ##########    ++++++/////    %%%%&&&%%%%   ====,::/ 
             |/     **********     +++++////       %%%%%%%         |:/    

      

*Funções de primeira classe*, é o termo usado
para funções são tratadas como objetos da 
mesma forma que strings e números.

*Funções de alta ordem*, é o termo usado para
para funções que retornam outras funções.

Algoritmos como dados? Lindo.

      









# Exemplo:

Preço de passagens de avião para
diferentes tipos de clientes.

:e [ticket_price.js](https://github.com/rafaelbandeira3/The_Stateless_Server_pt-BR/blob/master/ticket_price.js)
















IMUTÁVEL
--------

Funções que apenas computam suas entradas sem
causar *efeitos colaterais*, ou seja alterar seu 
contexto, são chamadas de *funções puras*.

Funções puras são idempotentes e garantem 
transparência referencial.








# Exemplo: 

Calcular capacidade disponível para demandas
de gás em tubulações que transportam gás por
vários estados.

:e [scheduling_gas.cs](https://github.com/rafaelbandeira3/The_Stateless_Server_pt-BR/blob/master/scheduling_gas.cs)

















SEM ESTADO
----------

Elimina o conceito de *comportamento*.

Permite *avaliação tardia* e *otimizações*
pelo compilador.





# Exemplo:

API de json com suporte a diferentes ambientes.

:e [restful_server.coffee](https://github.com/rafaelbandeira3/The_Stateless_Server_pt-BR/blob/master/restful_server.coffee)
















NODE.JS
=======

* Ambiente virtual de Javascript criado 
  em cima da V8 (usada no Chrome)
* Infra-estrutura assíncrona com suporte
  à file system, IO... e HTTP
* REPL
* NPM - gerenciador de extensões, feito
  do jeito certo
* PasS com Heroku, Nodester... outros?
* Javascript










# Exemplo:

[Criando um servidor node.js do zero](https://github.com/rafaelbandeira3/The_Stateless_Server-nodejs-example/commits/master)









THE STATELESS SERVER
====================

Como *não ter* estado quando...
* Persistência e IO são dependentes de estado
* Cookies são estado do cliente
* Sessões são o estado da aplicação para um usuário















Como *ter* estado quando...
* HTTP é inerentemente sem estado
* Design funcional
* REST
 















REFERÊNCIAS E LEITURAS
======================

* Introdução à programação funcional com Java http://www.defmacro.org/ramblings/fp.html
* Vantagens de design sem estado http://stackoverflow.com/questions/844536/advantages-of-stateless-programming
* Objetos imutáveis http://www.javapractices.com/topic/TopicAction.do?Id=29
* Por que precisamos de objetos imutáveis http://stackoverflow.com/questions/3769607/why-do-we-need-immutable-class
* Programando com dados imutáveis http://msdn.microsoft.com/en-us/library/hh297115(v=vs.100).aspx
* Programação funcional com dados imutáveis http://www.slideshare.net/adorepump/functional-programming-with-immutable-data-structures
* Idempotência http://en.wikipedia.org/wiki/Idempotence
* Transparência referencial http://en.wikipedia.org/wiki/Referential_transparency_(computer_science)
* Connect para nodejs http://www.senchalabs.org/connect
* API do nodejs http://nodejs.org/api/all.html





















ENTREM EM CONTATO
=================

* Rafael Bandeira
* @rafb3
* rafaelbandeira3@gmail.com
* http://github.com/rafaelbandeira3
* http://anythingsoftware.posterous.com
























