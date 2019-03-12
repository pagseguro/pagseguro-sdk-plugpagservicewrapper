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
implementation 'br.com.uol.pagseguro.plugpagservice.wrapper:wrapper:1.0'
```
