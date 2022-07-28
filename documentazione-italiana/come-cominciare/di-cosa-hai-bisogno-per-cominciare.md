# Di cosa hai bisogno per cominciare

**Table of contents**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597225799646 {padding: 0px;}\
div.rbtoc1597225799646 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597225799646 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Di cosa hai bisogno per cominciare](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Dicosahaibisognopercominciare)
  * [Istruzioni per un set-up veloce](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Istruzioniperunset-upveloce)
  * [Istruzioni dettagliate per il set-up](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Istruzionidettagliateperilset-up)
    * [Registrare un nome a dominio](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Registrareunnomeadominio)
    * [Trovare un host](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Trovareunhost)
    * [Requisiti tecnici](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Requisititecnici)
    * [Strumenti](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Strumenti)
    * [Fai un piano](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-Faiunpiano)
    * [Installazione di PrestaShop](di-cosa-hai-bisogno-per-cominciare.md#Dicosahaibisognopercominciare-InstallazionediPrestaShop)

## Di cosa hai bisogno per cominciare <a href="#dicosahaibisognopercominciare-dicosahaibisognopercominciare" id="dicosahaibisognopercominciare-dicosahaibisognopercominciare"></a>

### Istruzioni per un set-up veloce <a href="#dicosahaibisognopercominciare-istruzioniperunset-upveloce" id="dicosahaibisognopercominciare-istruzioniperunset-upveloce"></a>

Ecco una veloce lista di cose che necessiti per cominciare ad installare PrestaShop 1.6. In caso non ti sentissi a tuo agio per la mancanza di dettagli troverai le istruzioni dettagliate nelle sezioni successive.

* Requisiti di Sistema:
  * PHP 5.2 or successivo.
    * impostazioni utili: `allow_url_fopen` settato su On, `register_globals` settato su Off, `magic_quotes_*` settato su Off, `safe_mode` settato su Off (tutto nel file `php.ini`), `file_max_upload_size` settato su "16M".
    * Utili estensioni di PHP: PDO\_MySQL, cURL, SimpleXML, mcrypt, GD, OpenSSL, DOM, SOAP (tutto nel file `php.ini` file).
    * Utili strumenti del server: cron/crontab, Memcached.
  * MySQL 5.0 or successivo.
  * Meglio se:\

    * Unix/Linux hosting.
    * Apache Web Server 1.3 or successivo or nginx Web Server.
      * Impostazioni del modulo Apache: `mod_rewrite` enabled, `mod_security` disabled, `mod_auth_basic` disabled.
    * Almeno 64 Mb of RAM dedicati al PHP.
* Codici di accesso al tuo server FTP, al tuo database MySQL e\

  * Questi dati ti dovrebbero essere forniti dal tuo web-host se non stai facendo un'installazione locale.
* Qualsiasi editor di testo.
* Qualsiasi client FTP.
* Qualsiasi moderno Web browser (se usi Internet Explorer: almeno che sia IE8).

Hai anche bisogno di conoscere da quale/i URL vuoi che il tuo/tuoi store siano accessibili.

Controlla la pagina ufficiale dei requisiti di sistema: [http://www.prestashop.com/it/requisiti-di-sistema](http://www.prestashop.com/it/requisiti-di-sistema).

Una volta che il set-up è a posto, è possibile passare alla guida di installazione: [http://doc.prestashop.com/display/PS16/Installazione+di+Prestashop](http://doc.prestashop.com/display/PS16/Installazione+di+Prestashop).

### Istruzioni dettagliate per il set-up <a href="#dicosahaibisognopercominciare-istruzionidettagliateperilset-up" id="dicosahaibisognopercominciare-istruzionidettagliateperilset-up"></a>

PrestaShop è una applicazione web: necessita di essere installata su un web server per girare, e ha bisogno di un nome a dominio che i tuoi visitatori utilizzeranno per accedere al tuo store.

#### Registrare un nome a dominio <a href="#dicosahaibisognopercominciare-registrareunnomeadominio" id="dicosahaibisognopercominciare-registrareunnomeadominio"></a>

Prima di scaricare o installare nulla, è necessario fornire una locazione per il tuo negozio online PrestaShop. Che è fatta di due componenti: un nome a dominio e un server web. Un dominio è l'identificatore online per il tuo sito web, come `example.com` o `myonlineshop.net` . E 'il volto pubblico del vostro server web, e quindi del tuo negozio.

È necessario acquistare un nome di dominio per il tuo negozio. Potresti essere in grado di ottenerne uno, mentre stai acquistando un web hosting: molti venditori di hosting web offrono un dominio gratuito con ogni nuovo account. Potrebbe essere gratuito per un anno, o per tutto il tempo che rimani cliente di tale venditore di hosting web. Questo rende più facile ottenere il pacchetto completo (hosting + dominio) in un colpo solo.

Ci potrebbe essere un problema con i nomi di dominio forniti dal tuo fornitore di hosting: se vi trovate insoddisfatti del servizio del fornitore di hosting, e volete passare a un fornitore migliore. Sarete costretti a spostare i file, dati e nome di dominio presso un altro fornitore di hosting.

I file e i dati sono facili da spostare, ma a seconda del fornitore di hosting, potrebbe essere necessario molto tempo per avere l'abilitazione al trasferimento del vostro dominio. Dal momento che hanno comprato il nome del dominio per voi, tecnicamente il dominio appartiene a loro, e possono sia vietare di trasferire presso un altro host, oppure possono farvi pagare per questo. E dal momento che il nome di dominio è il tuo marchio e il tuo indirizzo sul web, è necessario rispettare le regole del web host.

Questo è il motivo per cui è spesso raccomandato di comprare il vostro nome a dominio da un registrar di nome a dominio indipendente (vedi:[http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://translate.googleusercontent.com/translate\_c?depth=1\&hl=it\&rurl=translate.google.it\&sl=en\&tl=it\&u=http://en.wikipedia.org/wiki/Domain\_name\_registrar\&usg=ALkJrhghab9u4zij86Zr4qUkXjwjZDn8Ag)). Tecnicamente, non si può mai comprare un nome di dominio, si può solo affittare, il più delle volte pagando un canone annuale. Questo ti dà il diritto di usare quel nome a dominio, ma non appena smetti di pagare per esso, non è più tuo e chiunque lo può prendere per se stesso. Così, pagherai per la registrazione del nome a dominio in aggiunta al tuo web hosting, ma almeno sarai libero di muoverti verso un miglior fornitore di hosting in qualsiasi momento, senza alcun costo aggiuntivo: basta cambiare gli indirizzi DNS del nome a dominio, ed entro 24 ora l'operazione sarà propagata a tutti i server DNS del mondo.

Se invece volete ottenere il vostro nome a dominio da un registrar indipendente, qui ci sono alcuni fornitori di cui vi potete fidare:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* PairNIC: [https://www.pairnic.com/](https://www.pairnic.com/)

Ce ne sono molti altri. Chiedete ai vostri amici!

#### Trovare un host <a href="#dicosahaibisognopercominciare-trovareunhost" id="dicosahaibisognopercominciare-trovareunhost"></a>

Ora che si dispone di un nome di dominio, è necessario disporre di esso per posizionarci PrestaShop. Ciò significa che i file PrestaShop devono risiedere su un server web. Potresti avere un server web di tua proprietà, ma è più probabile che hai o avrai il tuo negozio ospitato da un servizio Internet di hosting (vedi: [http://it.wikipedia.org/wiki/Hosting](http://it.wikipedia.org/wiki/Hosting) ), che fornisce servizio di hosting pagando un canone mensile o annuale.

Se non avete mai avuto un host web, qui ci sono alcuni fornitori dei quali ci si può fidare:

* InMotion Hosting: [http://www.inmotionhosting.com/](https://secure1.inmotionhosting.com/cgi-bin/gby/clickthru.cgi?id=prestashop\&campaign=endocumentation\&page=336)
* OVH France: [http://www.ovh.com/](http://www.ovh.com/fr/web/prestashop/)
* OVH UK: [http://www.ovh.co.uk/](http://www.ovh.co.uk/items/modules/ecommerce/prestashop.xml)

Scopri i [nostri partner di hosting](http://www.prestashop.com/en/ecommerce-hosting)!

Al momento di scegliere il tuo host, ricordati un requisito fondamentale: deve fornire il supporto per PHP 5.2 (o più recente), il linguaggio di programmazione con cui PrestaShop è scritto, e MySQL 5 (o più recente) il sistema di database in cui memorizza PrestaShop tutti suoi dati. Ci sono altri requisiti: vedi la sezione "Requisiti tecnici" qui sotto.

PrestaBox

PrestaShop può ospitare il tuo business online sui propri server web in-house: il nostro servizio PrestaBox è stato costruito in modo da liberare i venditori da vari problemi tecnici, come l'installazione o l'aggiornamento di PrestaShop.

Si prega di consultare il nostro sito PrestaBox per i dettagli sul nostro conveniente e sicuro servizio di hosting. Questo è altamente raccomandato per le aziende con poca o nessuna esperienza con Internet o computer.

È possibile raggiungere PrestaBox a questo indirizzo: [http://www.prestabox.com/](http://translate.googleusercontent.com/translate\_c?act=url\&depth=1\&hl=it\&ie=UTF8\&prev=\_t\&rurl=translate.google.it\&sl=en\&tl=it\&u=http://www.prestabox.com/\&usg=ALkJrhgdyZJmcEeZkBwuYp6ACmJPPBvqOg)

#### Requisiti tecnici <a href="#dicosahaibisognopercominciare-requisititecnici" id="dicosahaibisognopercominciare-requisititecnici"></a>

PrestaShop è un'applicazione che gira su un server web, ed è scritto utilizzando il linguaggio di programmazione PHP. Memorizza i propri dati in un server MySQL.

PHP è un linguaggio di programmazione open source, utilizzato principalmente per le applicazioni web. Creata nel 1995, da allora è diventato il linguaggio di programmazione più utilizzato dagli sviluppatori web. Esso utilizza una sintassi simile al linguaggio C, rendendo più facile per gli sviluppatori l'apprendimento.

MySQL è un database management system open-source. Creato Sempre nel 1995, da allora è diventato il sistema di database più utilizzato dagli sviluppatori web. Si basa sul linguaggio SQL, il linguaggio del database più utilizzato.

Qualunque sia il servizio di hosting che sceglierai, deve avere i seguenti componenti installati sul server web:

* **Sistema**: Unix, Linux o Windows. Unix è altamente raccomandato.
* **Web server**: Apache Web server 1.3 o successivo.
* **PHP 5.2 o successivo**. Potrebbe essere necessario attivare PHP 5 (chiedi al tuo fornitore di hosting).
* **MySQL 5.0 o successivo**.
* Almeno 64 Mb of RAM sul tuo server (128 Mb sarebbe meglio, più ce n'è meglio è).

PrestaShop può funzionare anche con server Web Microsoft IIS 6.0 o versione successiva e nginx 1.0 o versione successiva.

Ulteriori informazioni sono disponibili agli amministratori di sistema in [Linux System Administration Guide](http://translate.googleusercontent.com/translate\_c?act=url\&depth=1\&hl=it\&ie=UTF8\&prev=\_t\&rurl=translate.google.it\&sl=en\&tl=it\&u=http://doc.prestashop.com/display/PS15/System%2BAdministrator%2BGuide\&usg=ALkJrhjgOumuiGJ\_Ru3WVl2efc3qSmfm3g) . Assicurati di leggerla!

#### Strumenti <a href="#dicosahaibisognopercominciare-strumenti" id="dicosahaibisognopercominciare-strumenti"></a>

Avrete bisogno di due strumenti: un editor di testo, al fine di modificare i file di testo, e un client FTP, al fine di trasferire i file dal vostro computer al server e viceversa.

**Editor di testo**

Qui ci sono alcuni editor di testo molto utilizzati dai programmatori:

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

NON usare un word processor durante la modifica di file di testo, come ad esempio Microsoft Word o OpenOffice.org Write.

**Client FTP**

FTP è l'acronimo di "File Transfer Protocol", cioè il metodo standard utilizzato per trasferire file da un computer a un web-host.

In questa guida, useremo Filezilla, che è un ottimo e gratuito client FTP per Windows, Mac OS X e Linux. Scaricalo da [http://filezilla-project.org/](http://translate.googleusercontent.com/translate\_c?act=url\&depth=1\&hl=it\&ie=UTF8\&prev=\_t\&rurl=translate.google.it\&sl=en\&tl=it\&u=http://filezilla-project.org/\&usg=ALkJrhgLOY-zxO5A3yOJNw8Um9dssH73FQ) e avvia l'installer. Nota: non scaricare FileZilla Server, solo FileZilla client!

Una volta che FileZilla è installato, sarà necessario configurarlo con i parametri di connessione per il server web, che vi avrebbe dovuto mandare il vostro fornitore di hosting. In caso contrario, chiedere al vostro fornitore di hosting- o controlla la cartella spam.

Fondamentalmente, i parametri necessari sono:

* **un hostname** o **un indirizzo IP:** la posizione del server FTP del vostro spazio di hosting.
* **un username**: l'identificatore account di hosting, che è univoco.
* **una password**: misura di sicurezza obbligatoria.

Aprire FileZilla, e aprire il suo strumento Site Manager. È possibile farlo in tre modi diversi:

* Premendo Ctrl-S,
* Facendo clic sull'icona "Apri l'Amministratore del Sito", in alto a sinistra,
* Aprendo il menu "File" e selezionando l'opzione "Site Manager ...".

Si aprirà una finestra.

Per aggiungere il tuo spazio di hosting al Site Manager:

1. Clicca sul bottone "Nuovo sito". Una nuova voce sarà creata nella lista dei siti. Assegnagli un nome riconoscibile.
2. Sul lato destro, nella scheda "Generale",Inserisci i parametri che il tuo fornitore di host ti ha dato: host, user, e password. Non dovresti aver bisogno di cambiare gli altri parametri di default, a meno che a dirtelo non sia il tuo fornitore di hosting.
3. Una volta che hai correttamente inserito tutti i parametri, clicca il tasto "Connetti". Facendo questo il tuo sitò sarà salvato nella lista e contemporaneamente avrai accesso al tuo account, in questo modo potrai verificare se la connessione avviene correttamente.

Se FileZilla non fa per te, qui ci sono altri client FTP molto conosciuti:

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

#### Fai un piano <a href="#dicosahaibisognopercominciare-faiunpiano" id="dicosahaibisognopercominciare-faiunpiano"></a>

Si dovrebbe decidere subito dove si desidera ospitare PrestaShop. Ci sono quattro possibilità relative al tuo nome di dominio::

* Nella radice del dominio: [http://www.example.com/](http://www.example.com/)
* In una cartella: [http://www.example.com/shop/](http://www.example.com/shop/)
* In un sottodominio: [http://store.example.com/](http://store.example.com/)
* In una cartella di un sottodominio: [http://clothes.example.com/boutique/](http://clothes.example.com/boutique/)

Si noti che, grazie alla funzione multistore, puoi avere molti negozi, se necessario con una singola installazione di PrestaShop 1.6, ciascuna con un proprio nome di dominio specifico, se necessario. Ne dovresti tenere conto al momento di decidere dove posizionarlo. \
Qualunque sia il vostro piano, il negozio di default risiederà sempre nel luogo in cui hai posizionato PrestaShop.

#### Installazione di PrestaShop <a href="#dicosahaibisognopercominciare-installazionediprestashop" id="dicosahaibisognopercominciare-installazionediprestashop"></a>

Finalmente, ora che tutti i requisiti sono a posto, è possibile utilizzare la guida di installazione: [http://doc.prestashop.com/display/PS16/Installazione+di+Prestashop](installazione-di-prestashop.md).
