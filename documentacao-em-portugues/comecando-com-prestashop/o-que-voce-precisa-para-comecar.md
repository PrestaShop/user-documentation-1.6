# O que você precisa para começar?

**Sumário**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597243846841 {padding: 0px;}\
div.rbtoc1597243846841 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597243846841 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [O que você precisa para começar](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-Oquevocêprecisaparacomeçar)
  * [Configurações Resumidas](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-ConfiguraçõesResumidas)
  * [Configurações Detalhadas](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-ConfiguraçõesDetalhadas)
    * [Registrando um domínio](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-Registrandoumdomínio)
    * [Encontre uma hospedagem](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-Encontreumahospedagem)
    * [Requisitos Técnicos](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-RequisitosTécnicos)
    * [Ferramentas](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-Ferramentas)
    * [Construa um plano](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-Construaumplano)
    * [Instalando o PrestaShop](o-que-voce-precisa-para-comecar.md#Oquevocêprecisaparacomeçar?-InstalandooPrestaShop)

## O que você precisa para começar <a href="#oquevoceprecisaparacomecar-oquevoceprecisaparacomecar" id="oquevoceprecisaparacomecar-oquevoceprecisaparacomecar"></a>

### Configurações Resumidas <a href="#oquevoceprecisaparacomecar-configuracoesresumidas" id="oquevoceprecisaparacomecar-configuracoesresumidas"></a>

Aqui está uma lista resumida de configurações para você iniciar a instalação do PrestaShop 1.6,  Talvez você não se sinta confortável em ficar lendo instruções extremamente detalhadas, mas caso deseje mais detalhes, abaixo desta seção se encontram as instruções detalhadas.

* Requisitos do Sistema:
  * PHP 5.2 ou superior.
    * Configurações recomendadas (no arquivo `php.ini`): \

      * `allow_url_fopen` setado como On,&#x20;
      * `register_globals` setado como Off,
      * `magic_quotes_*` setado como Off,
      * `safe_mode` setado como Off,
      * `upload_max_filesize` setado como "16M" (ou mais).
    * Extensões PHP que devem estar habilitadas  (no arquivo `php.ini`): PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP.
    * Recomendamos a instalação no servidor: cron/crontab, Memcached.
  * MySQL 5.0 ou mais recente.
  * Será melhor se for: \

    * Hospedagem Unix/Linux.
    * Apache Web Server 1.3 ou mais atual ou um servidor web nginx.
      * Configurações dos módulos Apache: \

        * `mod_rewrite` habilitado,&#x20;
        * `mod_security` desabilitado,
        * `mod_auth_basic` desabilitado.
    * Pelo menos 64 Mb de memória  RAM dedicada para o PHP, quanto mais melhor.
* Acesso aos códigos do seu servidor FTP, seu banco de dados MySQL\

  * Isto deverá ser fornecido pelo seu servidor Web se você não estiver usando uma instalação local.
* Algum editor de texto.
* Algum programa para cessar FTP.
* Algum Navegador Web (se estiver usando Internet Explorer: use a partir do IE8).

Você também precisa saber que domínio sua loja terá, pois é a partir dele que você acessa a loja.

Cheque a página oficial dos requisitos básicos: [http://www.prestashop.com/en/system-requirements](http://www.prestashop.com/en/system-requirements).

Logo após finalizar as configurações, você pode usar este guia de instalação: [http://doc.prestashop.com/display/PS16/Instalando+o+PrestaShop](http://doc.prestashop.com/display/PS16/Instalando+o+PrestaShop).

### Configurações Detalhadas <a href="#oquevoceprecisaparacomecar-configuracoesdetalhadas" id="oquevoceprecisaparacomecar-configuracoesdetalhadas"></a>

O PrestaShop é uma aplicação web: isto significa que ele precisa de um servidor web para funcionar, e também vai precisar de um domínio que os visitantes irão usar para encontrar e acessar a loja.

#### Registrando um domínio <a href="#oquevoceprecisaparacomecar-registrandoumdominio" id="oquevoceprecisaparacomecar-registrandoumdominio"></a>

Antes de você baixar e instalar qualquer coisa, você precisa ter um local onde vai ficar sua loja PrestaShop. Isto é feito de dois componentes: um nome de domínio, e um servidor web. o nome de domínio é a identificação on line do seu website, por exemplo [`examplo.com`](http://example.com) ou [`minhalojaonline.net`](http://myonlineshop.net). Isto é como seu servidor será chamado, e portanto a sua loja também.

Você precisa comprar um domínio para sua loja. Você pode comprar um domínio no mesmo local onde vai contratar sua hospedagem: Muitos serviços de hospedagem oferecem um domínio grátis para novas hospedagens. Geralmente é grátis o primeiro ano de uso, ou enquanto você for cliente daquele serviço de hospedagem. Isto facilita muito na hora de você comprar o pacote (hospedagem+domínio) em apenas um passo.

Caso haja algum problema com a sua hospedagem: se você encontrar-se insatisfeito com o serviço de hospedagem, você pode mudar para uma hospedagem melhor . Isto significa que você vai precisar mudar seus arquivos , dados e nome de domínio para a outra hospedagem.

Os arquivos e banco de dados são fáceis de se mudar, mas, dependendo do host, você pode ter que esperar muito tempo para obter o seu nome de domínio de volta. Desde que você tenha comprado o nome de domínio para você, tecnicamente, o domínio pertence a eles, e eles podem proíbo de transferi-lo para outra hospedagem , ou eles podem te cobrar a mais por isso. E uma vez que o nome de domínio é a sua marca e seu endereço na web, você deve obedecer as regras da hospedagem.

É por isso que muitas vezes é recomendado você obter o seu nome de domínio a partir de um registro de domínio independente ( veja : [http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://en.wikipedia.org/wiki/Domain\_name\_registrar) ) . Tecnicamente, você nunca pode comprar um nome de domínio ; você só pode alugá-lo , na maioria das vezes por uma taxa anual. Isto dá-lhe o direito de usar esse nome de domínio , mas assim que você parar de pagar por isso , não é mais seu e ninguém pode comprá-lo para si. Então, se você pagar por um registo de domínio por fora da sua hospedagem, você pelo menos está livre para mudar para uma hospedagem melhor a qualquer momento, sem pagar nenhuma taxa adicional : basta alterar os endereços de DNS do seu domínio, e dentro de 24 horas a alteração é propagada para o mundo.

Se você preferir comprar o seu nome de domínio de um registrador independente , aqui estão algumas que você pode confiar

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Existem muitos outros. Pergunte aos seus amigos !

#### Encontre uma hospedagem <a href="#oquevoceprecisaparacomecar-encontreumahospedagem" id="oquevoceprecisaparacomecar-encontreumahospedagem"></a>

Agora que você tem um nome de domínio, você precisa instalar PrestaShop. Isto significa que os arquivos PrestaShop precisam estar em um servidor web. Você pode ter um servidor de hospedagem próprio, mas é mais provável que você tenha ou terá sua loja hospedada por um serviço de hospedagem na Internet (ver: [http://en.wikipedia.org/wiki/Internet\_hosting\_service](http://en.wikipedia.org/wiki/Internet\_hosting\_service)), que fornece-lhe uma hospedagem on-line por uma taxa mensal ou anual.

Antes de iniciar uma loja online, primeiro você precisa selecionar um provedor de hospedagem. Praticamente qualquer serviço de hospedagem pode hospedar a solução PrestaShop. No entanto, apenas alguns provedores de hospedagem oferecem servidores otimizados para o PrestaShop (com 1-clique você instalar e atualiza). Aqui está a nossa [lista de parceiros de hospedagem](https://www.prestashop.com/en/ecommerce-hosting).

Ao escolher o sua hospedagem, lembre-se de um requisito fundamental: eles devem fornecê suporte para PHP 5.2 (ou mais recente), a linguagem de programação com a qual o PrestaShop está escrito, e MySQL 5 (ou mais recente), o sistema de banco de dados onde as lojas PrestaShop armazena seus dados. Há mais requisitos: consulte a secção "Requisitos técnicos" abaixo.

PrestaShop Cloud

PrestaShop Inc. pode hospedar seu negócio on-line em seus próprios servidores de hospedagem: o nosso serviço PrestaShop Cloud foi concebido a fim de que comerciantes fiquem livres da necessidade de qualquer conhecimento técnico, tais como instalar ou atualizar PrestaShop .

O serviço é totalmente gratuito, para sempre e para qualquer tipo de loja. É altamente recomendável para empresas com pouca ou nenhuma experiência com a Internet ou computadores.

Você pode criar sua conta no PrestaShop Cloud diretamente no site [http://www.prestashop.com](http://www.prestashop.com) !

#### Requisitos Técnicos <a href="#oquevoceprecisaparacomecar-requisitostecnicos" id="oquevoceprecisaparacomecar-requisitostecnicos"></a>

PrestaShop é uma aplicação que roda em um servidor web, e é escrito usando a linguagem de programação PHP. Ele armazena seus dados em um servidor MySQL .

PHP é uma linguagem de programação de código aberto , usado principalmente para aplicações web. Criado em 1995, desde então se tornou a linguagem de programação mais utilizado pelos desenvolvedores web. Ele usa a sintaxe parecida com C, tornando mais fácil para os desenvolvedores a aprender.

MySQL é um sistema de gerenciamento de banco de dados open-source. Também criado em 1995, que desde então se tornou o sistema de banco de dados mais usado pelos desenvolvedores web . Ele baseia-se na linguagem SQL, a linguagem de base de dados mais amplamente utilizado .

Qualquer que seja o serviço de hospedagem que você escolher, ele deve ter os seguintes componentes instalados no seu servidor web :

* **Sistema**: Unix, Linux or Windows. Unix é altamente recomendável.
* **Web server**: Apache Web server 1.3  versão superior.
* **PHP 5.2 ou versão superior**. Você dever ter o  PHP 5 habilitado(peça para sua hospedagem).
* **MySQL 5.0 ou versão superior**.
* Pelo menos 64 Mb de RAM no seu servidor (128 Mb é mais produtivo, quanto memória mais melhor).

PrestaShop também pode rodar com o servidor Web IIS da Microsoft 6.0 ou posterior, e nginx 1.0 ou posterior .

Mais informações estão disponíveis para administradores de sistema no [Guia de administradores de sistema](http://doc.prestashop.com/display/PS16/System+Administrator+Guide). Certifique-se de lê-lo!

#### Ferramentas <a href="#oquevoceprecisaparacomecar-ferramentas" id="oquevoceprecisaparacomecar-ferramentas"></a>

Você vai precisar de duas ferramentas: um editor de texto, para você poder editar os arquivos, um programa cliente FTP, para que você possa transferir os arquivos do seu computador para o servidor e vice-versa.

**Editor de Texto**

Aqui estão alguns editores de texto bem conhecidos:

* Windows:
  * Notepad++: [http://notepad-plus-plus.org/](http://notepad-plus-plus.org/)
  * UltraEdit: [http://www.ultraedit.com/](http://www.ultraedit.com/)
  * Crimson Editor: [http://www.crimsoneditor.com/](http://www.crimsoneditor.com/)
* OS X:
  * Textmate: [http://macromates.com/](http://macromates.com/)
  * Coda: [http://www.panic.com/coda/](http://www.panic.com/coda/)
  * Smultron: [http://www.peterborgapps.com/smultron/](http://www.peterborgapps.com/smultron/)
* Unix/Linux:
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

Não FAÇA USO de processadores de texto quando você estiver editando os arquivos, como por exemplo usar o Microsoft Word ou o [OpenOffice](http://openoffice.org) Write.

**Cliente FTP**

FTP é a abreviação de "File Transfer Protocol " , ou seja, a forma padrão usado para transferir arquivos de um computador para um servidor web.

Neste guia, vamos usar o Filezilla, que é um programa muito bom e gratuito para acesso cliente  FTP, está disponível para Windows, Mac OS X e Linux. Basta baixá-lo do [http://filezilla-project.org/](http://filezilla-project.org/) e iniciar a sua instalação. Nota: não baixar FileZilla Server, baixe apenas o FileZilla client!

Uma vez que o FileZilla está instalado, você precisará configurá-lo com os parâmetros de conexão para seu servidor web, o que deve ter sido enviado pelo seu site de hospedagem. Caso não tenha, peça para que seu servidor de hospedagem - ou verifique sua caixa de mensagens ou de spam.

Basicamente, os parâmetros necessários são os seguintes:

* **um domínio** ou **um endereço IP**: a localização do servidor FTP do seu espaço de hospedagem.
* **um nome de usuário**: o identificador de conta de hospedagem, que é exclusiva sua.
* **uma senha**: obrigatório por medida de segurança.

Abra o FileZilla , e abra sua ferramenta de gerenciamento de sites. Você pode fazer isso de três maneiras diferentes :

* Pressione Ctrl-S,
* Clique no ícone "Abrir Gerenciamento de sites" , no topo esquerdo,
* Clique no menu "Arquivo", e selecione a opção "Gerenciamento de sites...".

Uma janela se abre.

Para adicionar o seu espaço de hospedagem para o Administrador do Site :

1. Clique no botão "Novo Site". Uma nova entrada é criada na lista de site. Dê-lhe um nome reconhecível .
2. No lado direito, na guia "Geral", digite os parâmetros da sua hospedagem que lhe foi fornecido : servidor, usuário e senha. Você não precisa alterar os outros parâmetros padrão, a menos que sua hospedagem tenha informado.
3. Uma vez que todos os campos são devidamente preenchido, clique no botão " Conectar". Isso vai salvar o seu site na lista, e loga-lo em sua conta, de modo que você pode verificar se tudo funcionou corretamente .

Se o FileZilla não lhe agradar, aqui estão alguns outros clientes FTP bem conhecidos :

* Windows:
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X:
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux:
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

#### Construa um plano <a href="#oquevoceprecisaparacomecar-construaumplano" id="oquevoceprecisaparacomecar-construaumplano"></a>

Você deve decidir onde você quer hospedar sua loja PrestaShop. Existem quatro possibilidades relacionadas com seu domínio:

* Na Raiz do seu domínio: [http://www.examplo.com/](http://www.example.com/)
* Dentro de uma pasta: [http://www.examplo.com/loja/](http://www.example.com/shop/)
* Em um subdomínio: [http://loja.examplo.com/](http://store.example.com/)
* Em uma pasta do subdomínio: [http://roupas.examplo.com/boutique/](http://clothes.example.com/boutique/)

Observação: Graças a função multilojas, você pode ter quantas lojas quiser com apenas uma instalação do PrestaShop 1.6, cada uma com seu próprio domínio caso seja necessário. Você deverá estar logado na sua conta para decidir onde ficará cada instalação.\
Independente de onde você planejar instalar, a loja padrão sempre estará localizada onde o  PrestaShop está instalado.

#### Instalando o PrestaShop <a href="#oquevoceprecisaparacomecar-instalandooprestashop" id="oquevoceprecisaparacomecar-instalandooprestashop"></a>

Finalmente, agora que todos os requisitos foram cumpridos, você pode usar o guia de instalação: [http://doc.prestashop.com/display/PS16/Instalando+o+PrestaShop](http://doc.prestashop.com/display/PS16/Instalando+o+PrestaShop).
