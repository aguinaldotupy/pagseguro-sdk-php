Biblioteca de integração PagSeguro para PHP
===========================================

[![Code Climate](https://codeclimate.com/github/pagseguro/pagseguro-php-sdk/badges/gpa.svg)](https://codeclimate.com/github/pagseguro/pagseguro-php-sdk)
[![Total Downloads](https://poser.pugx.org/pagseguro/pagseguro-php-sdk/d/total.svg)](https://packagist.org/packages/pagseguro/pagseguro-php-sdk)
[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%207.1.3-blue.svg?style=flat-square)](https://php.net/)
[![Latest Stable Version](https://poser.pugx.org/pagseguro/pagseguro-php-sdk/v/stable.svg)](https://packagist.org/packages/pagseguro/pagseguro-php-sdk)
[![Latest Unstable Version](https://poser.pugx.org/pagseguro/pagseguro-php-sdk/v/unstable.svg)](https://packagist.org/packages/pagseguro/pagseguro-php-sdk)

> Caso você deseje usar uma versão abaixo do PHP 7.1.3 por favor consulte o branch https://github.com/pagseguro/pagseguro-php-sdk/tree/5.x.x

Descrição
---------

A biblioteca PagSeguro em PHP é um conjunto de classes de domínio que facilitam, para o desenvolvedor PHP, a utilização das funcionalidades que o PagSeguro oferece na forma de APIs. Com a biblioteca instalada e configurada, você pode facilmente integrar funcionalidades como:

 - [Criar Requisições de Pagamentos]
 - [Criar Requisições de Pagamento Recorrente] (assinatura transparente)
 - [Criar Requisições de assinaturas]
 - [Cancelar Assinaturas]
 - [Consultar Assinaturas]
 - [Consultar Transações por Código]
 - [Consultar Transações por Intervalo de Datas]
 - [Receber Notificações]


Requisitos
----------

 - [PHP] ^7.1.3|^8.0
 - [SPL]
 - [cURL]
 - [SimpleXml]
 - [Composer]


Instalação
----------
> Nota: Recomendamos a instalação via **Composer**. Você também pode baixar o repositório como [arquivo zip] ou fazer um clone via Git.
 
 ### Instalação via Composer
> Para baixar e instalar o Composer no seu ambiente acesse https://getcomposer.org/download/ e caso tenha dúvidas de como utilizá-lo consulte a [documentação oficial do Composer].

É possível instalar a biblioteca pagseguro-php-sdk([pagseguro/pagseguro-php-sdk]) via Composer de duas maneiras:

- Executando o comando para adicionar a dependência automaticamente
  ```
  php composer.phar require pagseguro/pagseguro-php-sdk
  ```

**OU**

- Adicionando a dependência ao seu arquivo ```composer.json```
  ```composer.json
  {
      "require": {
         "pagseguro/pagseguro-php-sdk" : "^6.0"
      }
  }
  ```
 
### Instalação manual
 - Baixe o repositório como [arquivo zip] ou faça um clone;
 - Descompacte os arquivos em seu computador;
 - Execute o comando ```php composer.phar install``` no local onde extraiu os arquivos.
 
 
 Como usar
 ---------
 O diretório *[public](public)* contém exemplos das mais diversas chamadas à API do PagSeguro utilizando a biblioteca (pagamento, assinatura, notificação) e o diretório *[source](source)* contém a biblioteca propriamente dita (código fonte).


Configuração
------------

Para fazer uso real da biblioteca, é preciso fazer algumas configurações. 
Para saber mais sobre como configurar a biblioteca acesse a [documentação](/public/Configuration/README.md).


Dúvidas?
----------
---
Caso tenha dúvidas ou precise de suporte, abra um chamado conosco [link].


Changelog
---------
Para consultar o log de alterações acesse o arquivo [CHANGELOG.md](CHANGELOG.md).


Licença
-------

Copyright 2016 PagSeguro Internet LTDA.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.


Notas
-----

 - O PagSeguro somente aceita pagamento utilizando a moeda Real brasileiro (BRL).
 - Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial.
 - Certifique-se que tenha definido corretamente o charset de acordo com a codificação (ISO-8859-1 ou UTF-8) do seu sistema. Isso irá prevenir que as transações gerem possíveis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
 - Para que ocorra normalmente a geração de logs, certifique-se que o diretório e o arquivo de log tenham permissões de leitura e escrita.

Dúvidas?
----------

Em caso de dúvidas acesse nosso [fórum].


Contribuições
-------------

Achou e corrigiu um bug ou tem alguma feature em mente e deseja contribuir?

* Faça um fork
* Adicione sua feature ou correção de bug (git checkout -b my-new-feature)
* Commit suas mudanças (git commit -am 'Added some feature')
* Rode um push para o branch (git push origin my-new-feature)
* Envie um Pull Request
* Obs.: Adicione exemplos para sua nova feature. Se seu Pull Request for relacionado a uma versão específica, o Pull Request não deve ser enviado para o branch master e sim para o branch correspondente a versão.

  [Criar Requisições de Pagamentos]: https://devs.pagseguro.uol.com.br/docs/checkout-web
  [Criar Requisições de Pagamento Recorrente]: https://devs.pagseguro.uol.com.br/docs/pagamento-recorrente
  [Criar Requisições de assinaturas]: https://devs.pagseguro.uol.com.br/docs/arquivo-documentacoes-depreciadas
  [Cancelar Assinaturas]: https://devs.pagseguro.uol.com.br/docs/arquivo-documentacoes-depreciadas
  [Consultar Assinaturas]: https://devs.pagseguro.uol.com.br/docs/arquivo-documentacoes-depreciadas
  [Cancelar Transações por Código]: https://devs.pagseguro.uol.com.br/docs/pagamento-recorrente-cancelamento-de-adesao
  [Consultar Transações por Código]: https://devs.pagseguro.uol.com.br/docs/pagamento-recorrente-consulta-pelo-codigo-de-adesao
  [Consultar Transações por Intervalo de Datas]: https://devs.pagseguro.uol.com.br/docs/pagamento-recorrente-consulta-por-intervalo-de-datas
  [Receber Notificações]: https://devs.pagseguro.uol.com.br/docs/checkout-web-notificacoes
  [link]: https://app.pipefy.com/public/form/k8aKYyJE/?_ga=2.175732066.1759255508.1544013668-532205691.1540442951
  [PHP]: http://www.php.net/
  [SPL]: http://php.net/manual/en/book.spl.php
  [cURL]: http://php.net/manual/en/book.curl.php
  [SimpleXml]: http://php.net/manual/en/book.simplexml.php
  [Composer]: https://getcomposer.org
  [pagseguro/pagseguro-php-sdk]: https://packagist.org/packages/pagseguro/pagseguro-php-sdk
  [Como receber pagamentos pelo PagSeguro]: https://pagseguro.uol.com.br/receba-pagamentos.jhtml#checkout-transparent
  [arquivo zip]: https://github.com/pagseguro/pagseguro-php-sdk/archive/master.zip
  [documentação oficial do Composer]: https://getcomposer.org/doc/
