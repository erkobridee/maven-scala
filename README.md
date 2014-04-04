# Maven Scala

Exemplo de como criar um projeto em Scala utilizando o Maven.


## Archetype do Maven que gerou a estrutura inicial do projeto

```bash
mvn archetype:generate \
  -DarchetypeGroupId=org.scala-tools.archetypes \
  -DarchetypeArtifactId=scala-archetype-simple \
  -Dversion=1.0 \
  -DgroupId=com.erkobridee.maven.scala \
  -DartifactId=maven-scala
```


## Utilizado neste projeto

* Ambiente de desenvolvimento

  * [Maven](http://maven.apache.org/) 3

  * [Java](http://www.java.com/) 1.6+

  * [Scala](http://www.scala-lang.org/) 2.9.1

  * [Eclipse](http://eclipse.org/) Juno JEE

  * [Scala IDE](http://scala-ide.org/) 2.0.2 plugin para o Eclipse, como o Eclipse é o Juno, a versão do plugin é a disponível nesse link: [Scala IDE Helium, Nightly, for Eclipse 4.2 (Juno)](http://scala-ide.org/download/nightly.html)


## Montando o ambiente local para uso desse projeto

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


## Material de apoio para desenvolvimento com Scala

* [Learning Scala](http://www.scala-lang.org/node/1305)

* [Learning Scala in small bites](http://matt.might.net/articles/learning-scala-in-small-bites/)

* [Scala School](http://twitter.github.com/scala_school/)

* [Effective Scala](http://twitter.github.com/effectivescala/)

* [Scala Documentation](http://docs.scala-lang.org/index.html)


### Caso de Uso

* [Transitioning to Scala | Medium](https://medium.com/p/d1818f25b2b7) - Advice from a developer who helped rebuild Walmart.ca with Scala and Play


## Alterações

* Descrições de cada versão em [releases](https://github.com/erkobridee/maven-scala/releases)
