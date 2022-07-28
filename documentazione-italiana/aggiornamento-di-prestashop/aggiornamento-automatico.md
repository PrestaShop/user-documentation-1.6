# Aggiornamento automatico

**Table of contents**

/\*\<!\[CDATA\[\*/\
div.rbtoc1597225800941 {padding: 0px;}\
div.rbtoc1597225800941 ul {list-style: disc;margin-left: 0px;}\
div.rbtoc1597225800941 li {margin-left: 0px;padding-left: 0px;}\
\
/\*]]>\*/

* [Aggiornamento automatico](aggiornamento-automatico.md#Aggiornamentoautomatico-Aggiornamentoautomatico)
* [Scaricamento e installazione del modulo 1-Click Upgrade](aggiornamento-automatico.md#Aggiornamentoautomatico-Scaricamentoeinstallazionedelmodulo1-ClickUpgrade)
* [La schermata di configurazione](aggiornamento-automatico.md#Aggiornamentoautomatico-Laschermatadiconfigurazione)
  * [Benvenuto](aggiornamento-automatico.md#Aggiornamentoautomatico-Benvenuto)
* [La lista di controllo pre-aggiornamento](aggiornamento-automatico.md#Aggiornamentoautomatico-Lalistadicontrollopre-aggiornamento)
* [Inizia la tua Aggiornamento](aggiornamento-automatico.md#Aggiornamentoautomatico-InizialatuaAggiornamento)
* [Modalità esperto](aggiornamento-automatico.md#Aggiornamentoautomatico-Modalitàesperto)

## Aggiornamento automatico <a href="#aggiornamentoautomatico-aggiornamentoautomatico" id="aggiornamentoautomatico-aggiornamentoautomatico"></a>

Lo strumento di aggiornamento automatico di PrestaShop permette ai proprietari di negozi di eseguire il backup e aggiornare il loro sito in pochi click e nessuna conoscenza tecnica.

Il modulo 1-Click Upgrade dovrebbe essere disponibile per impostazione predefinita nella pagina "Moduli" (nella categoria "Amministrazione"): basta cliccare sul relativo pulsante Installa, e lo si può utilizzare per eseguire l'aggiornamento alla versione più recente di PrestaShop.

Attenzione

Non si dovrebbe mai aggiornare il proprio negozio on-line subito. Lo strumento di aggiornamento automatico può fallire in alcune situazioni, e si potrebbe non essere in grado di ripristinare la versione precedente.

Il modo più sicuro è quello di avere una copia esatta del tuo negozio disponibile, sia sul computer locale o in un'altra cartella del vostro web server. Dovrebbe contenere tutti i vostri prodotti, le categorie, i temi, moduli, traduzioni, impostazioni, ecc

Fare un aggiornamento di prova su quella copia del vostro negozio. Una volta che l'aggiornamento è fatto, testare a fondo il vostro front office e back per assicurarsi che tutto è come previsto. In caso contrario, lo strumento di aggiornamento ha un problema con la configurazione, e si dovrebbe utilizzare il metodo di aggiornamento manuale, che ora è deprecato e richiede più tempo, ma che può aiutare nella vostra situazione.

## Scaricamento e installazione del modulo 1-Click Upgrade <a href="#aggiornamentoautomatico-scaricamentoeinstallazionedelmodulo1-clickupgrade" id="aggiornamentoautomatico-scaricamentoeinstallazionedelmodulo1-clickupgrade"></a>

Se il modulo 1-Click Upgrade non è disponibile nell'installazione di PrestaShop 1.4 o 1.5, è possibile scaricarlo gratuitamente dal sito Addons.

Trucco

Anche se avete già installato il modulo "1-Click upgrade", assicurarsi che si sta utilizzando la versione più recente:

* PrestaShop 1.4: Controllare il numero di versione nella scheda "Moduli", poi confrontarla con il numero di versione elencati sul sito web Addons (vedi sotto). Se i numeri sono diversi, scaricare e aggiornare.
  * Per aggiornare il modulo: disinstallarlo ed eliminarlo dall'amministrazione PrestaShop, quindi copiare la cartella "/autoupgrade" dall'archivio del modulo (che è stato scaricato dal sito web Addons) nella cartella "/modules" della vostra installazione di PrestaShop. Infine, installare il modulo da parte dell'amministrazione.
* PrestaShop 1.5 e versioni successive: PrestaShop controllerà automaticamente il sito di Addons per nuove versioni dei moduli. Se una nuova versione è disponibile, essa presenterà il pulsante "Aggiorna" accanto al pulsante "Installa / Disinstalla". Clicca perchè PrestaShop scarichi e aggiorni il modulo per te.

Semplicemente segui la normale procedura di installazione di un modulo su PrestaShop:

1. Scarica il modulo 1-Click Upgrade da PrestaShop Addons: [http://addons.prestashop.com/en/administration-tools/5496-autoupgrade.html](http://addons.prestashop.com/en/administration-tools/5496-autoupgrade.html). Salva il file zip sul desktop.
2. Nel tuo pannello di amministrazione PrestaShop, vai sulla pagina "Moduli" del menu "Moduli".
3.  Fai clic sul pulsante "Aggiungi un modulo", che si trova in alto a destra della lista dei moduli disponibili.

    Trucco

    Se l'aggiornamento dalla versione 1.4, fare clic sul link "Aggiungi un modulo dal mio computer", che si trova in alto a sinistra.
4. Nel modulo che si apre, fare clic sul pulsante "Sfoglia ...", quindi individuare e selezionare il file zip del modulo che avete appena scaricato.
5. Fai clic sul pulsante "Carica questo modulo". PrestaShop caricherà il modulo sul server, decomprimerlo, e posizionando i file nella cartella /modules.

Il modulo è ora disponibile nella vostra lista di moduli, ma si deve ancora installare:

1. Nella scheda "Moduli", trovare il modulo 1-Click upgrade: scrivi "1-click upgrade" o "Upgrade automatico" nella casella di ricerca del modulo (non la ricerca globale in alto). Un collegamento diretto al modulo dovrebbe apparire durante la digitazione. Fare clic su di esso.
2. PrestaShop quindi visualizza il modulo nella lista modulo principale.
3. Fai clic sul pulsante "Install" del modulo.

Il modulo è pronto per la configurazione ed essere utilizzato.

## La schermata di configurazione <a href="#aggiornamentoautomatico-laschermatadiconfigurazione" id="aggiornamentoautomatico-laschermatadiconfigurazione"></a>

Schermata di configurazione del modulo è disponibile sotto la lista "Moduli", cliccando sul link "Configura" del modulo.

Trucco

La schermata di configurazione è anche disponibile da:

* PrestaShop 1.4: nella scheda "Strumenti", nel "1-Click Upgrade" scheda secondaria.
* PrestaShop 1.5 e versioni successive: sotto i "parametri avanzati", nella pagina "1-Click Upgrade".

La schermata di configurazione si presenta con una serie di sezioni, fornendo informazioni, strumenti e le impostazioni.

### Benvenuto <a href="#aggiornamentoautomatico-benvenuto" id="aggiornamentoautomatico-benvenuto"></a>

Questa piccola sezione serve a ricordare che un aggiornamento non è mai sicuro al 100%, e che quindi è necessario assicurarsi di aver effettuato un backup completo dei file e dei dati. In questo modo, qualora l'aggiornamento non riuscire, si sarà in grado di ritornare allo stato iniziale del negozio - anche se con un po' di lavoro di lavoro in più.

Questo processo è spiegato in dettaglio nel capitolo "Eseguire e ripristinare un backup" di questa guida: [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).

![](<../../.gitbook/assets/23038081 (3).png>)Si noti che il modulo 1-Click upgrade esegue una propria serie di attività, al fine di consentire il ripristino dopo un errore. Tuttavia, si dovrebbe fare affidamento sul proprio backup.

## La lista di controllo pre-aggiornamento <a href="#aggiornamentoautomatico-lalistadicontrollopre-aggiornamento" id="aggiornamentoautomatico-lalistadicontrollopre-aggiornamento"></a>

La sezione "La lista di controllo pre-aggiornamento" fornisce informazioni utili sul vostro attuale sistema PrestaShop, e come potrebbe interagire con l'aggiornamento automatico.\
![](<../../.gitbook/assets/23038082 (3).png>)È necessario assicurarsi che tutti i controlli vengono abbiano  prima di poter avviare l'aggiornamento.

* **Il modulo 1-click upgrade è aggiornato (la versione corrente è xx)**. Indica se è necessario aggiornare il modulo di aggiornamento stesso. Se lo avete appena installato, ci sono poche possibilità è necessario aggiornarlo.\
  Se non avete l'ultima versione del modulo, sotto questo campo appare un pulsante, contrassegnati da "Installa l'ultima facendo clic su 'Aggiungi dal mio computer'". Clic su di esso vi porta alla pagina "Moduli". Da lì, cliccare sul link "Aggiungi un modulo dal mio computer" per far apparire il form pre-riempita. Fai clic sul pulsante "Scarica questo modulo" per avviare l'aggiornamento del modulo. Infine, tornare al 1-Click Aggiornamento pagina di configurazione di continuare a svolgere i controlli precedenti l'aggiornamento.
* **La vostra directory di archiviazione principale è scrivibile (permessi CHMOD appropriate)**. Indica se i permessi di lettura / scrittura siano impostati correttamente. In caso contrario, li si dovrà aggironare, utilizzando il client FTP, come FileZilla.\
  Vedere la sezione "Configurazione di sistema e compatibilità di sistema" della Guida introduttiva per una rapida spiegazione di come eseguire un CHMOD.
* **L'opzione PHP "safe mode" deve essere disabilitata.**
* **L'opzione PHP "allow\_url\_fopen" deve essere attivata o CURL deve essere installato.**
* **È necessario mettere il vostro negozio in manutenzione**. Indica se il negozio è attivo o in modalità di manutenzione. È necessario mettere il negozio in modalità di manutenzione durante l'intero processo (backup di file, backup di database, aggiornamento automatico, verifica), in modo da impedire ai clienti di effettuare ordini e perderli ... e per evitare di perdere clienti. Il modulo può disattivare il negozio per voi: è sufficiente cliccare sul pulsante "Clicca qui per mettere il tuo negozio in manutenzione". Si può anche scegliere di disattivare il negozio autonomamente, utilizzando la pagina delle preferenze del negozio:\

  * PrestaShop 1.4: attivare/disattivare il negozio nella scheda principale "Preferenze".
  * PrestaShop 1.5 e versioni successive: attivare/disattivare il negozio nella pagina "Manutenzione", nel menu "Preferenze".
* **È necessario disattivare le funzioni di cache PrestaShop**. Indica se la cache del negozio viene attivata o disattivata. È necessario disattivarla durante l'intero processo. Il modulo non lo farà per voi.
  * PrestaShop 1.4: attivare/disattivare la cache nella pagina "Performances", sotto la scheda "Preferenze".
  * PrestaShop 1.5 e versioni successive: attivare/disattivare la cache della pagina "Performance", nel menu "Parametri avanzati".
* **Il limite di tempo PHP è alto o disabilitato (valore attuale: xxx)**. L'aggiornamento automatico può essere un processo lungo, in quanto il modulo ha bisogno di scaricare l'archivio da [prestashop.com](http://prestashop.com), scompattarlo sul server, sostituire i file attualmente installate, quindi attivare l'aggiornamento stesso. Quindi, le impostazioni di PHP potrebbero essere troppo basse, e bloccare del tutto l'aggiornamento, peggio alla metà del processo. In questo campo, PrestaShop ti dà un'indicazione delle attuali impostazioni del PHP. Idealmente, dovrebbe indicare "disabilitate".

Tutti questi indicatori devono essere verdi per far funzionare l'aggiornamento. In caso contrario, il pulsante di aggiornamento non apparirà.

Attenzione

Quando il negozio è ospitato sul server locale (http: // localhost o [http://127.0.0.1](http://127.0.0.1/)), il modulo di aggiornamento automatico capisce che la modalità di manutenzione non è necessaria, dal momento che nessuno altro ha la possibilità di accedere al sito. Pertanto, anche se non si è in modalità di manutenzione, le spunte sono verdi.

## Inizia la tua Aggiornamento <a href="#aggiornamentoautomatico-inizialatuaaggiornamento" id="aggiornamentoautomatico-inizialatuaaggiornamento"></a>

Questa sezione mette a confronto la versione di PrestaShop con l'ultima più recente stabile. Potete capire immediatamente se è necessario aggiornare o meno. Se sai che esiste una versione più recente disponibile di quella mostrata, è possibile attivare un controllo di versione, fare clic sul  pulsante "Controllare se è disponibile una nuova versione".

![](<../../.gitbook/assets/23038083 (3).png>)

Per impostazione predefinita, lo strumento di aggiornamento è impostato per aggiornare il vostro negozio alla minor versione. Questo significa che se si utilizza una versione dal ramo 1.4.x, non suggerirà l'ultima versione 1.6.x, piuttosto l'ultima versione 1.4.x. Pertanto, se si desidera aggiornare da una versione 1.4.x alla versione più recente 1.6.x, è necessario fare clic sul pulsante "Altre opzioni (modalità Expert)". Si aprirà una nuova sezione, denominata "Altre opzioni (modalità esperto)", dove è possibile scegliere la versione a cui si desidera aggiornare.

Questo è anche molto utile se si desidera controllare se esiste una versione diversa da quella stabile stabile (ad esempio, beta, RC o qualsiasi altra versione instabile).

Prima di lanciare l'aggiornamento, è necessario assicurarsi di aver compreso tutte le impostazioni. Le sezione "Opzioni di backup" e "Opzioni di aggiornamento" sono disponibili in fondo alla pagina (sono descritte più avanti in questo capitolo). Assicurati di aver capito tutto.

## Modalità esperto <a href="#aggiornamentoautomatico-modalitaesperto" id="aggiornamentoautomatico-modalitaesperto"></a>

\
Questa sezione consente di individuare esattamente a quale versione si desidera aggiornare l'installazione PrestaShop corrente.\
PrestaShop 1.6> Aggiornamento automatico> upd004-avanzate-it.png\
Le opzioni sono:\
Channel. Scegliere il canale di distribuzione che si desidera utilizzare. La scelta consigliata è "minor release", che significa "qualsiasi release stabile sopra quello attuale". Le altre opzioni sono:\
Major release. Prossime versioni stabili dall'ultimo ramo: dal momento che il ramo corrente è 1.6.x, lo strumento di aggiornamento sarebbe utilizzare l'ultima versione 1.6 (al momento della scrittura, v1.6.0).\
Minor release. Questa è l'impostazione predefinita. Utilizza solo la prossima release stabile all'interno del ramo corrente: se si dispone di PrestaShop 1.4.2, che aggiornerà il negozio a v1.4.9, anche se v1.6.2 è disponibile.\
Release candidate. Versioni RC sono considerati abbastanza stabile per essere testato da parte della maggioranza, ma non abbastanza stabile per essere il rilascio vero. Utilizzare a proprio rischio.\
Versioni Beta, versione alpha. Si tratta di versioni di sviluppo. Utilizzare a proprio rischio.\
Rilascio privato. A volte, gli sviluppatori PrestaShop carica una versione di prova privato. Se avete l'URL destra e tasto cancelletto, è possibile aggiornare a questa versione facilmente utilizzando questo canale. Se si seleziona la casella "Consenti major upgrade", si indica che sono interessati solo a versioni principali.\
Archivio locale. Da utilizzare se avete scaricato la versione che si desidera eseguire l'aggiornamento a nella cartella locale corretto, / admin / AutoUpgrade / download. Una volta selezionato archivio nella selettore a discesa, indicare il numero di versione nel campo di testo (molto esatto!).\
Directory locale. Da utilizzare se avete scaricato e decompresso la versione che si desidera effettuare l'aggiornamento al primo / admin / AutoUpgrade / ultima cartella / PrestaShop. Quella cartella / PrestaShop deve provenire direttamente dall'archivio scaricato.\
ramo. Indica se tutto è disponibile nel canale prescelto.\
nome. Il nome della versione più recente del canale scelto.\
url. L'URL per la versione più recente del canale scelto.\
md5. La verifica hash per la versione più recente del canale scelto.\
Confronto Version\
Per i curiosi, le differenze tra la versione corrente e l'ultima versione del canale scelto numerato.\
PrestaShop 1.6> Aggiornamento automatico> upd005-versionComparison.png\
Nel caso in cui si dispone di apportare modifiche direttamente ai file principali invece di utilizzare le possibilità superiori di PrestaShop, queste liste possono aiutare a sapere se le modifiche sono sicuri o no.\
Tuttavia, è possibile migliorare la durata della vita del vostro codice personalizzato trasformandolo in file imperative. Consultare la documentazione per sviluppatori per ulteriori informazioni.\
Rollback\
Questa sezione viene visualizzata solo quando è stata eseguita almeno un aggiornamento.\
Vedi sotto per ulteriori informazioni.\
Opzioni di backup\
Queste opzioni consentono di avere un certo controllo sul processo di backup:\
Backup miei files e del database. È necessario avere i vostri file di backup, e il modulo si prenderà cura di questo per voi. Non si dovrebbe mai disattivare questa impostazione, a meno che detto di farlo.\
Backup mie immagini. Si dovrebbe lasciare che il modulo di prendersi cura delle vostre immagini troppo, in modo da essere in grado di fare una pulizia re-installare nuovamente ri-caricamento dei file.\
PrestaShop 1.6> Aggiornamento automatico> upd006-options-it.png\
Opzioni di aggiornamento\
Queste opzioni consentono di avere un certo controllo sul processo di aggiornamento:\
Le prestazioni del server. Alcuni condiviso ospitato offerta scarso rendimento, che potrebbe ostacolare l'esecuzione del processo di aggiornamento, o addirittura renderlo sicuro. "Low" è quindi selezionata per impostazione predefinita, ma se sai di avere un server potente, è possibile scegliere "Medio" o anche "Alto".\
Disabilitare i moduli non-native. Si consiglia di scegliere "Sì" per questa opzione, come alcuni modulo potrebbe rivelarsi un ostacolo quando si aggiorna PrestaShop.\
Aggiornare il tema "default". Il processo di aggiornamento sovrascrive il tema di default, con la sua ultima incarnazione. Se sono state apportate modifiche al tema direttamente, è possibile proteggere queste modifiche, scegliendo "No". Come promemoria, non è consigliabile modificare il tema di default! Si dovrebbe fare una copia del tema, e apportare modifiche a quella copia.\
Aggiornare i predefiniti e-mail. Un aggiornamento potrebbe portare nuovi modelli di posta elettronica predefinito. Per impostazione predefinita, l'aggiornamento sostituirà quelli esistenti con quelli del recente archivio, e aggiungere i nuovi modelli. Se sono stati personalizzati i modelli, si consiglia di tenerli. Si sarebbe quindi necessario personalizzare i nuovi modelli, al fine di adattarsi allo stile generale del vostro negozio.\
Step-by-step modo. Modalità Dev soltanto. Se abilitato, il modulo si ferma ad ogni passo per chiedere conferma.\
Errori di visualizzazione PHP. Modalità Dev soltanto. Se abilitato, il modulo visualizza gli errori di PHP, che potrebbe aiutare a scoprire problemi di server che altrimenti rimanere nascosti alla vista.\
PrestaShop 1.6> Aggiornamento automatico> upd007-upgOptions-it.png\
Il processo di aggiornamento\
Una volta che tutti gli indicatori nella sezione "lista di controllo pre-aggiornamento" sono verdi, il pulsante di aggiornamento appare nella sezione "Avviare il aggiornamento", insieme con l'URL dal quale verrà scaricato la nuova versione.\
Cliccando su "Aggiorna ora PrestaShop!" tasto genera l'intero processo.\
Una volta che il processo di aggiornamento è lanciato, la pagina di configurazione intero è sostituito da due sezioni: "Registro attività" e "rollback".\
Il registro attività fornisce un diario dettagliato di quello che il programma di aggiornamento sta facendo, in una schermata è possibile scorrere:\
File rimossi: solo i file di esempio vengono rimossi, come le classi di override vuoti e controllori.\
Nome dell'archivio di backup: il nome segue la forma auto-backupfiles\_V1.6.0.2\_20140127-120310-798d3a69.zip.\
I file aggiunti all'archivio di backup: tutti i file rimanenti della vostra installazione corrente vengono messi in archivio Zip.\
Le tabelle del database aggiunti all'archivio di backup: i file sono importanti, ma tutto il vostro catalogo sono memorizzati nel database, ed è quindi salvati nello stesso archivio.\
File rimossi: la maggior parte dei moduli, controller, classi CSS e file JavaScript. Ora che tutti i file sono stati salvati nell'archivio di backup, possono essere rimossi in tutta sicurezza.\
I file copiati dal nuovo archivio: tutti i file esistenti vengono sostituiti da loro nuova versione.\
File di traduzione unite.\
Creato, cancellato, modificato e aggiornato le tabelle del database.\
Cartelle temporanee svuotati: se possibile, il upgrader cercherà di eliminare il contenuto delle cartelle di cache.\
Un sacco di file sono menzionati durante l'intero processo. Non hai bisogno di leggere tutte le notifiche, è solo lì per essere esaminate in caso di errore.\
". Aggiornamento completo Si prega di controllare il vostro tema di front office è funzionale (provate a fare un ordine, controllare tema)" Lo saprai l'aggiornamento è finito quando il seguente messaggio appare in verde, insieme con la seguente voce di registro finale: "Fine processo ".\
L'upgrader indica anche che si dovrebbe riattivare il negozio, ma prima di farlo, si dovrebbe innanzitutto verificare che tutto funzioni nel back office: nessun errore, tutti i prodotti e le categorie sono a posto con le loro immagini e file allegati, ecc . Fino a che non controllato che tutto va bene nel vostro negozio, è meglio evitare che agli occhi del pubblico.\
In primo carico, le pagine possono apparire traballante: perché il browser Web memorizza nella cache file, probabilmente sta usando il vecchio CSS file invece di quelle nuove. Non esitate a ricaricare la pagina più volte, o anche svuotare la cache del browser, al fine di ottenere l'interfaccia corretta.

Quando si esegue l'aggiornamento dalla versione 1.4 alla versione 1.6, i menu non saranno disposti nel modo in cui sarebbero stati se hai fatto una nuova installazione di versione 1.6.\
Questo perché PrestaShop 1.4 linguette ricevuti riorganizzate in 1.6 menu, e un sacco di pagine sono state spostate in modo da creare menu coerenti. Inoltre, il Upgrader presuppone che i vostri 1.4 schede potrebbero essere stati personalizzati o spostate, sia da un modulo o da soli azione. Pertanto, piuttosto che rompere le impostazioni esistenti, il Upgrader prende le schede così com'è, e non ri-organizzare nell'ordine menu predefinito 1.6.\
Se si desidera cambiare la posizione delle pagine all'interno di un menu dopo aver aggiornato alla versione 1.6, andare alla pagina di "Menu" nel menu "Amministrazione", e iniziare a giocherellare con le posizioni.\
Una volta che avete fatto in modo che la vostra installazione PrestaShop è installato e funzionante, è possibile riattivare il negozio utilizzando l'opzione nella pagina "Manutenzione" del menu "Preferenze", poi fare le prove sul front office: visualizzare le produzioni, ordinarli, cercare di ordinare uno, ecc In breve, passare attraverso l'intero processo di acquisto, al fine di assicurarsi che non vi perderete una vendita.\
E 'tutto bene funziona? Congratulazioni, si sa hanno aggiornato con successo l'installazione PrestaShop!\
In alcune configurazioni server, potrebbe essere visualizzato un messaggio di errore, ad esempio "errore Javascript (parseJSON) rilevato per azione" upgradeNow ". Avvio di restauro ...".\
Seguire questa procedura per risolvere l'errore,:\
Aprire il file php.ini e attivare (decommentare) le estensioni MySQLi e MySQL DOP. Se non è possibile accedere al file php.ini, contattare il proprio host web su questo.\
Aprire il /modules/autoupgrade/db/Db.php e trovare queste righe (circa 210 riga):\
getClass funzione statici pubblici ()\
{\
&#x20;   $ class = 'MySQL';\
&#x20;   / \* se (PHP\_VERSION\_ID> = 50200 && extension\_loaded ('pdo\_mysql'))\
&#x20;       $ class = 'DbPDO';\
&#x20;   else if (extension\_loaded ('mysqli'))\
&#x20;       $ class = 'DbMySQLi'; \* /\
&#x20;   return $ classe;\
}\
Basta togliere il commento alle righe (rimuovere / \* e \* /). Essi dovrebbero apparire così:\
getClass funzione statici pubblici ()\
{\
&#x20;   $ class = 'MySQL';\
&#x20;   if (PHP\_VERSION\_ID> = 50200 && extension\_loaded ('pdo\_mysql'))\
&#x20;       $ class = 'DbPDO';\
&#x20;   else if (extension\_loaded ('mysqli'))\
&#x20;       $ class = 'DbMySQLi';\
&#x20;   return $ classe;\
}

Dopo aver fatto tutto questo, riavviare il processo AutoUpgrade.\
Tornando alla versione precedente: rollback\
Purtroppo, non tutti gli aggiornamenti sono di successo - che è il motivo per cui molto si dovrebbe sempre il back-up di tutti i file e dati, e perché PrestaShop esegue un backup aggiuntivo di tali file e dati di per sé, che non si deve contare sempre su. Rendere il proprio sostegno in primo luogo. Vedere il capitolo "Esecuzione e ripristinare il proprio backup" di questa guida per ulteriori informazioni.\
Propri file di backup di PrestaShop vengono salvati sul server, e se si scopre l'aggiornamento è andato male, si possono trovare nella sezione "rollback" della pagina di configurazione del modulo 1-Fare clic su Aggiorna.\
I file di backup vengono creati, non appena il processo di aggiornamento si avvia, e sono immediatamente disponibili nell'elenco a discesa "Scegli il tuo backup".\
Scegli il più recente. La data e l'ora della creazione del file di backup sono proprio all'interno del nome: vVersion-Data-ora-casuale, per esempio "V1.4.9.0\_20120907-114024-f85f41a" per il backup di una precedente installazione PrestaShop 1.4.9, fatto 7 Settembre, 2012, alle 11:40:24.\
Il pulsante "Ripristina" innesca due azioni:\
Prende i file dal backup più recente, e li re-installa in sostituzione di quelli dalla versione attualmente installata.\
Prende i dati dal backup più recente, e reinstallato in luogo di quello dal database corrente.\
Selezionare l'archivio di backup da cui si desidera ripristinare e fare clic sul pulsante "Rollback". Come per il processo di aggiornamento, l'intera interfaccia scompare per lasciare solo la sezione "Registro attività" e la sezione "rollback". È possibile seguire il processo di rollback nella rivista di scorrimento, e una volta finito, ricaricare la pagina per verificare che tutto sia davvero a posto.\
Tornando alla versione precedente: il ripristino del proprio sostegno\
Questo è spiegato in dettaglio nella sezione "Esecuzione e ripristinare il proprio sostegno" di questa guida: [http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup](http://doc.prestashop.com/display/PS16/Making+and+restoring+your+own+backup).
