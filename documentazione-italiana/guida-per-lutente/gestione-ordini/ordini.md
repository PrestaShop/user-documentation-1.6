# Ordini

La pagina  "Ordini" nel menu "Ordini" ti abilita a vedere tutte le informazioni relative a tutti gli acquisti del tuo negozio. Tutte le transazioni del tuo negozio sono disponibili qua, organizzate per data (in automatico, sono settate per dalla più recente alla più vecchia).

Puoi filtrare i risultati e trovare facilmente gli ordini che stai cercando usando i campi di cui sopra. Per esempio, per identificare gli ordini di mr Doe, digita Doe nel campo "Cliente" e poi clicca "Filtra".

NON PUOI CANCELLARE UN ORDINE. E' illegale poter rimuovere un'informazione sul pagamento o sull'ordine, e/o sulle fatture relative ad un affare in Europa. Quindi, implementare un tasto "Elimina" per gli ordini, renderebbe illegale PrestaShop in Europa.

Per cancellare in automatico un ordine, installa il modulo "pulitore del database (che è sempre disponibile nella installazione sin dalla versione 1.5.4), apri lo schermo di configurazione e spunta la casella "Ordini e clienti" prima di cliccare sul tasto "Cancella ordini & clienti".

Puoi esportare un elenco di ordini cliccando sul tasto "Esporta" in alto.

Non puoi importare ordini.&#x20;

## Creare ordini <a href="#ordini-creareordini" id="ordini-creareordini"></a>

Uno delle grandi funzioni di  PrestaShop è la possibilità di creare un ordine direttamente dal  back office. Per esempio, questo diventa davvero utile quando un cliente che vorrebbe comprare nun prodotto non ci riesce, e devi farlo al suo posto mentre sei al telefono o durante una conversazione on line con il cliente.

Cliccando su "Aggiungere un nuovo ordine" si apre una nuova pagina con un campo testo intitolato "ricerca dei clienti". Quando crei un nuovo ordine attraverso il back office, la prima cosa da fare è associare l'ordine al cliente. Digita le prime lettere del nome del cliente, il cognome e l'indirizzo  e-mail, e  PrestaShop ti mostrerà gli accounts possibili.

Se il cliente per il quale stai creando un ordine non ha ancora un account, puoi crearne uno cliccando su "Aggiungi un nuovo cliente" per aprire una finestra con i principali dati dell'account da inserire. Una volta che l'account è stato salvato, diventa l'account scelto per l'ordine.

Ricorda che dovrai anche registrare l'indirizzo del cliente - per questo c'è il tasto "aggiungi un nuovo indirizzo" in fondo alla pagina, nella sezione "indirizzo"..

Clicca sul tasto "Scegli" per il corretto cliente, e apparirà l'intero ordine. La sua sezione principale "Carrello", è dove prenderai tutte le necessarie decisioni per questo ordine. Puoi anche scegliere di usare un ordine precedente dello stesso cliente, o un carrello precedentemente abbandonato.

Il campo "Scegli un prodotto" ti permette di cercare dinamicamente i prodotti da aggiungere, digita le prime lettere del suo nome e  PrestaShop  riempirà una lista di prodotti possibili. Scegli un prodotto, seleziona la quantità, clicca sul tasto "Aggiungi al carrello". Puoi ovviamente scegliere tra molte combinazioni di prodotti, se ce ne sono, nella lista di "Combinazioni" che apparirà in tal caso. \
Nota che  PrestaShop ti dà anche indicazioni di quanti prodotti ti rimangono in magazzino, così che puoi dire al cliente che sei sprovvisto di un dato prodotto incluso nell'ordine.

La pagina ti permette di vedere i carrelli e ordini precedenti di quel cliente, se ce ne sono. Se scopri che stai utilizzando un carrello che il cliente in qualche modo non può validare, puoi usare quel carrello per l'ordine, cliccando sul tasto "Usa".

Se necessario, puoi anche garantire un voucher a quell'ordine, o crearne uno sul momento, cliccando sul tasto "Aggiungi un nuovo voucher"

Infine, dovrai specificare a che indirizzo spedire l'ordine e la fattura. Qui, di nuovo, puoi anche creare l'indirizzo sul momento usando il tasto "Aggiungi un nuovo inidirzzo".

## Vedere i dettagli di un ordine <a href="#ordini-vedereidettaglidiunordine" id="ordini-vedereidettaglidiunordine"></a>

