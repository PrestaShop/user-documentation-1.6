# Instalando o PrestaShop em seu computador

Você pode querer instalar PrestaShop em sua máquina local, a fim de testá-lo antes de investir o dinheiro em um servidor e domínio, ou para personalizar sua loja local antes de enviar suas modificações para a instalação do PrestaShop que já está online.

A instalação de qualquer aplicação web localmente requer que você instale primeiro o ambiente adequado, ou seja, o servidor web Apache, o intérprete de linguagem PHP, o servidor de banco de dados MySQL, e, idealmente, a ferramenta phpMyAdmin. Isto é conhecido como um AMP: Apache + MySQL + PHP. Ela existe para muitos sistemas operacionais, o que proporciona uma outra letra para a sigla: WAMP (Windows + Apache + MySQL + PHP), MAMP (Mac OS X + ...) e LAMP (Linux + ...).

## Escolhendo um pacote MySql, Apache e PHP <a href="#instalandooprestashopemseucomputador-escolhendoumpacotemysql-apacheephp" id="instalandooprestashopemseucomputador-escolhendoumpacotemysql-apacheephp"></a>

Isso exigiria que você fosse bastante técnico; Felizmente existem muitos pacotes pré-construídos que você pode instalar facilmente. Isso não impede que você de tenha que chamar um técnico aqui ou ali, mas eles já fornecem uma grande ajuda. Uma vez que todos os itens compactados são open-source, esses instaladores são a maior parte do tempo grátis. Aqui está uma lista de instaladores AMP gratuitos:

