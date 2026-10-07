# Osservazioni — Esercitazione 0

Gruppo: a

Componenti (nome, cognome e username GitHub di entrambi): Edoardo Luciani (EdoLuciani) Leonardo Mariani (mariani2258738-max)

URL del repository condiviso: https://github.com/EdoLuciani/esercitazione-0-template.git

Chi ha usato la tastiera nello step 1 e nello step 2: step 1 - Luciani, step 2 - Mariani

Compilate insieme le osservazioni e discutete le risposte: entrambi dovete
saper spiegare le prove svolte.

## Step 1 — Hello World: compilazione ed esecuzione

Comando di compilazione: gcc -std=c17 -Wall -Wextra -Wpedantic hello.c -o hello

Comando di esecuzione e risultato osservato: ./hello, e sul terminale abbiamo osservato l'output corrispondete alla frase indicata nella funzione printf nel codice

Che cosa ho capito su sorgente ed eseguibile: Ho capito che la sorgente è il file contenete il codice che è necessario compilare per ottenere un eseguibile, che potrà essere lanciato dal terminale affinché svolga quanto indicato nel codice della sorgente. Qualora il codice venisse modificato, è necessaria la ricompilazione per ottenere un eseguibile aggiornato.

Output richiesto e comportamento del programma prima della modifica: "Hello, computational physics!" è l'output che ci è stato richiesto di far apparire su schermo: prima della modifica l'eseguibile rendeva come output il testo indicato

Esito dopo la modifica e spiegazione della correzione:

## Step 1 — Git

Quali file ho incluso nel commit e perché: ho incluso i file hello.c e osservazioni.md nel commit perché sono gli unici due che ho modificato e dei quali posso constatarne l'evoluzione.

Come ho verificato che la versione provata sia presente su GitHub: Ho aperto i file su GitHub e ho verificato che la versione presente corrispondesse a quanto selezionato per il push.

Che cosa ho osservato prima e dopo `git pull`, e perché non serve un nuovo clone: Prima di 'git pull' non trovavamo nel file la frase che avevamo modificato attraverso GitHub, mentre dopo 'git pull' il file è stato aggiornato al nuovo commit, ed è necessario un solo clone poiché basta copiare una sola volta il reposit di GitHub sul terminale affinché poi Git possa constatatre le differenze tra i due corrispettivi: serve dunque solo un'azione di clone affinché si crei corrispondenza tra GitHub e la cartella sul terminale, da quel momento in poi attraverso le azioni di push e pull si trasferiscono e modificano file aggiornandoli nell'altro.

## Step 2 — Eco: prima prova

Argomenti passati, comando e risultato: Dagli argomenti passati abbiamo potuto riprendere i concetti di array, puntatori e dichiarazione di variabili.

Che cosa posso concludere: Che per prendere gli argomenti dal comando di esecuzione sul terminale senza utilizzare funzioni di input nel codice sostituiamo la dicitura "void" nell'argomento della funzione main con un intero, che segnala il numero di argomenti inseriti nel testo del comando da terminale (e dunque la dimensione di argv), e un puntatore char* argv[], che punta invece al contenuto di argv[] il quale per ogni locazione di memoria contiene uno degli argomenti passati al codice da terminale.

## Step 2 — Eco: seconda prova

Argomenti passati, comando e risultato: In questa seconda sezione abbiamo ripreso confidenza con la forma necessaria per la funzione di stampa e le sue caratteristiche

Che cosa ho capito su testo, conversioni e stampa: Abbiamo compreso che passando da terminale degli elementi senza utilizzare scanf al codice è necessaria una conversione nel tipo di elemento che si intende tratatre nel codice: dal comando di esecuzione, tutti gli argomenti sono rilevati dal programma come testo, dunque array di caratteri. E' necessaria dunque una conversione degli elementi numerici (percepiti però come testo) presenti nel comando nel valore che effettivamente essi rappresentano mediante strtol e strtod. Per quanto riguarda invece il comando di stampa, occorre specificare nel testo sia il tipo di elemento che bisognerà stampare con %s %d o %f, e, nel caso del double, il numero di cifre dopo la virgola con %.6f.

## Step 2 — Risultato ed errori

Previsioni per l'esecuzione con argomenti validi e per quella con `dodici`:

Contenuto di `eco.txt`, messaggi nel terminale e codici di uscita osservati:

Come un controllo automatico può riconoscere un errore:

## Step 2 — Parametri e calcolo fisico

Quando serve ricompilare e quando basta cambiare gli argomenti: Serve ricompilare quando negli argomenti inseriti nel comando d'esecuzione vengono cambiate le tipologie di elemento o il loro ordine rispetto a come prevede di ricevere i dati il programma, dunque si necessita un cambiamento dello script, mentre ogni qualvolta che cambia l'argomento, ma non la tipologia, basta sostituire il nuovo argomento desiderato eseguendo da terminale il programma.

## Step 2 — Git

Come riconosco nella cronologia i commit dei due step: Attraverso l'intestazione che gli abbiamo dato, che segna data e ora del salvataggio.

Come ho verificato che la versione finale sia presente su GitHub: Ho verificato che la versione finale fosse presente su GitHub dopo il push aprendo i file nella repository e controllando che l'intestazione del commit effettuato coincidesse con l'ultima versione salvata da terminale.