Per lavorare gli ordini che ricevi, devi vedere le informazioni che contengono.

Clicca sulla riga che contiene l'ordine o clicca sul tasto a destra dell'ordine.

I dettagli dii un ordine riempiono una pagina intera.

In cima alla pagina c'è un veloce riepilogo dell'ordine: la data in cui è stato validato, il numero della conversazione di servizio con il cliente, il numero dei prodotti, il totale da pagare.

La pagina dei dettagli dell'ordine ti dà accesso a:

* A sinistra, le informazioni sull'ordine:\

  * a che stadio è, e la cronologia degli stadi.
  * le informazioni per la spedizione: il peso totale, e lo spedizioniere scelto dal cliente.&#x20;
* Sulla destra, le informazioni sul cliente:
  * Nomi della storia degli acquisti.
  * Indirizzi di spedizione e fatturazione (usando Google Maps anche con una rudimentale mappa).
* Il metodo di pagamento che è stato utilizzato, il costo dei prodotti, i costi di spedizione.
* Vari dettagli sui prodotti ordinati.

## Modificare l'ordine <a href="#ordini-modificarelordine" id="ordini-modificarelordine"></a>

Gli ordini non sono definitivi. Ci sono molti motivi per i quali potresti dover modificare un ordine prima che tutti i prodotti siano preparati, imballati e spediti: uno dei prodotti non è disponibile in magazzino, il cliente ha cambiato idea, ecc.&#x20;

### Aggiungere un prodotto <a href="#ordini-aggiungereunprodotto" id="ordini-aggiungereunprodotto"></a>

In fondo alla lista "Prodotti",  trovi il tasto "Aggiungi un prodotto", che fa aggiungere un campo all'ordine.&#x20;

Quando aggiungi un prodotto, la tabella dei prodotti aggiunge una nuova riga con alcuni campi. Il primo campo testo è di fatto un piccolo motore di ricerca: digita le prime lettere del prodotto per vedere una lista di prodotti corrispondenti. Seleziona quello che vuoi aggiungere, ed il campo disabilitato diventa disponibile.\
Se il prodotto ha più combinazioni, puoi selezionarlo nella lista a tendina che appare sotto il nome: il prezzo unitario si aggiorna in automatico\
Inserisci la quantità di prodotti e clicca sul tasto "Aggiungi un prodotto": il prodotto è stato aggiunto.

Non si può aggiungere un numero maggiore di prodotti di quanti siano disponibili.&#x20;

### Togliere dei prodotti <a href="#ordini-toglieredeiprodotti" id="ordini-toglieredeiprodotti"></a>

Per cancellare un prodotto, va alla lista prodotti, e puoi o cancellarlo cliccando su "Cancella" o cliccando su "Modifica" se devi modificare solo la quantità.

Puoi modificare la quantità di più prodotti nello stesso momento.

Se la quantità di un prodotto è 0, viene tolto dall'ordine direttamente.\
Non puoi togliere una quantità di prodotti maggiore a quella indicata.\
Clicca sul tasto "Cancella" per cancellare o modificare.&#x20;

## Modificare i dettagli dell'ordine. <a href="#ordini-modificareidettaglidellordine." id="ordini-modificareidettaglidellordine."></a>

Molte sezioni dell'ordine possono essere modificate, attivando un aggiornamento o correggendo dei dati inseriti dal cliente.&#x20;

### Stato dell'ordine <a href="#ordini-statodellordine" id="ordini-statodellordine"></a>

La prima lista a finestra della pagina dell'ordine ti permette di modificarne lo stato. E' una parte molto importante di tutto il processo di monitoraggio, nuove funzionalità e documentazione verrà resa disponibile per l'ordine.

Puoi scegliere tra i seguenti stati:

* In attesa del pagamento dalla banca.
* In attesa della validazione in contrassegno.
* In attesa dell'assegno.
* In attesa del pagamento con PayPal.
* Cancellato.
* Consegnato.
* Ordine in arretrato.
* Pagamento accettato.
* Errore nel pagamento
* Payment remotely accepted.
* in corso di lavorazione.
* Rimborsato.
* Spedito.

Per avere una visione migliore dell'attività relativa all'ordine, ogni modifica dello stato viene registrata e il log appare proprio sotto la lista a finestra delle modifiche di stato. Quindi, devi modificare uno stato solo se è stato chiaramente confermato: non contrassegnare un ordine come "consegnato" se hai inviato il pacco, usa "Spedito", non utilizzare "In corso di preparazione" quando hai solo dato un'occhiata all'ordine, ecc.

