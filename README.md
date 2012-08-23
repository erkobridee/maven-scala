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
  * [Scala](http://www.scala-lang.org/) 2.8.0

Teste do Projeto
----------------

Utilize o comando: `mvn clean install`

Alterações
----------

* [v1](https://github.com/erkobridee/maven-scala/tree/v1) 
  * versão inicial funcional
* v2 - ***versão atual***
