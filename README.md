Maven Scala
===========

Exemplo de como criar um projeto em Scala utilizando o Maven.


Archetype do Maven que gerou a estrutura inicial do projeto
-----------------------------------------------------------

<pre><code>mvn archetype:generate \
    -DarchetypeGroupId=org.scala-tools.archetypes \
    -DarchetypeArtifactId=scala-archetype-simple \
    -Dversion=1.0 \
    -DgroupId=com.erkobridee.maven.scala \
    -DartifactId=maven-scala</code></pre>


Utilizado neste projeto
-----------------------

* Ambiente de desenvolvimento
  * [Maven](http://maven.apache.org/) 3
  * [Java](http://www.java.com/) 1.6+
  * [Scala](http://www.scala-lang.org/) 2.9.1
  * [Eclipse](http://eclipse.org/) Juno JEE
  * [Scala IDE](http://scala-ide.org/) 2.0.2 plugin para o Eclipse, como o Eclipse é o Juno, a versão do plugin é a disponível nesse link: [Scala IDE Helium, Nightly, for Eclipse 4.2 (Juno)](http://scala-ide.org/download/nightly.html)

Montando o ambiente local para uso desse projeto
---------------
O projeto disponibilizado no github, não possui nenhum arquivo para incluí-lo diretamente no Eclipse. Então após baixar o projeto no seu computador local.

Conforme especificado anteriormente, os itens citados do ambiente de desenvolvimento serão necessários.

Feito o download/clone do projeto para a sua máquina local, realize o respectivos passos a seguir:

1. Vá até o diretório do projeto
2. Execute os comandos em sequência:
  
  	`mvn compile` 
  	
  	`mvn eclipse:eclipse`
  
3. Importe o projeto no Eclipse

  	**Atenção:**

    	É necessário ter a variável M2_REPO configurada nas 
    	variáveis do ClassPath, apontando para o diretório 
    	do .m2/repository do Maven
    
4. Feito isso, o projeto está pronto para ser executado no Eclipse. Caso queira gerar o *.jar* do projeto utilize o comando

	`mvn clean install`    

Material de apoio para desenvolvimento com Scala
--------------

* [Learning Scala](http://www.scala-lang.org/node/1305)
* [Learning Scala in small bites](http://matt.might.net/articles/learning-scala-in-small-bites/)
* [Scala School](http://twitter.github.com/scala_school/)
* [Effective Scala](http://twitter.github.com/effectivescala/)


Alterações
----------

* [v1](https://github.com/erkobridee/maven-scala/tree/v1) 
  * versão inicial funcional
  * Scala 2.8.0

* [v2](https://github.com/erkobridee/maven-scala/tree/v2)
  * Scala 2.9.1, configuração do `pom.xml` conforme a dica do [gist](https://gist.github.com/1196756) 
  * **Observações:** 
  	* realizei o teste com a versão do Scala 2.9.2, porém não funcionou as dependências, com isso mantive a versão 2.9.1
  	* Como o Maven está gerenciando a compilação, não é necessário ter o Scala visivel no *PATH* da máquina de desenvolvimento
  	
* v3 - ***versão atual***
  * Incluido o suporte para importar o projeto no Eclipse e utilizar o Scala IDE 2.0.2 plugin (**Observação:** essa versão do plugin exige que o Scala seja a versão 2.9+) 
  * Necessário aumentar a quantidade de memória RAM utilizada pelo Eclipse, conforme descrito nesse [link](http://wiki.eclipse.org/FAQ_How_do_I_increase_the_heap_size_available_to_Eclipse%3F)
  