Sin dalla versione 1.6.1.0, puoi rispedire una e-mail per un determinato stato dell'ordine al cliente. Per inviare una nuova e-mail, clicca su "Reinvia una e-mail" accanto allo stato dell'ordine. Se nel frattempo hai modificato un ordine, verrà inviata una mail di aggiornamento.&#x20;

### Tasti azione <a href="#ordini-tastiazione" id="ordini-tastiazione"></a>

I tasti azione cambiano in base allo stato dell'ordine. Per esempio, nello stato di "Consegnato" i tasti "Aggiungi un prodotto" e "Togli prodotti" diventano dei nuovi tasti: "Prodotti resi" e "Rimborso parziale".

La restituzione dei prodotti non è attivata in automatico. Per attivarla, va alla pagina "Restituzioni di prodotti" nel menu "Ordini" ed attiva l'opzione in fondo alla pagina. Questa si applicherà a tutti i prodotti dell'ordine.

* **Rimborso Standard**. Disponibile una volta che hai raggiunto lo stato "Pagamento accettato". Non è disponibile una volta che i prodotti sono stati inviati.\
  Da usare solo quando devi rimborsare totalmente un ordine, e può essere utilizzato quando i prodotti sono ancora in magazzino.\
  Clicca sul tasto "Rimborso standard" ed apparirà una nuova colonna nella lista prodotti, chiamata "Rimborso". Inserisci l'ammontare e la quantità per ogni prodotto, scegli una delle opzioni della lista (vedi sotto) e clicca sul tasto "Rimborso parziale" in fondo alla tabella.&#x20;
* **Rimborso parziale**. Disponibile una volta che l'ordine raggiunge lo stato "Pagamento accettato".\
  Da usare quando devi rimborsare solo una parte dell'ordine e non l'ordine totale, sia perchè il cliente ha restituito un prodotto ordinato, o semplicemente come gesto di cortesia per un prodotto danneggiato che un cliente abbia deciso di tenere comunque. \
  Clicca sul tasto "rimborso parziale" e apparirà una nuova colonna nella lista prodotti, intitolata "rimborso parziale". Inserisci l'ammontare e la quantità di prodotti interessati, scegli una delle opzioni in fondo alla lista  (vedi sotto) e clicca sul tasto "rimborso parziale" in fondo alla tabella.
* **Prodotti restituiti.** Disponibile una volta che l'ordine raggiunge lo status di "inviato". PrestaShop deve essere settato in modo da accettare la restituzione delle merci, e non lo si fa dalla pagina Ordini > Restituzione della merce, con l'opzione "attiva i resi".\
  Da utilizzare solo quando un cliente ha restituito i prodotti: una volta che i prodotti sono stati ricevuti, li etichetti restituiti direttamente nell'ordine.\
  Clicca sul tasto "Prodotti restituiti" ed apparirà una nuova colonna nella lista prodotti, intitolata "Resi". Barra la casella dei prodotti interessati, indica la quantità di articoli che sono stati restituiti e clicca sul tasto "Prodotti restituiti" .

Quando imposti un prodotto come restituito o da rimborsare, ci sono 4 opzioni possibili sotto la lista prodotti:

* **Prodotti di nuovo in magazzino**. Una volta controllati,  PrestaShop considererà i prodotti resi come nuovamente disponibili per la vendita, e quindi aumenterà la scorta di tale prodotto. Non bisogna utilizzare questa opzione se il prodotto è stato restituito rotto....
* **Generare una nota di credito**. Una volta controllato, si crea una nota di credito per i prodotti selezionati. Una nota di credito è un modo per riconoscere che il tuo negozio ha ricevuto della merce in reso e che è stato emesso un rimborso. Il cliente può utilizzare questo credito per il suo prossimo acquisto.
*   **Generare un voucher**. Una volta controllato, si crea un voucher per la somma degli articoli selezionati. Un voucher è di fatto un codice per uno sconto che il cliente può utilizzare quando fa un pagamento. \
    Puoi modificare i vouchers di un cliente guardando la pagina del cliente: dalla pagina dell'ordine corrente, clicca sul link sotto il nome del cliente nella sezione "informazioni sul cliente", una volta che sei nella pagina del cliente, vai alla sezione " "Vouchers" . Puoi modificare ciascun voucher cliccando l'icona "Modifica" .

    In PrestaShop, vouchers fanno parte di uno speciale tipo di funzione sconto: regole del carrello. Possono venire create e modificate dalla pagina "Regole del carrello" sotto il menu "Regole del prezzo". Il processo di creazione delle regole del carrello sono nel prossimo capitolo "Creare regole del prezzo e Vouchers".