* EasyPHP: [http://www.easyphp.org/](http://www.easyphp.org/) (Windows)
* MAMP: [http://www.mamp.info/](http://www.mamp.info/) (Mac OS X)
* WampServer: [http://www.wampserver.com/en/](http://www.wampserver.com/en/) (Windows)
* XAMPP: [http://www.apachefriends.org/en/xampp.html](http://www.apachefriends.org/en/xampp.html) (Windows, Mac OS X, Linux, Solaris)

EasyPHP tem um pacote especial all-in-one, o que inclui uma instalação de pronta para usar do PrestaShop 1.6! Essa é a maneira mais fácil de descobrir a nova versão do PrestaShop, para os desenvolvedores desenvolverem temas e módulos.

Faça o Download Aqui: [http://www.easyphp.org/prestashop.php](http://www.easyphp.org/prestashop.php)

Escolha o pacote que você sinta o mais confortável, e instale.

## Verificando se tudo está funcionando <a href="#instalandooprestashopemseucomputador-verificandosetudoestafuncionando" id="instalandooprestashopemseucomputador-verificandosetudoestafuncionando"></a>

Antes de ir em frente com este tutorial de instalação do PrestaShop, certifique-se de que todos os componentes do seu pacote AMP funcionam corretamente:

*   **O servidor web deve ser instalado e funcionando.** Você deve ser capaz de acessá-lo através de seu navegador, digitando "127.0.0.1" na barra de endereços.\
    &#x20;

    [http://127.0.0.1](http://127.0.0.1) é o mesmo que "localhost", que significa "computador local": é um endereço de loopback que direciona o navegador para o servidor web local.\
    Com efeito, [http://127.0.0.1](http://127.0.0.1) e [http: //localhost](http://doc.prestashop.com/http:%20/localhost) são sinônimos: você pode usar um ou o outro alternadamente, ambos irão enviá-lo para a pasta raiz do seu servidor web local.

    Alguns servidores web pode não ser capaz de iniciar porque suas portas de conexão (normalmente, a porta 80) já estão sendo utilizado por outra aplicação.

    Isso geralmente acontece quando o Skype é usado. Para parar impedir o Skype de parar o seu servidor web local, vá para as configurações avançadas do Skype (Ferramentas> Opções> Avançado> Conexões) e desmarque a opção "Usar a porta 80 e 443 como alternativas". Reinicie o Skype, e reinicie o seu servidor web local novamente.
* **O servidor de banco de dados deve estar instalado e funcionando**. O MySQL é o lugar onde todos os dados do PrestaShop são armazenados. O pacote AMP deve fornecê-lo com um indicador claro se o MySQL está funcionando ou não.
* **A ferramenta phpMyAdmin deve ser acessível.** Esta é a aplicação web que lhe ajuda a lidar com os dados armazenados no MySQL. A sua localização depende do pacote AMP que você escolheu: ele pode ser encontrado em [http://127.0.0.1/phpmyadmin](http://127.0.0.1/phpmyadmin) (XAMPP, WampServer, MAMP), [http://127.0.0.1/mysql](http://127.0.0.1/mysql) (EasyPHP), ou talvez em outro local . Verifique a documentação do seu pacote - que poderá até mesmo fornecer um botão phpMyAdmin do tipo que iria abrir a URL correta no seu browser.

## Encontrando o diretório raiz no servidor local <a href="#instalandooprestashopemseucomputador-encontrandoodiretorioraiznoservidorlocal" id="instalandooprestashopemseucomputador-encontrandoodiretorioraiznoservidorlocal"></a>

Depois de ter verificado que o pacote está instalado corretamente e que todas as suas partes estão em execução, você precisa encontrar a pasta raiz do seu servidor web local.

Essa é a pasta local onde você vai colocar arquivos de sua aplicação, e pode ser comparada com a pasta raiz do seu servidor on-line, o seu conteúdo é apenas acessado com [http://127.0.0.1](http://127.0.0.1).

A localização local real da pasta depende grandemente do pacote AMP, e pode ser personalizado:

* EasyPHP: `C:\easyphp\www`
* MAMP: `/Applications/MAMP/htdocs/`
* WampServer: `C:\wamp\www`
* XAMPP: `C:\xampp\htdocs` or `/Applications/xampp/htdocs`

## Encontrando as informações de usuário do MySQL <a href="#instalandooprestashopemseucomputador-encontrandoasinformacoesdeusuariodomysql" id="instalandooprestashopemseucomputador-encontrandoasinformacoesdeusuariodomysql"></a>

Finalmente, você precisa saber o nome de usuário e senha de administração para o MySQL, a fim de instalar o PrestaShop.

**A maioria dos pacotes usar o nome de usuário "root" com uma senha em branco**, incluindo EasyPHP, WAMP, Wamp Server e XAMPP.

Leia a documentação do pacote.

## Observações finais antes do tutorial de instalação <a href="#instalandooprestashopemseucomputador-observacoesfinaisantesdotutorialdeinstalacao" id="instalandooprestashopemseucomputador-observacoesfinaisantesdotutorialdeinstalacao"></a>

Com tudo esclarecido e feito, você pode acompanhar o resto deste guia de introdução e começar a instalar PrestaShop.

Quando você instalar o PrestaShop localmente, tenha em mente que:

* Os arquivos não são para serem enviados através de um software FTP (como o Filezilla) para um servidor web: basta movê-los na pasta local correto, como indicado acima.
* Você não tem que criar um nome de domínio local: O PrestaShop está disponível através do endereço de loopback indicado acima, que é http: // localhost ou [http://127.0.0.1](http://127.0.0.1). - se o PrestaShop está disponível neste endereço adicionando o nome da sua pasta, por exemplo [http://localhost/prestashop](http://localhost/prestashop) ou [http://127.0.0.1/prestashop](http://127.0.0.1/prestashop) se o PrestaShop está no /prestashop / subpasta da pasta raiz local. Ao entrar neste endereço, pela primeira vez, você deve ser redirecionado automaticamente para o instalador prestashop, em [http://localhost/prestashop/](http://localhost/prestashop/install)[install](http://localhost/prestashop/install) ou [http://127.0.0.1/prestashop/install](http://127.0.0.1/prestashop/install).

Você já leu tudo? Agora siga o guia de instalação, acessando diretamente a opção "Criando o banco de dados da sua loja" da seção: "Instalando o PrestaShop".
