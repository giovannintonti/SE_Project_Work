**Descrizione**

Progettare e realizzare il firmware per il sistema di controllo di fornello ad induzione.

**Accensione e spegnimento**

Il dispositivo deve prevedere un pulsante di accensione e spegnimento. Quando il dispositivo è spento,
la pressione del tasto provoca l'accensione dello stesso. Al contrario, quando il dispositivo è acceso la
pressione dello stesso tasto per almeno 1 secondo ne provoca lo spegnimento. Un led deve mostrate
all'utente lo stato del dispositivo.
Lo spegnimento può avvenire in qualsiasi momento se l'utente preme il pulsante apposito.

**Controllo della potenza**

Il dispositivo può operare con quattro livelli di potenza (300W, 500W, 1000W, 1500W). Una volta
acceso il dispositivo, l'utente deve poter aumentare e diminuire la potenza tramite due pulsanti
dedicati.
Appena acceso il dispositivo parte da una potenza nulla (0W) ed il fornello si considera non attivo. Una
volta selezionata la potenza desiderata, il fornello viene attivato se entro 5 secondi questa non viene
variata ulteriormente.
L'utente può variare la potenza del fornello mentre questo è già attivo, ma la nuova potenza verrà
applicata se entro 5 secondi questa non viene variata ulteriormente.
I tasti di aumento/riduzione della potenza devono essere premuti per almeno 1 secondo affichè il
comando abbia effetto.

*Visualizzazione della potenza*

Un led indica l'attivazione del fornello. Il led opera nel seguente modo in accordo alla potenza erogata:
● 0W spento
● 300W lampeggia con periodo di 2s
● 500W lampeggia con periodo di 1s
● 1000W lampeggia con periodo di 500ms
● 1500W lampeggia con periodo di 250ms

**Controllo della presenza**

Il dispositivo deve garantire che il fornello si attivi solo nel caso in cui sia presente un pentola sul piano.
Inoltre, qualora questa venisse rimossa mentre il fornello è attivo, il dispositivo segnala per 10 secondi
l'anomalia tramite un led, se la pentola non viene riposizionata entro questo tempo il dispositivo
disattiva il fornello (potenza 0W).

**Input ed Output**
Il dispositivo è dotato quindi seguenti input e output:
1. Pulsante di accensione/spegnimento
2. Pulsante per aumentare la potenza
3. Pulsante per ridurre la potenza
4. Sensore per rilevare la presenza della pentola
5. Led di accensione del dispositivo (indica se il fornello è acceso, rimane acceso fino a quando
questo è acceso)
6. Led di errore si accende in caso di errore
7. Led di attivazione fornello (indica la potenza erogata dal fornello in accordo ai requisiti
descritti in precedenza)

**Deliverables**
Il team dovrà produrre e consegnare
1. Progettazione del sistema in termini di casi d'uso, diagrammi di attività e diagramma di stato
2. Modellazione del sistema nell'ambiente Simulink tramite Stateflow
3. Ambiente di test in Simulink Test con almeno 5 casi d'uso significativi
4. Codice sorgente e dimostratore hardware con il firmware generato dell'ambiente Matlab