* **Rimborsare il costo di spedizione**. Puoi scegliere di rimborsare il costo di spedizione relativo ad un prodotto reso, che viene sempre apprezzato.

Se il cliente ha pagato l'ordine usando una carta di credito, il sistema di pagamento dovrebbe rifondere la carta automaticamente. Se l'ordine è stato pagato con un assegno o con un bonifico, allora devi effettuare un rimborso, poi etichettare l'ordine come rimborsato manualmente nel back office (nella pagina dell'ordine).

Difference between a credit slip, a voucher and a cart rule

Una nota di credito è la prima e principale prova scritta che un prodotto è stato restituito. Quasi sempre, il cliente può utilizzarlo come voucher.

Un voucher è un codice sconto che non deve essere collegato alla merce restituita o rimborsata, e che può prendere varie forme oltre ad una nota di credito:

* Uno sconto per un ordine (percentuale).
* Uno sconto per un ordine (somma).
* Spedizione gratuita.

Puoi applicare un voucher a tutti i clienti, o a un gruppo di clienti, o ad un singolo cliente, puoi inserire anche una data di scadenza;

La regola carrello è una versione avanzata dei voucher: oltre a ciò che un voucher può fare nella versione PrestaShop 1.4, il sistema di regole carrello introdotte nella versione di PrestaShop 1.5 ti permette:

* dare un nome allo sconto.
* Permettere al cliente di utilizzare solo una parte dello sconto.
* Dare delle priorità tra le varie regole carrello.
* Impostare le compatibilità tra le regole carrello.
* Far si che lo sconto funzioni solo con alcuni spedizionieri.
* Far si che lo sconto funzioni solo per dei prodotti selezionati e/o categorie di prodotti e/o produttori e/o fornitori ecc, oppure tutte queste allo stesso tempo se necessario!
* Far si che lo sconto sia applicabile alla spedizione gratuita e/o ad unoo sconto per un ordine e/o per un regalo, o per tutti questi allo stesso tempo!

### Documenti <a href="#ordini-documenti" id="ordini-documenti"></a>

Puoi creare tutti i documenti in pdf che vuoi dalla pagina ordine. Quando sono disponibili, sono elencati nella sezione "Documenti" .Puoi scaricare l'ordine stesso in Pdf, cliccando sul tasto "Stampa l'ordine" a destra.

Puoi creare una fattura per un ordine cliccando sul tasto "Genera fattura" dalla sezione "Documenti". La fattura può essere generata una volta che l'ordine viene inserito nello status "pagamento accettato" .

Una volta che viene generato, il tasto "Vedi fattura" che sta sotto viene attivato nella barra in alto.

Puoi personalizzare la fattura facilmente: i files dei template del Pdf sono posizionati nella cartella `/pdf` folder. Questi files `.tpl` sono dei files in HTML con degli Smarty tags per dati dinamici. Puoi cambiare la struttura della fattura modificando il file chiamato `invoice.tpl`.

Quando un ordine viene inserito nello status "in corso di preparazione" viene generata una nota di consegna in Pdf, che può venire scaricata dalla sezione "Documenti".

### Spedizione <a href="#ordini-spedizione" id="ordini-spedizione"></a>

I dettagli di spedizione dell'ordine corrente possono venire parzialmente modificati. Più specificatamente, puoi modificare il numero di tracciabilità: nella sezione "Spedizione" clicca sull'icona "Modifica" nella colonna "numero di tracciabilità" e poi inserisci il nuovo numero.Shipping Address

La sezione "Indirizzo di spedizione" ti permette di modificare l'indirizzo di destinazione del pacco che state per spedire. Puoi utilizzare sia una lista a tendina per scegliere un altro indirizzo che il cliente ha già inserito nel tuo negozio, o puoi utilizzare l'icona "modifica" nell'indirizzo prescelto.

