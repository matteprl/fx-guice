fx-guice
========

[![Build Status](https://travis-ci.org/cathive/fx-guice.png)](https://travis-ci.org/cathive/fx-guice)

This library provides some useful classes that help you integrate
Google Guice into your JavaFX based applications.

The idea for that class was born after I read an article on
fxexperience.com (http://fxexperience.com/2011/10/fxml-guice/).
Therefore,... credits go to 'Richard Bair' for the initial idea.

A compiled and ready-to-use version of this library can be found in the
Sonatype OSS Maven Repository (oss.sonatype.org). To use the library
in your Maven based projects just add the following lines to your
'pom.xml':

```xml
<dependency>
  <groupId>com.cathive.fx</groupId>
  <artifactId>fx-guice</artifactId>
  <version>${fx-guice.version}</version>
</dependency>
```

In your project all you need to do is create an application class 
that extends `com.cathive.fx.guice.GuiceApplication` instead of the
`javafx.application.Application` class that ships with JavaFX.

Next step: instead of using `javafx.fxml.FXMLLoader` to load FXML files
you use `com.cathive.fx.guice.GuiceFXMLLoader`... that's basically it!
