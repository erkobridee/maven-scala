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

Teste do Projeto
----------------

Utilize o comando: `mvn clean install`

Alterações
----------

* [v1](https://github.com/erkobridee/maven-scala/tree/v1) 
  * versão inicial funcional
  * Scala 2.8.0

* v2 - ***versão atual***
  * Scala 2.9.1, configuração do `pom.xml` conforme a dica do [gist](https://gist.github.com/1196756) 
  * **Observação:** realizei o teste com a versão do Scala 2.9.2, porém não funcionou as dependências, com isso mantive a versão 2.9.1