Se ti serve inviare un pacco ad un indirizzo che non è stato ancora registrato in PrestaShop, devi prima crearlo. Per far questo, vai al menu "Clienti", apri la pagina "Indirizzi" e clicca sul tasto "Aggiungi uno nuovo".  Non dimenticare di inserire la giusta mail del cliente, in quanto questo è il modo in cui PrestaShop saprà associare il nuovo indirizzo al cliente già esistente. Una volta fatto, vai alla pagina dell'ordine e cambia l'indirizzo usando la lista a tendina.

Nota che una piccola mappa ti permette di visualizzare la destinazione del pacco nella mappa di Google.

### Indirizzo della fattura  <a href="#ordini-indirizzodellafattura" id="ordini-indirizzodellafattura"></a>

La sezione "indirizzo della fattura" ti permette di modificare l'indirizzo del pagamento nell'ordine. Così come per l'indirizzo di spedizione, puoi scegliere un altro indirizzo che il cliente ha già inserito nel tuo negozio, oppure utilizzare l'icona "Modifica" per modificare l'indirizzo corrente.

Se ti serve che un pagamento sia collegato ad un indirizzo non ancora registrato  in PrestaShop, devi prima crearlo. Per farlo, vai al menu "Clienti", apri la pagina "Indirizzi" e clicca sul tasto "Aggiungi uno nuovo". Non dimenticare di inserire la giusta mail del tuo cliente, you must first create it. To do this, go to the "Customers" menu, open the "Addresses" page, and click in the "Add new" button. Do not forget to put the correct e-mail of the customer, in quanto questo è il modo in cui PrestaShop saprà associare il nuovo indirizzo al cliente già esistente. Una volta fatto, vai alla pagina dell'ordine e cambia l'indirizzo usando la lista a tendina.

### Sconto <a href="#ordini-sconto" id="ordini-sconto"></a>

Nella sezione "Prodotti", in fondo alla lista prodotti, c'è il tasto "Aggiungi un nuovo sconto". Questo crea un semplice sconto, non così avanzato come il sistema vouchers/regole carrello, ma comunque utile.

Cliccando si aprirà un nuovo modulo, con i sotto indicati articoli:

* **Nome**. Dai un nome breve allo sconto. Sarà di aiuto al tuoi clienti.
* **Tipo**. Scegli il tipo di sconto: "percentuale", "ammontare" o "spedizione gratuita" .
* **Valore**. Per ogni tipo di "percentuale " o "ammontare", inserisci il valore dello sconto.
* **Fattura**. Seleziona la fattura dell'ordine a cui applicare lo sconto. Quando vi sia più di una fattura, puoi selezionare la casella per applicare lo sconto a tutte le fatture.&#x20;

Lo sconto verrà applicato al totale al netto dei costi di spedizione.

## Allegare un messaggio ad un ordine <a href="#ordini-allegareunmessaggioadunordine" id="ordini-allegareunmessaggioadunordine"></a>

Nella sezione "Nuovo messaggio" a destra sulla pagina, puoi allegare un commento all'ordine che arriva ai tuoi collaboratori.

Puoi far si che questo commento arrivi anche al cliente, in modo da fornirgli informazioni sull'ordine, su ritardi, una sorpresa, tenerlo informato su offerte. Questo è un punto molto importante per i rapporti con i clienti.&#x20;

Ci sono due links disponibili:

* **Clicca qua per aggiungere un commento o inviare un messaggio al cliente.**
  * Puoi aggiungere un messaggio semplicemente scrivendo nella casella messaggio e cliccando "Invio". Il messaggio verrà archiviato nel profilo del cliente nel database del tuo Servizio Cliente, al quale puoi accedere sia andando sulla pagina del cliente, sia nella pagina di Servizio al Cliente. Puoi anche scegliere di inviare il messaggio alla mail del cliente.&#x20;
  * Dei messaggi predefiniti possono essere salvati ed utilizzati più volte, in modo da non doverli riscrivere ogni volta. Se vuoi inviare uno di questi messaggi, selezionalo dalla lista a tendina. Puoi anche aggiungere ulteriori dettagli al messaggio predefinito, se necessario. Puoi anche creare altri messaggi predefiniti usando la funzione nella pagina "Ordine messaggi"  sotto la pagina "Ordini" .
* **Clicca qua per vedere tutti i messaggi**. Questo link ti porta alla pagina "Servizi clienti" nel menu "Clienti" . Questo viene spiegato in modo dettagliato nel capitolo "Gestire i clienti" di questa guida.&#x20;
