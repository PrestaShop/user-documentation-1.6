# Sovrascrittura del comportamento di default

## [Sovrascrittura del comportamento di default](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Sovrascritturadelcomportamentodidefault)[Override di classi e controllori di PrestaShop](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-OverridediclassiecontrolloridiPrestaShop)[Override di una classe](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Overridediunaclasse)[Overriding di controller](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Overridingdicontroller)[Override altri comportamenti](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Overridealtricomportamenti)[Override comportamento di un modulo](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Overridecomportamentodiunmodulo)[Manipolare il codice override manuale](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Manipolareilcodiceoverridemanuale)[Codice di esempio](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Codicediesempio)[Example 1](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Example1)[Example 2](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Example2)[Example 3](sovrascrittura-del-comportamento-di-default.md#Sovrascritturadelcomportamentodidefault-Example3) <a href="#sovrascritturadelcomportamentodidefault-less-than-cdata-div.rbtoc1597225808978-padding-0px-div.rbtoc" id="sovrascritturadelcomportamentodidefault-less-than-cdata-div.rbtoc1597225808978-padding-0px-div.rbtoc"></a>

## Sovrascrittura del comportamento di default <a href="#sovrascritturadelcomportamentodidefault-sovrascritturadelcomportamentodidefault" id="sovrascritturadelcomportamentodidefault-sovrascritturadelcomportamentodidefault"></a>

PrestaShop permette di sostituire i vari componenti e comportamenti predefiniti. Questo sistema è costituito da due punti principali:

1. Sovrascrittura comportamento di PrestaShop (file di classe e file di controller) al fine di indirizzare una sezione specifica dei componenti necessari.&#x20;
2. Sovrascrittura delle parti visibili dei moduli (Modelli, JavaScript, linguaggio di fogli di stile ...) in modo che i temi possono adattarsi meglio.

### Override di classi e controllori di PrestaShop <a href="#sovrascritturadelcomportamentodidefault-overridediclassiecontrolloridiprestashop" id="sovrascritturadelcomportamentodidefault-overridediclassiecontrolloridiprestashop"></a>

La Sovrascrittura (o Overriding) è un modo per "sovrascrivere" i file di classe e i file del controller. Prestashop utilizza un sistema ingegnoso per auto caricare le classi di sistema ed effettua lo switch alle classi sovrascritte in maniera semplice. Grazie al codice object-oriented di PrestaShop, si può contare sull'ereditarietà di un oggetto per modificare e aggiungere nuovi comportamenti, utilizzando le proprietà e i metodi delle varie classi esistenti genitore.

Classi e controllori di solito sono costruiti seguendo uno standard. Ecco la classe del prodotto e il relativo controller:

* `/classes/Product.php`\
  Questa classe sarebbe chiamata ProductCore.
* `/controllers/front/ProductController.php`\
  Questo controller sarebbe chiamata ProductControllerCore.

E' necessario creare un file PHP e posizionarlo sia delle cartelle di override, a seconda che questo file faccia parte di un modulo, o distribuito così com'è. Infatti, dalla versione 1.5 di PrestaShop, ci sono due luoghi in cui è possibile inserire i file di di Overriding: o nella root di PrestaShop , o all'interno di un modulo.

#### Override di una classe <a href="#sovrascritturadelcomportamentodidefault-overridediunaclasse" id="sovrascritturadelcomportamentodidefault-overridediunaclasse"></a>

Per Sovrascrivere la classe del prodotto, il file deve essere chiamato Product.php e deve avere una classe di prodotto che poi estende la classe ProductCore.

Il file può essere inserito in una di queste posizioni:

* `/override/classes/Product.php`
* `/modules/my_module/override/classes/Product.php`

#### Overriding di controller <a href="#sovrascritturadelcomportamentodidefault-overridingdicontroller" id="sovrascritturadelcomportamentodidefault-overridingdicontroller"></a>

Per sostituire la classe ProductController, il file deve essere chiamato ProductController.php e deve avere una classe ProductController che poi estende la classe ProductControllerCore.

Il file può essere inserito in una di queste posizioni:

* `/override/controllers/front/ProductController.php`
* `/modules/my_module/override/controllers/front/ProductController.php`

