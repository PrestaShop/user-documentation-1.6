# Outras Informações

**Sumário**

* [Outras Informações](outras-informacoes.md#OutrasInformações-OutrasInformações)
  * [Tenha sempre uma versão de testes pronta!](outras-informacoes.md#OutrasInformações-Tenhasempreumaversãodetestespronta!)
  * [Verificando a biblioteca GD](outras-informacoes.md#OutrasInformações-VerificandoabibliotecaGD)
  * [Ativando PHP5](outras-informacoes.md#OutrasInformações-AtivandoPHP5)
    * [1&1](outras-informacoes.md#OutrasInformações-1&1)
    * [Free.fr](outras-informacoes.md#OutrasInformações-Free.fr)
    * [OVH](outras-informacoes.md#OutrasInformações-OVH)
    * [GoDaddy](outras-informacoes.md#OutrasInformações-GoDaddy)
    * [Lunarpages Hospedagem](outras-informacoes.md#OutrasInformações-LunarpagesHospedagem)

## Outras Informações <a href="#outrasinformacoes-outrasinformacoes" id="outrasinformacoes-outrasinformacoes"></a>

### Tenha sempre uma versão de testes pronta! <a href="#outrasinformacoes-tenhasempreumaversaodetestespronta" id="outrasinformacoes-tenhasempreumaversaodetestespronta"></a>

Depois de ter concluído a criação de sua loja e feito configuração da forma como você desejar, antes de você lançar oficialmente ao público para começarem as compras, nós recomendamos que você instale uma versão de teste local em seu computador pessoal (usando WAMP para Windows, MAMP para Mac ou LAMP para Linux, ou XAMPP para qualquer uma dessas plataformas), ou em outro lugar no seu servidor de hospedagem.

Esta segunda instância será útil como um ambiente de pré-produção em que você pode realizar todas as futuras alterações à sua loja PrestaShop antes de efetuar em seu site de produção. Dessa forma, se um erro ocorrer, sua loja permanece intacta e intocada.

Depois de confirmar que a sua versão de teste funciona como deveria, copie a versão de teste sobre a versão de produção. É melhor fazer isso fora de horário de pico de uso, e com sua loja corretamente e temporariamente desativada de através do painel PrestaShop.

### Verificando a biblioteca GD <a href="#outrasinformacoes-verificandoabibliotecagd" id="outrasinformacoes-verificandoabibliotecagd"></a>

A biblioteca GD habilitado o PrestaShop manipular imagens ao carregar, especialmente redimensionando-as.

Em uma instalação padrão do PHP, a biblioteca GD deve ser habilitada, se esse é o caso  da sua instalação, as instruções padrão do Windows são:

1. Na raiz do diretório PHP, abra o arquivo `php.ini`.
2. Retire o comentário da linha  `extension=php_gd2.dll`  (aproximadamente no meio do arquivo, no meio de uma longa lista de extensões) deletando ";" no começo da linha.
3. Reinicie os serviços do PHP.

Se você não tem acesso ao arquivo php.ini (que é frequentemente o caso em hospedagem compartilhada), contacte o sua hospedagem informando sobre as suas necessidades.

### Ativando PHP5 <a href="#outrasinformacoes-ativandophp5" id="outrasinformacoes-ativandophp5"></a>

Muitas vezes, os servidores dedicados ou compartilhados podem ter tanto o PHP 4 e o PHP 5 disponíveis, mas apenas o PHP4 é ativado por padrão.

Para instalar o PrestaShop, o PHP 5 deve ser ativado. Se você tentar executar o PrestaShop usando o PHP 4, você receberá vários erros, incluindo esta mensagem de erro muito comum:

```
Parse error: parse error, unexpected T_STATIC, expecting T_OLD_FUNCTION or T_FUNCTION or T_VAR or '}' in [php file] on line X.
```

Por favor, não hesite em postar um relato de erro sobre as dicas necessárias para fazer PrestaShop ser executado no seu serviço de hospedagem, no PrestaShop Forge (você vai precisar de uma conta). Vamos adicionar suas dicas a este guia assim que nós recebê-las.

O que se segue é uma lista de procedimentos dos quais são específicos para algumas hospedagens ...

#### 1&1 <a href="#outrasinformacoes-1-and-1" id="outrasinformacoes-1-and-1"></a>

Adicione esta linha ao seu arquivo  `.htaccess`:

```
AddType x-mapp-php5 .php
```

Para usar o recurso de reescrita de URL , Adicione esta linha ao seu arquivo :

```
Options +FollowSymLinks
RewriteEngine On
```

#### [Free.fr](http://free.fr) <a href="#outrasinformacoes-free.fr" id="outrasinformacoes-free.fr"></a>

Adicione esta linha ao seu arquivo  `.htaccess`:

```
php 1
```

#### OVH <a href="#outrasinformacoes-ovh" id="outrasinformacoes-ovh"></a>

Adicione esta linha ao seu arquivo  `.htaccess`:

```
SetEnv PHP_VER 5
```

Para desativar o global registers:

```
SetEnv REGISTER_GLOBALS 0
```

#### GoDaddy <a href="#outrasinformacoes-godaddy" id="outrasinformacoes-godaddy"></a>

Para visualizar sua versão do PHP:

1. Entre em sua conta de administração.
2. Na seção produtos, clique em hospedagem.
3. Depois selecione a conta de hospedagem desejar usar e clique nela.

Na seção servidor, mostrará a versão do PHP.

Para mudar sua versão PHP:

1. No meu de contexto, selecione linguagem de programação.
2. Selecione a versão do PHP você deseja usar, e clique em continuar.
3. Clique em atualizar.

As mudanças podem demorar 24 horas para finalizarem.

#### Lunarpages Hospedagem <a href="#outrasinformacoes-lunarpageshospedagem" id="outrasinformacoes-lunarpageshospedagem"></a>

1. Entre no endereço de seu cPanel. ele deve estar localizado por exemplo em [http://www.(seu\_dominio).(com/net/org/etc)/cpanel](http://www.\(your\_domain\).\(com/net/org/etc\)/cpanel)
2. Digite seus dados de acesso e clique em entrar.
3. Uma nova página parecerá. Vá até o conjunto de botões na página e clique no que possuir o ícone com o titulo "Habilitar/Desabilitar PHP 5"
4. Uma nova página parecerá. Clique em  "Adicionar PHP 5".

Seu pedido de alteração na linguagem foi enviado. Por favor aguarde 24 horas para que a mudança seja concluída.
