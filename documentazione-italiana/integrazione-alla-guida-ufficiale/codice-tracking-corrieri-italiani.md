# Codice Tracking corrieri Italiani

I corrieri Italiani mettono a disposizione sul proprio sito solitamente un form per la ricerca dei colli o numeri di spedizione, che viene passato tramite il metodo **GET** di php alla successiva pagina che esegue la vera e propria ricerca.\
E' quindi possibile ricavare stringhe di codice dalle suddette pagine con form, da inserire nella configurazione del corriere.

Spesso non esistono stringhe di tracking ufficiali, e sono ricavate dal sito stesso, con il variare del tempo potrebbero subire modifiche ed andranno quindi aggiornate.\
Si tenga a mente anche che tutti gli ordini effettuati con un corriere prima della modifica del codice di tracking stesso, continueranno ad utilizzare la vecchia stringa di codice, in quanto modificando tale parametro del corriere, Prestashop esegue la duplicazione dello stesso (nella tabella carrier) disabilitando quello col vecchio tracking code, che rimane comunque associato a tutti gli ordini creati prima della modifica, quindi se necessario si dovrà agire direttamente sul database alla tabella carrier.&#x20;

## Corrieri: <a href="#codicetrackingcorrieriitaliani-corrieri" id="codicetrackingcorrieriitaliani-corrieri"></a>

* **Bartolini** - codice di spedizione: http://as777.bartolini.it/vas/sped\_det\_show.hsm?referer=sped\_numspe\_par.htm\&Nspediz=@\&RicercaNumeroSpedizione=Ricerca
* **UPS** - codice di spedizione: http://wwwapps.ups.com/etracking/tracking.cgi?InquiryNumber1=@\&TypeOfInquiryNumber=T\&AcceptUPSLicenseAgreement=yes\&submit=Track
* **GlS - Executive** - codice di spedizione: [http://www.gls-italy.com/tracktrace.asp?tiporicerca=numsped\&locpartenza=xx\&numsped=@](http://www.gls-italy.com/tracktrace.asp?tiporicerca=numsped\&locpartenza=xx\&numsped=@) (sostituire xx con il codice della propria filiale di partenza es: "G1" sono le prime due lettere del codice di una delle vostre spedizioni, da non specificare nuovamente inserendo il codice di traking nell'ordine, mettendo solo la parte numerica successiva)
* **GLS - Executive** - codice di collo: [http://www.gls-italy.com/tracktrace.asp?tiporicerca=numidc=@](http://www.gls-italy.com/tracktrace.asp?tiporicerca=numidc=@) (Utile se si spedisce in pacco singolo, per poter associare il codice all'ordine ancora prima di consegnare al corriere)
