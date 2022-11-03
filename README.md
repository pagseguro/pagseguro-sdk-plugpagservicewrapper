# **PlugPagServiceWrapper**


## **Introdução**

PlugPagServiceWrapper é uma biblioteca para integrar aplicativos Android com o terminal Moderninha Smart do PagSeguro e utilizar a solução de pagamentos, PlugPag, embarcado no POS.

O PlugPag é desenvolvido pelo PagSeguro com o objetivo de permitir que empresas e desenvolvedores independentes possam criar novas soluções com integração com um meio de pagamento presencial.

## **Importando PlugPagServiceWrapper**

Para utilizar o PlugPagService Wrapper adicione o seguinte código ao seu gradle do projeto:

```
allprojects {
	repositories {
		...
		maven {
        	   url 'https://github.com/pagseguro/PlugPagServiceWrapper/raw/master'
       		}

	}
}
```

Em seguida inclua a seguinte dependencia no gradle do modulo:
```
implementation 'br.com.uol.pagseguro.plugpagservice.wrapper:wrapper:1.22.0'
```

## **Documentação**

Mais informações sobre como utilizar o PlugPagServiceWrapper podem ser encontradas no arquivo **Documentacao.pdf**


## Pré-requisitos

Para utilizar o PlugPagServiceWrapper, é necessário incluir suporte ao Kotlin no app. Para isso, adicione os seguintes códigos:

No build.gradle do projeto:

```
buildscript {
	ext.kotlin_version = ‘1.3.21’
	...
	dependencies {
		...
		classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version"
		...
	}
}

```

No build.gradle do módulo:

```
...
apply plugin: 'kotlin-android'
apply plugin: 'kotlin-android-extensions'
...

dependencies {
	...
	implementation "org.jetbrains.kotlin:kotlin-stdlib:$kotlin_version"
	...
}
```


