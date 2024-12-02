# ZONECRON DONGLE + APPLICAZIONE
## Manuale Utente

![Dongle](../images/dongle/dongle.png)

### Contenuto

1. [Introduzione](#1-introduzione)
2. [Preparativi](#2-preparativi)
   - [2.1 Finestra "Non Chiudere"](#21-finestra-non-chiudere)
   - [2.2 Prima Di Iniziare](#22-prima-di-iniziare)
3. [Connessioni E Accessibilità](#3-connessioni-e-accessibilità)
   - [3.1 Connessione Al Dongle Zonecron](#31-connessione-al-dongle-zonecron)
   - [3.2 Connessione A Flowagility](#32-connessione-a-flowagility)
   - [3.3 Accesso Da Altri Dispositivi Nella Rete](#33-accesso-da-altri-dispositivi-nella-rete)
4. [Display E Operazioni](#4-display-e-operazioni)
   - [4.1 Controllo Del Timer Dall'Applicazione](#41-controllo-del-timer-dallapplicazione)
   - [4.2 Visualizzazione Del Timer Sullo Schermo](#42-visualizzazione-del-timer-sullo-schermo)
   - [4.3 Controllo E Visualizzazione Dell'Ordine Dall'Applicazione](#43-controllo-e-visualizzazione-dellordine-dallapplicazione)
   - [4.4 Streaming](#44-streaming)
   - [4.5 Guida Alle Immagini Di Streaming](#45-guida-alle-immagini-di-streaming)
5. [Varie](#5-varie)
   - [5.1 Più Timer](#51-più-timer)
   - [5.2 Informazioni](#52-informazioni)
   - [5.3 Uscita Dall'Applicazione](#53-uscita-dallapplicazion)

---

## 1 Introduzione

Il ZonEcron©, e quando diciamo ZonEcron©, vogliamo che immaginiate luci al neon e fuochi d'artificio sullo sfondo (ok, salterò questa parte per il resto del manuale, altrimenti diventerà troppo lungo)—come stavo dicendo, il ZonEcron© è stato progettato per soddisfare l'esigenza di cronometraggio delle esecuzioni delle zone (pista, palizzata e altalena) e, logicamente, anche per cronometraggio di brevi sequenze per determinare quale opzione è migliore.

Aggiungere un dongle per gestire il timer da un computer è stata un'evoluzione logica. Il tabellone ZonEcron© ha già il proprio server web, rendendo questa combinazione app-zaino ridondante. Pertanto, se possiedi un tabellone ZonEcron©, questo zaino con l'APP rappresenta un metodo ridondante per comunicare con il timer.

L'APP può essere scaricata [qui](https://zonecron.github.io/ZonEcronGW/).

---

## 2. Preparativi

### 2.1 Finestra "Non Chiudere"

1. Quando l'applicazione si avvia, si aprirà una finestra che non deve essere chiusa. Nella finestra appare "NON CHIUDERE QUESTA FINESTRA" in inglese.
2. Una serie di comandi può essere digitata in questa finestra per test o risoluzione dei problemi. In questa finestra, digita "HELP" e premi il tasto Invio per ulteriori informazioni.
3. I comandi e le risposte in questa finestra sono in inglese. Solo il manuale e l'aiuto sono tradotti nella lingua predefinita configurata.

---

### 2.2 Prima Di Iniziare

1. Quando l'applicazione si avvia, dovrebbe aprirsi anche un browser (Firefox, Chrome, ecc.) con la pagina web che contiene questo manuale. Se non si apre, ciò potrebbe essere dovuto a restrizioni di sicurezza sulla macchina che esegue l'applicazione. In tal caso, apri un browser e digita il seguente indirizzo: 
    - http://localhost:8080 
2. Potrebbe essere necessario provare diverse porte tra 8081 e 8100, se la porta 8080 era già occupata quando l'applicazione è stata avviata: 
    - http://localhost:8081
    - http://localhost:8082
    - ...
2. Nell'angolo in alto a destra, la lingua della sessione attuale può essere cambiata, ma la lingua predefinita non verrà modificata.
3. Il menu a sinistra ha quattro opzioni: "Informazioni", "Collegare", "Controlli" e "Schermi". Cliccando, ad esempio, sulla sezione "Informazioni", appare un sottomenu con altre quattro opzioni: "Manuale", "Sistema", "Tempi" e "Licenza". Cliccando, ad esempio, su "Sistema", verrai reindirizzato alla pagina web con le opzioni per configurare la lingua predefinita (in modo da non doverla cambiare ogni volta che l'applicazione si avvia) e altre informazioni di sistema. Da qui in poi, i riferimenti a ciascuna sezione saranno abbreviati. Questo esempio è abbreviato come **Informazioni -> Sistema**.
4. Il computer deve riconoscere il dongle ZonEcron quando è connesso. Di solito, un segnale acustico suona quando viene collegato un qualsiasi dispositivo USB. Se non lo fa, dovrai installare i driver per il chip CH340G. Ecco il sito del produttore: https://www.wch-ic.com/downloads/CH341SER_ZIP.html .
5. Per i passaggi successivi, il dongle deve rimanere scollegato dal computer fino a quando non viene indicato diversamente.
6. Se intendi collegarti alla piattaforma FlowAgility, assicurati che il computer abbia accesso a Internet, ad esempio navigando su un sito di notizie.

---

## 3. Connessioni E Accessibilità

### 3.1 Connessione Al Dongle Zonecron

1. Per collegare il dongle all'applicazione, fai clic nel menu a sinistra su **Collegare -> Dongle**.
2. La sezione "porta seriale" ha un menu a discesa con le porte seriali disponibili sul computer. Presta attenzione a quali sono.
3. Collega il dongle ZonEcron al computer.
4. Fai clic su aggiorna e controlla nuovamente le porte seriali. Il dongle sarà il nuovo porto che non era presente prima.
5. Fai clic su collegati e apparirà un messaggio grigio: "Aperto. In attesa di un segnale dal dongle." Se tutto va bene, dopo due o tre secondi diventerà verde chiaro, indicando "Dongle trovato. In attesa del segnale del timer."
6. Quando avvii o fermi il timer interrompendo il fascio delle celle, il messaggio deve cambiare in "Dongle e timer verificati." in verde scuro. Se non è così, rivedi l'intero processo di collegamento.

---

### 3.2 Connessione A Flowagility

1. Seleziona nel menu a sinistra **Collegare -> FlowAgility**.
2. Copia l'indirizzo MAC di 12 caratteri.
3. Sul sito di FlowAgility https://FlowAgility.com , dopo aver effettuato il login, vai al test dove hai accesso come organizzatore.
4. Seleziona l'icona di gestione del timer nella parte superiore. Una volta lì, incolla l'indirizzo MAC copiato in precedenza nel campo corrispondente e fai clic su "Accoppia con il timer."
5. La pagina cambierà e apparirà un URL simile a "flowagility.com/ws/timer/123456ABCDEF". Copia questo URL.
6. Tornando alla pagina **Collegare -> FlowAgility**, incolla l'URL nel campo "URL" e fai clic su collegati.
7. Se tutto è corretto, il messaggio "Collegato." dovrebbe apparire in verde. Se non è così, rivedi l'intero processo a partire dal passo 2. Fai attenzione a non includere spazi prima o dopo il testo quando copi, e non includere "https://" o "www" – copia semplicemente l'URL fornito.
8. Una volta collegato, il timer dovrebbe anche apparire come connesso sulla pagina di FlowAgility. Se non è così, aggiorna la pagina.
9. Puoi testare l'avvio e l'arresto del timer, e dovrebbe avviarsi e fermarsi sulla pagina di FlowAgility. Puoi anche testare il ripristino del timer dalla pagina di FlowAgility e verificare se il timer è stato ripristinato.
10. La comunicazione bidirezionale è ora stabilita.

---

### 3.3 Accesso Da Altri Dispositivi Nella Rete

1. Questa applicazione fa sì che il computer su cui è in esecuzione funzioni come un server web locale. Pertanto, le pagine web possono essere accessibili da qualsiasi altro dispositivo (PC, tablet, telefono mobile) che si trova sulla stessa rete.
2. Per accedere da un altro dispositivo, basta aprire un browser web (Firefox, Chrome, ...) e digitare l'indirizzo che appare in **Informazioni -> Sistema** sotto la sezione "Accesso Web", nella riga "Da altri dispositivi sulla rete".
3. **Ad esempio**, è possibile:
    - Avere il computer posizionato su un tavolo con il dongle connesso e l'applicazione in esecuzione senza supervisione
    - Segnare i difetti e i rifiuti da un telefono mobile al bordo dell'arena
    - Visualizzare il tempo, i difetti e i rifiuti su una televisione all'ingresso del ring

---

## 4. Display E Operazioni

### 4.1 Controllo Del Timer Dall'Applicazione

1. Il timer può essere controllato dall'applicazione facendo clic sulla sezione **Controlli -> Timer** nel menu a sinistra.
2. Nell'esempio precedente, questo sarebbe ciò che viene aperto sul telefono mobile.
3. I controlli sono abbastanza intuitivi. Puoi aumentare e diminuire i difetti e i rifiuti, eliminare e ripristinare, segnare i tempi di riconoscimento e altro ancora.
4. È importante notare che per ripristinare il timer, il coppia deve prima essere eliminata. Questo serve a prevenire ripristini accidentali, poiché un ripristino non può essere annullato.
5. Se l'applicazione è connessa a FlowAgility, questi controlli non sono necessari, poiché utilizzare entrambe le opzioni contemporaneamente (controlli e FlowAgility) può causare errori nella registrazione dei risultati.

---

### 4.2 Visualizzazione Del Timer Sullo Schermo

1. Seleziona **Schermi -> Monitor** dal menu a sinistra.
2. Nell'esempio precedente, questo sarebbe ciò che viene aperto nel browser di una smart TV.
3. Questa pagina è progettata per visualizzare il timer al pubblico su un monitor/televisione di dimensioni medie o grandi che consenta di leggere le informazioni da una certa distanza.
4. Il timer in esecuzione verrà visualizzato, così come i difetti e i rifiuti ricevuti dai controlli o dalla piattaforma FlowAgility.
5. In fondo, ci sono due selettori per cambiare i colori di sfondo e del testo se si desidera dare un aspetto più festoso o aziendale. Si consiglia di utilizzare colori con un buon contrasto tra loro.

---

### 4.3 Controllo E Visualizzazione Dell'Ordine Dall'Applicazione

1. Questa funzionalità è un bonus che non è correlato al timer stesso. L'idea è simile all'esempio del timer, dove, da un telefono mobile, indichi il numero del cane nell'anello, e su un monitor o televisione separati, quel numero viene visualizzato in grande formato.
2. Il controllo per questa funzione si trova nel menu a sinistra sotto **Controlli -> Turno**. È possibile gestire l'indicazione del numero del cane nell'anello, così come il numero dell'altezza del salto corrente: 20 (XS in Spagna), 30 (S), 40 (M), 50 (I) e 60 (L).
3. Per visualizzare il turno al pubblico, mostra lo schermo situato nel menu a sinistra sotto **Schermi -> Turno** su un monitor o una smart TV. Queste informazioni sono molto utili per i concorrenti per vedere il numero da lontano e organizzare i propri tempi di preparazione.
4. Come per lo schermo del timer, i colori di sfondo e dei numeri possono essere cambiati con i menu a discesa in fondo.

---

### 4.4 Streaming

1. Le sezioni **Schermi -> Streaming** e **Schermi -> Streaming FA** sono progettate per essere catturate da programmi di streaming.
2. Esse differiscono in quanto la prima è una versione semplificata della seconda per quando FlowAgility non viene utilizzato, ma con le stesse opzioni di personalizzazione.

---

### 4.5 Guida Alle Immagini Di Streaming

Poiché gli schermi di streaming sono progettati in modo speciale e altamente personalizzabili, dedichiamo una sezione per spiegare le possibilità che offrono.

1. Facendo doppio clic su un'area vuota dello schermo si aprirà la finestra generale.
2. In questa finestra generale, puoi inserire manualmente la distanza del corso per visualizzare il calcolo della velocità in tempo reale. La velocità non verrà visualizzata durante i primi 5 secondi del corso. Il campo di input "Velocità Massima" viene utilizzato per evitare di mostrare velocità eccessivamente elevate. Se l'applicazione è connessa a FlowAgility, le informazioni sulla distanza verranno aggiornate automaticamente. In caso contrario, la distanza deve essere inserita manualmente per ogni corsa.
3. Da questa finestra generale, puoi anche caricare un'immagine di sfondo, che verrà salvata con il resto delle personalizzazioni quando salvi.
4. Nello schermo "streaming FA", questa finestra includerà l'opzione per connettersi a FlowAgility. Per aggiornare le informazioni, devi inserire l'URL di connessione fornito da FlowAgility in questo menu e premere il pulsante di connessione.
5. In fondo a questa finestra generale, c'è un pulsante per entrare in modalità di modifica. In questa modalità, puoi trascinare e rilasciare ogni testo (tempo, errori, nome del cane, ecc.) per posizionarlo dove vuoi. Facendo doppio clic su ciascun testo si aprirà una finestra di proprietà dove puoi cambiare la sua dimensione, colore, trasparenza, ecc. Se è aperta una finestra, non puoi trascinare e rilasciare nulla tranne la finestra stessa. Deve essere chiusa per trascinare o modificare altri testi.
6. Attivare l'opzione "Nascondi" per un elemento non lo nasconderà fino a quando non esci dalla modalità di modifica. In modalità normale (non modifica), l'elemento "Eliminato" e gli elementi "Errori" e "Rifiuti" si alterneranno (uno o l'altro) a seconda che la coppia sia stata eliminata o meno. In modalità modifica, entrambi saranno visibili in modo da poter essere modificati. Ad esempio, se decidi di nascondere permanentemente "Errori" e "Rifiuti" attivando l'opzione "Nascondi", l'elemento "Eliminato" manterrà il suo comportamento in modalità normale, diventando visibile solo quando la coppia viene eliminata, e viceversa.
7. In modalità modifica, puoi annullare le ultime 100 azioni con Ctrl + Z o ripetere le ultime 100 azioni annullate con Shift + Ctrl + Z.
8. Una volta terminata la personalizzazione, fai doppio clic su un'area vuota per visualizzare di nuovo la finestra generale e premi il pulsante per uscire dalla modalità di modifica.
9. Nella stessa finestra, premendo il pulsante di salvataggio verranno salvati gli aggiustamenti effettuati e mantenuti anche se la pagina web viene chiusa e riaperta successivamente.
10. Premere il pulsante di salvataggio sincronizzerà anche questi aggiustamenti su tutte le **stesse finestre del browser** che visualizzano la stessa pagina di streaming. Questa funzionalità ti consente di modificare il design della finestra in un'istanza e, quando salvi, aggiorna la finestra in streaming senza mostrare i menu e le proprietà aperte per le modifiche.
11. In caso di errore di comunicazione con il cronometro o la piattaforma FlowAgility, verrà effettuato un tentativo di riconnessione in continuazione con una pausa di 5 secondi tra i tentativi.
12. Il pulsante Importa/Esporta consente di salvare la configurazione in un file per backup o migrazioni. La funzione di importazione è disponibile solo per nuove configurazioni o configurazioni recentemente ripristinate. Se l'opzione di importazione non appare, è necessario premere il pulsante di ripristino per riavviare le configurazioni, poiché qualsiasi modifica trasformerà il pulsante di importazione in un pulsante di esportazione.
13. Alcuni pulsanti o azioni mostreranno un messaggio di aiuto contestuale quando vengono cliccati o quando il mouse passa sopra l'elemento per un paio di secondi.

---

## 5. Varie

### 5.1 Più Timer

1. È possibile eseguire il programma più volte se hai diversi dongle con i loro timer per corsi simultanei, ad esempio.
2. In questo caso, ogni istanza dell'applicazione creerà un punto di accesso diverso, con lo stesso indirizzo ma una porta diversa, ad esempio: 
    - http://localhost:8080 
    - http://localhost:8081 
3. I codici necessari per connettersi a FlowAgility (indirizzo MAC) saranno consecutivi.
4. Le pagine per le prime 8 istanze si apriranno con colori diversi per differenziarle facilmente. A partire dalla nona, se mai dovesse accadere, si apriranno con il colore predefinito.

---

### 5.2 Informazioni

1. Nella pagina web **Informazioni -> Sistema**, puoi:
   - Selezionare la lingua predefinita.
   - Visualizzare gli indirizzi per accedere all'applicazione dal computer in cui è in esecuzione o da un altro dispositivo sulla stessa rete. Ad esempio, se il tuo computer è connesso al Wi-Fi e il tuo cellulare è anch'esso connesso alla stessa rete, puoi accedere all'applicazione dal tuo cellulare inserendo l'indirizzo mostrato nella sezione "Accesso Web", nella riga "Da altri dispositivi sulla rete".
   - Visualizzare lo stato della batteria delle celle ZonEcron.
   - Visualizzare informazioni di base sul dongle (noioso).
   - Visualizzare gli ultimi 10 tempi registrati dal cronometro nel giorno corrente in ordine inverso (il più recente per primo) se l'applicazione è stata connessa al dongle.
2. Nella pagina web **Informazioni -> Tempi**, vengono visualizzati tutti i tempi registrati dal cronometro nel giorno corrente. I tempi dei giorni precedenti sono disponibili anche in file di testo (uno per giorno) nella cartella "logs" all'interno della cartella dell'applicazione.
3. Nella pagina web **Informazioni -> Manuale**, puoi consultare questo manuale.
4. Nella pagina web **Informazioni -> Chi siamo**, puoi leggere la licenza d'uso.

---

### 5.3 Uscita Dall'Applicazion

1. Per chiudere l'applicazione, chiudi semplicemente la finestra "NON CHIUDERE" o digita il comando "esci" al suo interno.
2. Tutte le pagine web aperte su qualsiasi dispositivo perderanno la comunicazione e smetteranno di ricevere informazioni aggiornate.
3. Tutti i dati di configurazione verranno salvati. Se è stata stabilita una connessione riuscita con il dongle o FlowAgility, anche quella configurazione verrà salvata. La prossima volta che l'applicazione verrà avviata, tenterà automaticamente di connettersi al dongle e a FlowAgility utilizzando quella configurazione.
4. Nei giorni diversi, la connessione a FlowAgility cambia, quindi non funzionerà da un giorno all'altro.