#### Override altri comportamenti <a href="#sovrascritturadelcomportamentodidefault-overridealtricomportamenti" id="sovrascritturadelcomportamentodidefault-overridealtricomportamenti"></a>

PrestaShop ha alcuni file che è possibile utilizzare per sostituire elementi come la visualizzazione di reindirizzamento (Tools.php) e l'hook per la misurazione del tempo di esecuzione  (\_Module.php), ecc è possibile abilitare rimuovendo il "\_" prefisso. Ad esempio, rinominare \_Tools.php in Tools.php. Se esiste già un overriding di Tools.php, deve essere inglobato con il vostro.

### Override comportamento di un modulo <a href="#sovrascritturadelcomportamentodidefault-overridecomportamentodiunmodulo" id="sovrascritturadelcomportamentodidefault-overridecomportamentodiunmodulo"></a>

I moduli sono in genere nel seguente formato:

* `/modules/my_module/my_module.tpl`
* `/modules/my_module/my_module.css`
* `/modules/my_module/my_module.js`

Da PrestaShop 1.5, essi possono e **devono** anche essere nel seguente formato:

* `/modules/my_module/views/templates/front/my_module.tpl`
* `/modules/my_module/views/templates/front/my_module.css`
* `/modules/my_module/views/templates/front/my_module.js`

PrestaShop consente di sovrascrivere o sostituire alcuni file di moduli front-office con quelli nuovi all'interno dello stesso tema. L'override è governato dal tema: una volta contiene una cartella /modules (! O più), PrestaShop si visualizza il suo contenuto per i file che hanno lo stesso nome e il percorso di quelli dei moduli esistenti e sostituirli con quelli nuovi.

Questo significa che, per PrestaShop moduli 1.4 compatibili:

* `/themes/my_theme/modules/my_module/my_module.tpl`
* `/themes/my_theme/css/modules/my_module/my_module.css`
* `/themes/my_theme/js/modules/my_module/my_module.js`

Da PrestaShop 1.5, il percorso è leggermente più lungo

* `/themes/my_theme/modules/my_module/views/templates/front/my_module.tpl`
* `/themes/my_theme/css/modules/my_module/views/templates/front/my_module.css`
* `/themes/my_theme/js/modules/my_module/views/templates/front/my_module.js`

In generale, il percorso corretto per ignorare un file. Tpl,. File css js o. Dipende proprio percorso del modulo. Questo è il motivo per cui se PrestaShop deve lavorare con un modulo senza una cartella vista, sarà necessario lo stesso percorso override.\
In breve, è possibile mantenere il codice prevalente alla 1.6 come avete fatto in 1.4.

I nuovi file verranno utilizzati quando il cliente carica il negozio.

Contrary to the override code that is to be placed manually in the `/override` folder, module overrides are enabled as soon as the module is installed. During installation, overriding code is merge with those already in place (if any), otherwise they are copied to the `/override` folder at the root of the PrestaShop folder.

### Manipolare il codice override manuale <a href="#sovrascritturadelcomportamentodidefault-manipolareilcodiceoverridemanuale" id="sovrascritturadelcomportamentodidefault-manipolareilcodiceoverridemanuale"></a>

Moduli e temi possono aggiungere una sostituzione per un comportamento di default, e PrestaShop si occupa di resettare il file /cache/class\_index.php.

Ma a volte è necessario aggiungere che il codice prevalente te, caricando manualmente il file sul server. In tal caso, è necessario attivare la rigenerazione del /cache/class\_index.php presentare te stesso. Questo viene fatto semplicemente cancellando il file: se PrestaShop non riesce a trovare il file, verrà rigenerarlo, prendendo tutte le sostituzioni in considerazione.

E 'lo stesso quando si rimuove manualmente una sostituzione: al fine di ripristinare il comportamento predefinito, è necessario eliminare il file /cache/class\_index.php.

### Codice di esempio <a href="#sovrascritturadelcomportamentodidefault-codicediesempio" id="sovrascritturadelcomportamentodidefault-codicediesempio"></a>

#### Example 1 <a href="#sovrascritturadelcomportamentodidefault-example1" id="sovrascritturadelcomportamentodidefault-example1"></a>

Uso della classe di dati MySQL.php è semplicemente impossibile durante il tentativo di inserire i dati in un database diverso da PrestaShop del sullo stesso server MySQL. (Davvero!)

