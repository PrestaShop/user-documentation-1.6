# Instalando o PrestaShop

**Sumário**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597243847048 {padding: 0px;}\
div.rbtoc1597243847048 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597243847048 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Instalando o PrestaShop](instalando-o-prestashop.md#InstalandooPrestaShop-InstalandooPrestaShop)
  * [Instruções resumidas para instalação](instalando-o-prestashop.md#InstalandooPrestaShop-Instruçõesresumidasparainstalação)
  * [Instruções detalhadas para instalação](instalando-o-prestashop.md#InstalandooPrestaShop-Instruçõesdetalhadasparainstalação)
    * [Faça o Download e descompacte o arquivo PrestaShop](instalando-o-prestashop.md#InstalandooPrestaShop-FaçaoDownloadedescompacteoarquivoPrestaShop)
    * [Enviando o  PrestaShop para o servidor](instalando-o-prestashop.md#InstalandooPrestaShop-EnviandooPrestaShopparaoservidor)
    * [Criando o banco de dados da sua loja](instalando-o-prestashop.md#InstalandooPrestaShop-Criandoobancodedadosdasualoja)
    * [Iniciando o instalador automático](instalando-o-prestashop.md#InstalandooPrestaShop-Iniciandooinstaladorautomático)
    * [Concluindo a Instalação](instalando-o-prestashop.md#InstalandooPrestaShop-ConcluindoaInstalação)

Este capítulo foi escrito para pessoas que pretendam instalar o PrestaShop em seu servidor de hospedagem na internet.

Se você deseja instalar o PrestaShop em seu próprio computador, você deve primeiro seguir as instruções desta página : [Instalar PrestaShop em seu computador](instalando-o-prestashop-em-seu-computador.md).

Se você já leu as instruções dessa página, vá para a seção "Criando um banco de dados para a sua loja " nesta página atual.

## Instalando o PrestaShop <a href="#instalandooprestashop-instalandooprestashop" id="instalandooprestashop-instalandooprestashop"></a>

O PrestaShop é muito fácil de instalar. Uma vez que todos os arquivos estão no seu servidor web, você conseguirá começar a configurar a sua loja em nada menos que 5 minutos na maioria dos casos: o processo de instalação é muito simples, pois o instalador cuida de tudo para você. usuários com menos experiência podem precisar entre 10 e 20 minutos para completar todo o processo com sucesso.

\
Antes de começar a instalação, certifique-se que você tenha todos os requisitos disponíveis com você: espaço em um servidor de hospedagem, nome de domínio , cliente FTP, um editor de texto. Ter certeza de estar primeiramente seguindo as instruções da página  "[O que você precisa para começar?](http://doc.prestashop.com/pages/viewpage.action?pageId=47185938)[" .](http://doc.prestashop.com/pages/viewpage.action?pageId=47185938)

Alguns servidores de hospedagem oferecem a instalação em apenas 1 clique, a fim de poupar tempo e você começar ainda mais rápido. Usando um destes você pode reduzir drasticamente o tempo de instalação se você for um usuário inexperiente.

* A2 Hosting: [https://partners.a2hosting.com/solutions.php?id=3682\&url=311](https://partners.a2hosting.com/solutions.php?id=3682\&url=311)
* OVH Hosting: [http://www.ovh.com/fr/solutions/prestashop/?pk\_campaign=partenariatprestashop\&pk\_kwd=pagefr](http://www.ovh.com/fr/solutions/prestashop/?pk\_campaign=partenariatprestashop\&pk\_kwd=pagefr)
* 1&1 Hosting: [http://being.successfultogether.co.uk/click.asp?ref=657157\&site=3759\&type=text\&tnb=32](http://being.successfultogether.co.uk/click.asp?ref=657157\&site=3759\&type=text\&tnb=32)

Esses servidores de hospedagem usam as seguintes bibliotecas de script :

* SimpleScripts: [https://www.simplescripts.com/script\_details/install:PrestaShop](https://www.simplescripts.com/script\_details/install:PrestaShop),
* Installatron: [http://installatron.com/apps?locale=en#cmd=browser\&display=prestashop](http://installatron.com/apps?locale=en#cmd=browser\&display=prestashop),
* Softaculous: [http://www.softaculous.com/apps/ecommerce/PrestaShop](http://www.softaculous.com/apps/ecommerce/PrestaShop).

Alguns desses scripts até mesmo suportam a atualização em apenas 1 clique, isto algo de valor inestimável.

Outros servidores de hospedagem têm os seus próprios scripts de instalação. Verifique no seu servidor de hospedagem para obter mais informações.

Por último, mas não menos importante, o PrestaShop tem a sua própria solução de hospedagem: registando-se no site [PrestaShop.com](http://prestashop.com), você pode criar uma loja PrestaShop 100% grátis na nossa nuvem de hospedagem, e assim, deixar todos os obstáculos técnicos de hospedagem para nossa própria equipe, e poder se concentrar em sua loja, clientes e vendas. Visite [https://www.prestashop.com/](https://www.prestashop.com/) para mais informações.

### Instruções resumidas para instalação <a href="#instalandooprestashop-instrucoesresumidasparainstalacao" id="instalandooprestashop-instrucoesresumidasparainstalacao"></a>

Aqui estão as instruções para aqueles que já estão acostumados com a instalação de aplicações PHP / MySQL em servidores de hospedagem. Se a falta de detalhes lhe incomodar, você encontrará instruções detalhadas na próxima seção neste capítulo.

1. Baixe e descompacte o pacote PrestaShop, caso você ainda não tenha.
2. Criar um banco de dados para a loja PrestaShop em seu servidor de hospedagem, se for possível. No caso de não havia nenhum usuário MySQL que tinha todos os privilégios para acessar e modificar esse banco de dados, crie-o também.
3. Faça o upload dos arquivos PrestaShop e pastas, para o local escolhido em seu servidor de hospedagem. Não carregue a pasta raiz / prestashop diretamente:apenas envie os arquivos e pastas que ela contém.
4. Execute o script de instalação PrestaShop, acessando o URL pública na localização escolhida em um navegador web. Esta deve ser a URL onde você carregou os arquivos PrestaShop.
5. Siga as instruções em cada tela do instalador.
6. Uma vez que a instalação é feita , exclua a pasta de instalação /install e anote o novo endereço para a pasta admin / , que foi criada no intuito de ser exclusiva para sua loja, por razões de segurança .

O PrestaShop agora deverá estar instalado e pronto para ser configurado! Continue lendo a partir do capítulo  "Primeiros passos com PrestaShop 1.6" do Guia do Usuário.

### Instruções detalhadas para instalação <a href="#instalandooprestashop-instrucoesdetalhadasparainstalacao" id="instalandooprestashop-instrucoesdetalhadasparainstalacao"></a>

#### Faça o Download e descompacte o arquivo PrestaShop <a href="#instalandooprestashop-facaodownloadedescompacteoarquivoprestashop" id="instalandooprestashop-facaodownloadedescompacteoarquivoprestashop"></a>

```
```

Você pode baixar a última versão do PrestaShop em [http://www.prestashop.com/en/download](http://www.prestashop.com/en/download).

![](<../../.gitbook/assets/39125009 (1).png>)

Você só tem uma opção de download: a última versão estável, pronta para todos os tipos de lojas.

Se você precisar fazer download de qualquer das versões anteriores, vá a este endereço: [http://www.prestashop.com/en/developers-versions](http://www.prestashop.com/en/developers-versions). Vá até a seção " versões anteriores" e selecione a versão desejada.

Saiba que nunca é recomendado o uso de qualquer outra versão além da atual e estável.

Clique no botão "Download " e salve o arquivo no seu computador (como por exemplo na área de trabalho ). Você deve obter um arquivo chamado " prestashop\_1.6.0.4.zip " ( ou equivalente, dependendo dos números de versão ).

O arquivo baixado é um arquivo compactado, ou seja, um arquivo que contém todos os arquivos do PrestaShop em forma comprimida. A fim de continuar com o processo, você deve descompactar o arquivo.

Se seu sistema operacional não suporta nativamente arquivos compactados como o Zip, você pode baixar e instalar uma ferramenta dedicada para esta tarefa, tais como:

* Windows:
  * 7-zip: [http://www.7-zip.org/](http://www.7-zip.org/)
  * WinZip: [http://www.winzip.com/win/en/index.htm](http://www.winzip.com/win/en/index.htm)
  * WinRAR: [http://www.rarlab.com/](http://www.rarlab.com/)
* Mac OS X:
  * iZip: [http://www.izip.com/](http://www.izip.com/)
  * WinZip Mac: [http://www.winzip.com/mac/](http://www.winzip.com/mac/)
  * Zipeg: [http://www.zipeg.com/](http://www.zipeg.com/)

Usando uma ferramenta de descompactação Zip, extraia o conteúdo do arquivo em um local conhecido no seu disco rígido (como na área de trabalho novamente). **Não faça upload do arquivo Zip diretamente para o seu servidor de hospedagem**.

O arquivo Zip tem dois itens em sua raiz:

* A pasta " prestashop ", que contém todos os arquivos PrestaShop que em breve você vai enviar para a sua hospedagem.
* O arquivo " Install\_PrestaShop.html ", que abre esta mesma página no seu navegador padrão.

O arquivo " Install\_PrestaShop.html " não devem ser enviado para seu servidor de hospedagem.

#### Enviando o  PrestaShop para o servidor <a href="#instalandooprestashop-enviandooprestashopparaoservidor" id="instalandooprestashop-enviandooprestashopparaoservidor"></a>

Agora você deve ter um espaço de hospedagem à sua disposição (se não , leia o artigo " O que você precisa para começar " deste guia ), e tenha uma pasta em seu disco rígido com o arquivo PrestaShop descompactado.

Nesta etapa você deve fazer o upload dos arquivos do PrestaShop em seu espaço de hospedagem. Isso será feito quando você conectar seu computador ao servidor de hospedagem usando uma ferramenta conhecida como "cliente FTP", que você deve ter instalado durante a leitura do artigo " O que você precisa para começar ". Nós estaremos usando o FileZilla ( [http://filezilla-project.org/](http://filezilla-project.org/) ).

Faça a conexão com sua hospedagem usando seu cliente FTP, informando os detalhes de conexão fornecidos pelo seu provedor de hospedagem (se não possuir, contacte a sua hospedagem). Uma vez conectado, é hora de transferir os arquivos do PrestaShop do seu computador para o servidor.

Dentro do FileZilla (ou qualquer outro cliente de FTP) , navegue até suas pastas locais até encontrar aquela que contém os arquivos do PrestaShop. Mantenha ele aberto na seção " site local" à esquerda.

![](<../../.gitbook/assets/23037805 (1).png>)

Na seção "local remoto" (à direita ), navegue até o local onde deseja que o PrestaShop  seja instalado ( raiz do domínio , sub- pasta , sub- domínio ... ) . Isso pode mudar muito, dependendo tanto seu servidor de hospedagem e às suas necessidades:

* Sua hospedagem:
  * Algumas hospedagens podem exigir que você coloque os arquivos em uma pasta específica, como / htdocs, / public\_html, / web, / www, /[seudominio.com](http://yourdomainname.com/), etc.
  * Outras hospedagens irão simplesmente conectá-lo diretamente no espaço de upload adequada.
* O que você precisa:
  * Se você quer que a sua loja a seja o site principal  para o seu domínio (ou seja, [http://www.examplo.com](http://www.example.com/)), envie o PrestaShop para a pasta raiz do espaço de upload (que pode depender do host).
  * Se você quer a sua loja de esteja em uma sub-pasta de seu nome de domínio ([http://www.examplo.com/loja](http://www.example.com/shop)), você deve primeiro criar a referida pasta através do FileZilla (clique com o botão direito e escolha "Criar diretório"), em seguida, faça o upload do PrestaShop nessa pasta.
  * Se você quer que a sua loja de esteja em um sub-domínio do seu domínio ([http://shop.example.com](http://shop.example.com/)), você deve primeiro criar o referido sub-domínio. Isso depende do seu host: você pode ser capaz de fazê-lo simplesmente adicionando uma nova pasta com o seu cliente FTP, ou você pode ter que criar o sub-domínio através do painel de administração de sua hospedagem. Leia a documentação de suporte de sua hospedagem primeiro. Uma vez criado, navegue para a pasta do sub-domínio, e faça o upload do PrestaShop lá.\
    \
    \


No lado esquerdo do FileZilla, você deve agora ter a pasta local onde você guarda os arquivos do PrestaShop extraídos do arquivo Zip, e no lado direito, o local de destino. Se você não tiver feito isso ainda , upload é simples: selecione todos os arquivos e pastas a partir da pasta local ( use Ctrl- A) , e arraste e solte na pasta remota, ou clique com o botão direito do mouse e na seleção e no menu de contexto escolha " Enviar ".

![](<../../.gitbook/assets/23037806 (1).png>)

O envio pode levar vários minutos, pois o PrestaShop usa mais de 7500 arquivos e quase 1000 pastas. Depois de um tempo, todos os arquivos e pastas do PrestaShop devem estar online.

#### Criando o banco de dados da sua loja <a href="#instalandooprestashop-criandoobancodedadosdasualoja" id="instalandooprestashop-criandoobancodedadosdasualoja"></a>

Antes que você possa realmente instalar o PrestaShop, você precisa ter certeza de que seu servidor MySQL tem um banco de dados pronto para os dados do PrestaShop. Se não, você deve criar um.

Criação de um banco de dados pode ser feito usando qualquer ferramenta de administração de banco de dados. Nós estaremos usando a ferramenta phpMyAdmin ( [http://www.phpmyadmin.net/](http://www.phpmyadmin.net/) ), que deve vir pré-instalado na maioria das hospedagens.

Algumas hospedagens preferem que seus os clientes usem um painel de controle gráfico, como cPanel, Plesk ou um feito sob encomenda. Certifique-se de ler a documentação do seu servidor de hospedagem a respeito do banco de dados MySQL, e crie um banco de dados para a sua loja, seguindo suas explicações específicas.

Conecte-se ao phpMyAdmin usando suas credenciais de acesso, que o seu servidor de hospedagem lhe forneceu. Ele deve ser acessível através de uma URL padrão, vinculado ao seu nome de domínio ou nome de domínio do servidor de hospedagem.

![](<../../.gitbook/assets/23037808 (1).png>)

Na coluna à esquerda, você pode ver as bases de dados disponíveis atualmente no seu servidor MySQL. Alguns deles não devem ser alterados, pois eles são utilizadas pelo phpMyAdmin ou pela hospedagem: phpmyadmin , mysql, information\_schema, performance\_schema entre outros. Leia a documentação do servidor de hospedagem para saber se um destes pode ser usado como um banco de dados ou não.

De qualquer maneira, você pode criar um novo banco de dados, basta ir na aba "Databases" ou "Banco de dados" e usar o formulário de cadastro, adicionando um nome abaixo do titulo "Create new database" ou "Criar uma nova base de dados". Basta digitar um nome que ainda não está sendo usado, e clicar em "Create" ou "Criar". O nome do banco de dados será adicionado à lista na esquerda. Agora você pode usá-lo para armazenar dados do PrestaShop .

#### Iniciando o instalador automático <a href="#instalandooprestashop-iniciandooinstaladorautomatico" id="instalandooprestashop-iniciandooinstaladorautomatico"></a>

Agora vem a parte onde tudo é iniciado automaticamente: a instalação do PrestaShop.

O processo de instalação é muito fácil, como ele é particionado pelo instalador automático do PrestaShop. Você deve ser capaz de navegar por ele em apenas alguns minutos. faça a leitura de cada página cuidadosamente para que não se perca nenhuma informação no processo.

Para iniciar o instalador, abra no seu navegado o local onde o PrestaShop foi instalado em sua hospedagem: o script irá detectar automaticamente que PrestaShop ainda não está instalado, e vai levá-lo para a instalação automática.

Você também pode digitar diretamente o endereço da pasta  /install: [http://www.loja\_exemplo.com/local\_do\_prestashop/install](http://www.example.com/prestashop\_folder/install) .

Se você está fazendo uma instalação em seu próprio computador, a instalação deve ser feita na pasta PrestaShop em seu servidor web local, que deve estar disponível por exemplo em [http://127.0.0.1/prestashop](http://127.0.0.1/prestashop).

A partir daí, você só tem que ler, clicar, e preencher alguns formulários.

Há 6 etapas. No topo da página , o assistente de instalação lhe dá uma visualização de onde você está no processo: os círculos cinza transformam-se em marcas de seleção verdes após cada etapa é concluída .

![](<../../.gitbook/assets/39125004 (1).png>)

**Passo 1: Página de Boas Vindas**

Esta página é uma introdução rápida para o processo de instalação. Você pode escolher o idioma em que o instalador irá exibir suas instruções.

![](<../../.gitbook/assets/39125006 (1).png>)

Você também terá um link para o site da documentação ( [http://doc.prestashop.com/](http://doc.prestashop.com/) ), e o número de telefone de suporte do PrestaShop. Você pode aprender mais sobre o nosso serviço de suporte, indo até a página [http://support.prestashop.com/en/](http://support.prestashop.com/en/\~\~V).

Selecione o idioma no qual você deseja que o instalador configure sua loja, em seguida, clique no botão "Next". Isso também irá definir o idioma padrão para a sua instalação da loja PrestaShop, mas outras línguas também estarão disponíveis para que você possa permitir a tradução da loja.

**Passo 2: Licença do PrestaShop**

Esta segunda página é um requisito simples: O PrestaShop é gratuito e distribuído sob um determinado conjunto de licenças de código aberto.Você não deve usar este software se você não concordar com os termos das licenças, e este passo requer que você concorde explicitamente com a licença.

Leia a licença de uso do PrestaShop:

* _Open Software License 3.0_ para o PrestaShop, que você pode ler na página [http://www.opensource.org/licenses/OSL-3.0](http://www.opensource.org/licenses/OSL-3.0).&#x20;
* _Academic Free License 3.0_ para os módulo e temas, que você pode ler na página [http://opensource.org/licenses/AFL-3.0](http://opensource.org/licenses/AFL-3.0).

![](<../../.gitbook/assets/39125007 (1).png>)

Você deve concordar com ambas as licenças, para poder instalar o PrestaShop.

Para acessar o próximo passo, você deve marcar a opção "Eu concordo com os termos e condições"  e clicar em "Próximo". Se você não concorda explicitamente com as licenças, você não pode instalar o PrestaShop: o botão "Próximo" não vai estar clicável caso você não marque a opção.

**Passo 3 & 4: Compatibilidade do sistema & Informações da loja**

A terceira página faz uma rápida verificação de todos os parâmetros do servidor de hospedagem. Na maioria dos casos, você não vai ver esta página, porque se nada de errado for encontrado, você é levado diretamente para a quarta página , " informações da loja". Se isso acontecer, você pode ver as informações da terceira página, clicando no link "compatibilidade do sistema" na barra lateral esquerda.

Se algo der errado durante a verificação de configuração do servidor, que acontece na terceira etapa, o instalador exibe a página "compatibilidade do sistema", onde você pode ver todas as verificações que falharam.

**Compatibilidade do sistema**

Esta página verifica se tudo está OK com a configuração do servidor de hospedagem: configuração do PHP, permissões de arquivos e pastas, ferramentas de terceiros, etc.

![](<../../.gitbook/assets/39125008 (1).png>)

Se alguma coisa der errado, o instalador irá parar aqui, permitindo que você veja os poucos detalhes técnicos que precisam de correção, seja mudar a configuração do PHP ou atualizar as permissões de arquivo .

![](<../../.gitbook/assets/39125010 (1).png>)

Aqui está uma lista das verificações que são executadas durante este terceiro passo:

| O que deve ser verificado                                      | Como / onde corrigir?                                                                                        |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| O PHP 5.1.2 ou mais recente está instalado?                    | Na Hospedagem                                                                                                |
| O PrestaShop pode fazer o upload de arquivos?                  | Arquivo php.ini (`file_uploads`)                                                                             |
| O PrestaShop pode criar novos arquivos e pastas?               | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| A biblioteca GD está instalada ?                               | php.ini file (`extension=`[`php_gd2.so`](http://php\_gd2.so))                                                |
| O suporte ao MySQL está instalado?                             | php.ini file (`extension=`[`php_pdo_mysql.so`](http://php\_pdo\_mysql.so))                                   |
| Permissão recursiva de gravação em \~/config/                  | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/cache/                   | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/log/                     | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/img/                     | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/mails/                   | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/modules/                 | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/override/                | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/themes/default/lang/     | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/themes/default/pdf/lang/ | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/themes/default/cache/    | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/translations/            | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/upload/                  | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/download/                | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| Permissão recursiva de gravação em \~/sitemap.xml              | Navegador de arquivos / Cliente FTP / Linha de comando                                                       |
| O PrestaShop pode abrir URLs externas?                         | [Arquivo php.in](http://php.in) (`allow_url_fopen`)                                                          |
| No PHP a opção "register global" está off?                     | Arquivo php.ini (`register_globals`)                                                                         |
| A compressão do GZIP está ativada?                             | Arquivo .htaccess                                                                                            |
| A extensão Mcrypt está disponível?                             | Arquivophp.ini (leia [http://php.net/manual/en/mcrypt.setup.php](http://php.net/manual/en/mcrypt.setup.php)) |
| No PHP a opção "magic quotes" está desativada?                 | Arquivo php.ini (`magic_quotes_gpc`)                                                                         |
| A extensão Dom está carregada?                                 | `--enable-dom` compile time option                                                                           |
| A extensão PDO MySQL está carregada?                           | Arquivo php.ini (`extension=`[`php_pdo_mysql.so`](http://php\_pdo\_mysql.so))                                |

Alterar a configuração do PHP é algo que só pode ser feito observando-se cada caso, e também depende do seu nível de acesso ao seu servidor de hospedagem, portanto,deve ser explicado em detalhes, a alteração das permissões de arquivo é algo bem mais fácil de explicar.

As permissões são as formas como um sistema de arquivos concede direitos de acesso para usuários específicos ou grupos de usuários, controlando a sua capacidade de ver ou fazer alterações em arquivos e pastas. O instalador precisa fazer várias alterações para os arquivos que você carregou, e se o sistema de arquivos não permite essas mudanças através de permissões adequadas, então o instalador não pode completar o seu processo.

Assim, se o instalador mostrar que alguns arquivos ou pastas não tem permissão adequada, você tem que alterar essas permissões você mesmo. Isso vai exigir que você acesse seus arquivos em seu servidor de hospedagem e portanto, você irá usar o seu cliente FTP (como FileZilla) ou via linha de comando.

Acesse a conta de sua hospedagem usando o cliente FTP, navegue até a pasta da instalação do PrestaShop, e encontre as pastas que necessitarão de alteração das permissões indicadas pelo instalador.

CHMOD

Para mudar as permissões de arquivo ou pasta em um sistema Unix / Linux você deve usar o comando "CHMOD", leia para esta página para mais informações : [http://en.wikipedia.org/wiki/Chmod](http://en.wikipedia.org/wiki/Chmod) - você pode encontrar mais informações sobre permissões de arquivo aqui também: [http://www.elated.com/articles/understanding-permissions/](http://www.elated.com/articles/understanding-permissions/) .\
Para dar para arquivos ou pastas uma permissão de escrita você pode escrever o comando "chmod 755 nome\_do\_arquivo.extensao " ou "CHMOD 775 nome\_do\_arquivo.extensao", dependendo da hospedagem.

Algumas hospedagens podem exigir que você utilize o comando CHMOD 777, embora não seja recomendado para algo mais do que alguma necessidade temporária e logo após a execução da tarefa volte para as permissões padrão.\
Se você tiver que usar o comando CHMOD 777 nas pastas para instalar o PrestaShop, certifique-se de mudar para um ambiente mais seguro logo após a instalação (por exemplo, 775 para pastas e 664 para arquivos).\
Leia a documentação do seu servidor de hospedagem com cuidado.

Graças ao FileZilla (e a maioria dos clientes FTP), você não precisa usar qualquer comando Unix. A maioria dos clientes FTP tornam possível alterar as permissões de forma fácil e graficamente: depois de ter encontrado um arquivo ou pasta que você precisa de alterar as permissões, clique com o botão direito sobre ele e, no menu de contexto, escolha a opção "permissões de arquivo ..." . Ele irá abrir uma pequena janela.

![](<../../.gitbook/assets/23038066 (2).png>)

\
Dependendo da configuração do servidor (que nem sempre temos nas mãos), você terá que marcar tanto o "Ler" como o  "Executar" nas opções, e pelo menos,  deixar o "dono" e o "Grupo" com a opção de  "Escrever". Alguns servidores de hospedagem podem exigir que você marque a opção "Escrever" para o publico, mas tenha cuidado com essa configuração pois: ela raramente é uma boa coisa pois qualquer pessoa será capaz de editar o conteúdo de sua instalação do PrestaShop no seu servidor.

Algumas pastas podem precisar que as permissões de todos os seus arquivos e sub-pastas também sejam alterados. Nesse caso, marque a opção "Aplicar nos subdiretórios".

Enquanto você altera as permissões com seu cliente de FTP, você deve verificar regularmente se você fez as alterações corretas, executando verificações de compatibilidade do instalador novamente: clicando no botão do instalador "Atualizar essas configurações" quantas vezes for necessário.\
Uma vez que todos os indicadores estão verdes, você pode clicar em "Próximo". Se você não conseguir todos os indicadores verdes, pelo menos, certifique-se que o instalador exiba a mensagem "Compatibilidade com o PrestaShop e o ambiente do sistema foi verificada!" no topo da página.

**Informações da loja**

Este é o lugar onde você pode começar a personalizar a sua loja: dar-lhe um nome, indicar a sua principal atividade, e indicar a informações pessoais sobre o proprietário da loja (pois há uma ligação legal na maioria dos países ) ...

Não use uma vírgula ou dois pontos no nome de sua loja, isso poderia gerar algum erro de configuração (por exemplo, o e-mail pode não funcionar corretamente).\
Você pode substituir no título a vírgula por traço. Por exemplo , use " MinhaLoja - O melhor lugar para comprar itens" em vez de " MinhaLoja : O melhor lugar para comprar itens".

![](<../../.gitbook/assets/39125012 (1).png>)

Esta é a tela onde também onde você irá escolher a senha para entrar no painel de administração de sua loja - escolha com sabedoria para que você posso se lembrar, mas certifique-se de que é uma senha segura também!

Clique em "Próximo " para continuar.

**Passo 5: Configuração do sistema**

Esta página contém um formulário que permite que você informe ao PrestaShop onde o servidor de banco de dados está, e qual banco de dados a será usado, juntamente com alguns outros detalhes. Todas estas informações devem ter sido fornecidas a você pela sua hospedagem .

![](<../../.gitbook/assets/39125013 (1).png>)

Preencha todos os campos com as informações de conexão de banco de dados fornecido pelo seu servidor de hospedagem:

* **Endereço do servidor de banco de dados.** O endereço do seu servidor MySQL. Ele pode estar ligado ao seu nome de domínio (ou seja, [http://sql.examplo.com](http://sql.example.com)), vinculado ao seu host (ou seja [http://mysql2.exemplo.com](http://mysql2.alwaysdata.com)), ou simplesmente ser um endereço IP (ou seja 46.105.78.185 ).
* **Nome do banco de dados.** O nome do banco de dados onde você quer que o PrestaShop armazene seus dados. Você deve indicar o banco de dados que foi criado no seu servidor MySQL, ou o que você criou usando o phpMyAdmin (ou qualquer outra ferramenta SQL) na seção "Criando o banco de dados da sua loja" deste guia.
* **Usuário do banco de dados.** O nome do usuário MySQL que tem acesso ao seu banco de dados.
* **Senha do banco.** A senha do usuário do MySQL.
* **Mecanismo de armazenamento.** O mecanismo de armazenamento é o núcleo de seu servidor de banco de dados. O InnoDB é o padrão e você deve usá-lo, mas se você possuir mais técnico você pode querer escolher um outro mecanismo. Geralmente, não há necessidade de alterar a configuração padrão.
* **Prefixo das Tabelas.** O prefixo para as tabelas de banco de dados "PS\_" é o padrão, resultando nas tabelas PrestaShop SQL com nomes como "ps\_cart" ou "ps\_wishlist"; mas se você precisa instalar mais de uma instância do PrestaShop no mesmo banco de dados, então você deve usar um prefixo diferente para cada instalação. No entanto, nós recomendamos que você crie um banco de dados por instalação do PrestaShop, se o seu host permite. Melhor ainda: fazer uma instalação do PrestaShop, e ativar o recurso multistore, a fim de gerenciar muitas lojas a partir do mesmo painel de administração do PrestaShop.
* **Apague tabelas existentes.** Isto só está disponível no modo "Desenvolvimento". Ao reinstalar o PrestaShop, você pode optar por eliminar as tabelas de banco de dados do PrestaShop existentes, a fim de começar em uma base limpa.

Clique no botão " Testar conexão com o banco de dados", a fim de verificar se você preencheu as informações do servidor corretamente.

Clique em " Próximo": a instalação irá iniciar a configuração de sua loja, criar e preencher as tabelas de banco de dados, etc. Isso pode demorar alguns minutos: por favor, seja paciente e espere todo o procedimento terminar!

![](<../../.gitbook/assets/39125014 (1).png>)

O instalador faz o seguinte:

* Cria o arquivo settings.inc.php, com as suas configurações.
* Cria as tabelas de banco de dados.
* Cria a loja padrão com o seu idioma padrão.
* Preenche as tabelas de banco de dados.
* Configura as informações da loja.
* Instala os módulos padrão.
* Instala os dados de demonstração ( produtos, categorias, usuários , páginas CMS , etc.).
* Instala o tema padrão.

Uma vez que tudo está pronto, sua loja está instalado e pronta para ser configurada!

#### Concluindo a Instalação <a href="#instalandooprestashop-concluindoainstalacao" id="instalandooprestashop-concluindoainstalacao"></a>

Como você pode ler esta é a página final do processo de instalação, há apenas duas opções de ações a serem executadas antes de deixar o instalador.

![](<../../.gitbook/assets/39125016 (1).png>)

Uma maneira fácil de melhorar a segurança da sua instalação é apagar alguns arquivos importantes e pastas. Isso é feito usando o seu cliente de FTP, diretamente no servidor . Os itens a serem excluídos são:

* A pasta "/install"  (obrigatório).
* A pasta "/docs"  (opcional), a menos que você precise para testar a ferramenta de importação com os arquivos de importação de exemplo que esta pasta contém.
* O arquivo  "[README.md](http://readme.md)"  (opcional).

Clique no botão "Gerenciar  loja ", para que você seja levado para a área de administração da sua loja.

Outra forma de garantir a sua instalação é a utilização de um nome personalizado para a pasta de administração: altere a pasta "admin" para algo exclusivo para sua loja, como " 4dmin-1537 " ou " MySecReT4dm1n ".\
**Anote o novo nome para a  pasta "admin"**, porque a partir de agora você vai acessar suas páginas de administração usando esse nome no final do endereço!

Finalmente, a fim de fechar todas as brechas de ações potencialmente maliciosas, use o seu cliente FTP para atualizar os arquivos e permissões de pastas para 664, ou 666 se a sua hospedagem o exigir. Se você verificar que as permissões de arquivos que você setou impedem que alguns módulos funcionem, você deve definir as permissões de volta para 755 .

**Parabéns! A instalação está concluída.**

Faça login na área administrativa do PrestaShop, indo para a pasta que foi renomeada, anteriormente chamada de " admin", e comece a preencher o seu catálogo com os produtos, adicionando transportadoras e os custos de transporte, acrescentando fabricantes e fornecedores, mudando o tema  e geralmente, a configuração de muitas definições de acordo seu gosto e necessidade. Consulte o guia do usuário " Primeiros passos com PrestaShop 1.6 ", para obter mais informações:[First steps with PrestaShop 1.6](http://doc.prestashop.com/display/PS16/First+steps+with+PrestaShop+1.6).

Você deve fazer backup regularmente de seu banco de dados e arquivos, de preferência em mais de um computador, em caso de problemas relacionados ao hardware ou a segurança .
