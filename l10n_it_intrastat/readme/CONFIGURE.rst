**Italiano**

In Impostazioni → Utenti e aziende → Aziende → *Nome azienda*
impostare i parametri delle seguenti sezioni presenti nella scheda "Informazioni generali":

1. Intrastat

   a) ID utente (codice UA): inserire il codice identificativo Intrastat dell’azienda (codice alfanumerico di 4 caratteri, utilizzato come identificativo per l’accesso alle applicazioni delle Dogane).
   b) Unità di misura per kg: parametro che indica l’unità di misura che viene verificata sulla riga fattura soggetta a Intrastat. Se sulla riga il peso è espresso nell’unità di misura indicata nel parametro (o in un suo multiplo), il peso che viene riportato nella corrispondente riga Intrastat è quello preso dalla riga fattura.
   c) Unità supplementare da:

      i. peso: da peso dei prodotti sulla riga Intrastat
      ii. quantità: da quantità dei prodotti sulla riga Intrastat
      iii. nulla

   d) Escludere righe omaggio: esclude dalle righe Intrastat le righe a valore 0.
   e) Delegato: il nominativo della persona delegata alla presentazione della dichiarazione Intrastat.
   f) Partita IVA delegato: la partita IVA della persona delegata alla presentazione della dichiarazione Intrastat.
   g) Nome file da esportare: nome del file che può essere impostato per forzare quello predefinito (SCAMBI.CEE).
   h) Sezione doganale: sezione doganale predefinita da proporre in una nuova dichiarazione.
   i) Ammontare minimo : in caso di fatture di importo inferiore usa questo valore nella dichiarazione

2. Valori predefiniti per cessioni (parametri Intrastat per le fatture di vendita)

   a) Forzare valore statistico in euro: casella di selezione attualmente non gestita.
   b) Natura transazione: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento.
   c) Condizioni di consegna: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento.
   d) Modalità di trasporto: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento (Modo di trasporto).
   e) Provincia di origine: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento (provincia di origine della spedizione dei beni venduti).

3. Valori predefiniti per acquisti (parametri Intrastat per le fatture di acquisto)

   a) Forzare valore statistico in euro: casella di selezione attualmente non gestita.
   b) Natura transazione: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento.
   c) Condizioni di consegna: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento.
   d) Modalità di trasporto: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento (Modo di trasporto).
   e) Provincia di destinazione: indica il valore predefinito che verrà impostato nelle righe Intrastat di una fattura per il campo di riferimento (provincia di destinazione della spedizione dei beni acquistati).

**Tabelle di sistema**


In Fatturazione/Contabilità → Configurazione → Intrastat
sono presenti le funzionalità per la gestione delle tabelle di sistema.

- Sezioni doganali
- Nomenclature combinate
- Modalità di trasporto
- Natura transazione

Tali tabelle sono pre-popolate in fase di installazione del modulo, in base ai valori ammessi per le dichiarazioni Intrastat.

**Posizione fiscale**

L'assoggettamento ad Intrastat può essere gestito anche a livello generale di singolo partner, associandogli una posizione fiscale che abbia l'apposita casella "Soggetta a Intrastat" selezionata.

Tutte le fatture create per il partner che ha una posizione fiscale marcata come soggetta ad Intrastat avranno l’apposito campo "Soggetta a Intrastat" selezionato automaticamente.


**Prodotti e categorie**

La classificazione Intrastat dei beni o dei servizi può essere fatta sia a livello di categoria che a livello di prodotto.

La priorità è data al prodotto: se su un prodotto non è configurato un codice Intrastat, il sistema tenta di ricavarlo dalla categoria a cui quel prodotto è associato.

Per il prodotto la sezione Intrastat si trova nella scheda «Fatturazione/Contabilità», ove è necessario inserire:

- la tipologia (Bene, Servizio, Varie, Escludere);
- il codice Intrastat, tra quelli censiti tramite l’apposita tabella di sistema "Nomenclature combinate" (il campo viene abilitato solo per le tipologie "Bene" e "Servizio").


Per le categorie di prodotti, le informazioni sono presenti in un’apposita area Intrastat della maschera di dettaglio:


**Fatture e note di credito Intrastat**

È possibile indicare l’assoggettamento di una fattura ad Intrastat attraverso l'apposito campo presente sulla maschera di modifica della fattura stessa.

Sulla scheda Intrastat è presente un pulsante «Ricalcola righe Intrastat». Il pulsante permette al sistema:

- di verificare se le righe prodotto presenti in fattura (scheda "Righe fattura") si riferiscono a prodotti che hanno un codice Intrastat assegnato, o appartengono ad una categoria che ha un codice Intrastat aggregato;
- di generare per questi prodotti le corrispondenti righe Intrastat: le righe accorpano prodotti omogenei per codice Intrastat, indicando nel campo "Massa netta (kg)" il peso totale dei prodotti presenti nelle corrispondenti righe. La riga Intrastat, ovviamente, raggruppa il valore economico dei prodotti;
- N.B.: se una riga presente in fattura si riferisce ad un prodotto che ha come tipologia Intrastat “Varie”, l’importo della riga verrà automaticamente suddiviso in maniera uguale sulle altre righe Intrastat che si riferiscono a beni o servizi. Tale automatismo permette di gestire, in maniera conforme a quanto previsto dalla normativa, il ribaltamento proporzionale dei costi sostenuti per spese accessorie (es: spese di trasporto) sui costi sostenuti per l’acquisto vero e proprio di beni o servizi.

Nella scheda Intrastat, un clic su una riga Intrastat permette di accedere alla maschera di dettaglio.

Nella maschera:

- il campo "Stato acquirente/fornitore" viene popolato in automatico dal campo "Nazione" dell’indirizzo associato al partner;
- i campi configurati in Impostazioni → Utenti e aziende → Aziende → *Nome azienda* (vedi "Informazioni generali" su azienda) vengono popolati in automatico con i valori predefiniti impostati, in ragione della tipologia di fattura (vendita o acquisto);
- se fattura di vendita:
  1. i campi Origine → "Paese di provenienza" e Origine → "Paese di origine" vengono popolati in automatico con la nazione presente nell’indirizzo associato all'azienda;
  2. il campo Destinazione → "Paese di destinazione" viene popolato in automatico con la nazione presente nell'indirizzo associato al partner;
- se fattura di acquisto:
  1. i campi Origine → "Paese di provenienza" e Origine → "Paese di origine" vengono popolati in automatico con la nazione presente nell’indirizzo associato al partner (fornitore);
  2. il campo Destinazione → "Paese di destinazione" viene preso dai dati dell'azienda.

N.B.: tutti i campi possono ovviamente essere modificati, ma l’utilizzo del pulsante «Ricalcola righe Intrastat» ripristinerà i valori predefiniti, sui campi prelevati dalla configurazione dell'azienda o dalla riga fattura.


**Note di credito**


Nelle note di credito, sulla scheda Intrastat, è presente inoltre un menù a tendina che permette di selezionare il periodo fiscale di riferimento da rettificare per la nota di credito. Tale valore sarà utilizzato automaticamente nella dichiarazione (sezioni 2 e 4 - Rettifiche).

Importante:

se si seleziona un periodo che è lo stesso della dichiarazione, la nota di credito, per il suo importo, non confluirà nella sezione di rettifica, ma andrà a stornare direttamente il valore della fattura sulla quale è stata emessa. La verifica sulla fattura da stornare viene fatta confrontando la coppia di valori partner/nomenclatura combinata.