La soluzione è quella di utilizzare il seguente override della classe MySQLCore:

```
<?php
class MySQL extends MySQLCore
{
	public function __construct($server, $user, $password, $database, $newlink = false)
	{
		$this->_server = $server;
		$this->_user = $user;
		$this->_password = $password;
		$this->_type = _DB_TYPE_;
		$this->_database = $database;

		$this->connect($newlink);
	}
	
	public function connect($newlink = false)
	{
		if (!defined('_PS_DEBUG_SQL_'))
			define('_PS_DEBUG_SQL_', false);

		if ($this->_link = mysql_connect($this->_server, $this->_user, $this->_password, $newlink) )
		{
			if (!$this->set_db($this->_database))
				die(Tools::displayError('The database selection cannot be made.'));
		}
		else
			die(Tools::displayError('Link to database cannot be established.'));

		/* UTF-8 support */
		if (!mysql_query('SET NAMES \'utf8\'', $this->_link))
			die(Tools::displayError('PrestaShop Fatal error: no utf-8 support. Please check your server configuration.'));
		return $this->_link;
	}
}
?>
```

Per utilizzarlo è necessario creare un'istanza della classe come segue:

* Per la connessione locale: `new MySQL(`_`DB_SERVER`_`,`` `_`DB_USER`_`,`` `_`DB_PASSWD`_`, 'DB_name', true);`
* Per la connessione remota: `new MySQL(`_`DB_SERVER`_`,`` `_`DB_USER`_`,`` `_`DB_PASSWD`_`, 'DB_name', true);`

L'ultimo parametro forza la creazione di una connessione MySQL.

#### Example 2 <a href="#sovrascritturadelcomportamentodidefault-example2" id="sovrascritturadelcomportamentodidefault-example2"></a>

```
/*
 * Creare un'attività periodica per fare il backup del database
*/
class AdminTab extends AdminTabCore{
	public function ajaxProcess()
	{			 
		// Qui noi chiamiamo la stessa cosa come se abbiamo fatto alla vecchia maniera 
		// + Con "se": forse vogliamo limitare l'utilizzo di solo il backup aggiungendo 
		// Nota: trovare te stesso un modo per ottenere il link del file se si desidera inviare per posta!
		if (isset($_REQUEST['addbackup']))
			return $this->postProcess();
	} 

	public function displayAjax()
	{
		if (sizeof($this->_errors) > 0)
		{
			// errori 
			// per esempio, invia una mail con tutti i messaggi di errore
			$content = '';
			foreach($this->_errors as $errorMsg)
			 $content .= $errorMsg;

			 $lang = Configuration::get('PS_LANG_DEFAULT');
			// Qui inviamo una e-mail di dare il risultato del processo di 
			// Avviso: è necessario creare file mails template
			 Mail::Send($lang, 'backuptaskdone', '[autobackup] report backup error', array('backup_link'=>)), $to); 
		}
		else
		{
			// nessun errore, ma forse vogliamo una e-mail?
			if(Configuration::get('PS_NOTICE_SUCCEED_BACKUP')) 
			{
				// fileAttachment disponibile, guarda il nono parametro del metodo Send() in classes/Mail.php
				// + possiamo aggiungere una condizione "if (Configuration::get('PS_AUTOBACKUP_SEND_FILE'))"
				Mail::Send($lang, 'backuptaskerror', '[autobackup] report backup error', array('vars to use in tpl'), $to); 
			}
		}
	return true;
	}
}
```

```
/*
 * Questo override ti permette di utilizzare ajax-tab.php per effettuare ogni azione in admin
 * Usarlo per esempio con il crontask for example
*/
class AdminTab extends AdminTabCore {
	public function ajaxProcess()
	{
		return $this->postProcess();
	}
}
```

#### Example 3 <a href="#sovrascritturadelcomportamentodidefault-example3" id="sovrascritturadelcomportamentodidefault-example3"></a>

```
/*
 * Con questo override, ha una nuova variabile Smarty chiamata "currentController" disponibile in header.tpl
 * Ciò ti permette di utilizzar un differente header se se nella pagina del prodotto, nella pagina categoria o nella home
 */
class FrontController extends FrontControllerCore {
	public function initHeader()
	{
		self::$smarty->assign('currentController', get_class($this));
		return parent::initHeader();
	}
}
```
