# Installazione di PrestaShop usando lo script da riga di comando.

Dalla versione 1.5.4, PrestaShop ha un installer da riga di comando.

## Cosa sarebbe <a href="#installazionediprestashopusandoloscriptdarigadicomando.-cosasarebbe" id="installazionediprestashopusandoloscriptdarigadicomando.-cosasarebbe"></a>

Questo speciale programma di installazione rende possibile installare PrestaShop, senza la necessità di utilizzare un browser web: in poche parole metti il contenuto dell'archivio zip sul tuo server web, e potrai installare PrestaShop tramite l'interfaccia a riga di comando (CLI). Qualsiasi software CLI può essere utilizzato, fino a quando avrai possibilitò di interagire coi comandi del server : Bash, Windows PowerShell, OS X Terminal, PuTTY, ecc\
\
Il motivo di avere un installatore CLI in aggiunta al normale programma di installazione in-browser è quello di soddisfare alcuni utenti avanzati, che spesso preferiscono interfacce da riga di comando che tendono a fornire un mezzo più elementare e potente per controllare un programma o sistema operativo.

## Come usarlo <a href="#installazionediprestashopusandoloscriptdarigadicomando.-comeusarlo" id="installazionediprestashopusandoloscriptdarigadicomando.-comeusarlo"></a>

L'installatore CLI è facile da utilizzare: dal tuo terminale, vai alla cartella `/install` (o `/install-dev`) , e avvia lo script con questo comando:

```
$ php index_cli.php
```

Questo ti mostrerà le varie opzioni disponibili.

![](<../../.gitbook/assets/16779385 (3).png>)

Tutte le opzioni del regolare programma di installazione in-browser sono disponibili, con il loro valore di default elencato. Quasi tutti i valori di default possono essere lasciati così come sono, perché li puoi modificare  dal PrestaShop back-office una volta terminata l'installazione. Si noti che l'e-mail e la password saranno utilizzati per creare l'account di back-office dell'amministratore ...

Per avviare l'installazione, è sufficiente fornire un argomento. In realtà, è necessario fornirne qualcuno di più :

* **domain**. La posizione dove vuoi che il tuo store appaia.
* **db\_server**. L'indirizzo del tuo database.
* **db\_name**. Il nome del database che vuoi utilizzare.
* **db\_user**. Il nome utente del database che vuoi utilizzare.
* **db\_password**. La password dell'utende del database sopra citato.

per esempio:

```
$ php install_cli.php --domain=example.com --db_server=sql.example.com --db_name=prestashop --db_user=root --db_password=123456789
```

![](<../../.gitbook/assets/16779386 (3).png>)

se anche imposti il valore di `--email` col tuo indirizzo di posta, una e-mail di riepilogo ti sarà spedita una volta terminata l'installazione.

## Lista degli argomenti <a href="#installazionediprestashopusandoloscriptdarigadicomando.-listadegliargomenti" id="installazionediprestashopusandoloscriptdarigadicomando.-listadegliargomenti"></a>

Ecco qui la lista degli argomenti per index\_cli.php alla versione 1.6:

| Name           | Default setting    | Description                                                |
| -------------- | ------------------ | ---------------------------------------------------------- |
| --step         | process            |                                                            |
| --language     | en                 | codice iso della lingua                                    |
| --timezone     | localhost          |                                                            |
| --domain       | localhost          |                                                            |
| --db\_server   | localhost          |                                                            |
| --db\_user     | root               |                                                            |
| --db\_password | (blank)            |                                                            |
| --db\_name     | prestashop         |                                                            |
| --db\_clear    | 1 (true)           | Drop delle tabelle esistenti                               |
| --db\_create   | 0 (false)          | Crea il database se non esiste ancora                      |
| --prefix       | ps\_               |                                                            |
| --engine       | InnoDB             | InnoDB/MyISAM                                              |
| --name         | PrestaShop         | Nome dello shop                                            |
| --activity     | 0                  |                                                            |
| --country      | fr                 |                                                            |
| --firstname    | John               |                                                            |
| --lastname     | Doe                |                                                            |
| --password     | 0123456789         |                                                            |
| --email        | pub@prestashop.com |                                                            |
| --license      | 0 (false)          | Mostra la licenza di PrestaShop                            |
| --newsletter   | 1 (true)           | Sottoscrivi l'amministratore alla newsletter di Prestashop |
| --send\_email  | 1 (true)           | Manda una e-mail all'amministratore dopo l'installazione   |
