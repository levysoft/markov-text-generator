# Markov chain per generare nonsense leggibili
Markov è un generatore di testo che utilizza una semplice catena di Markov per produrre testo leggibile ma privo di significato.
Questa tecnica, sebbene generi prosa che non ha molto valore letterario, è sorprendentemente utile per prevedere la prossima parola, simile ai suggerimenti della tastiera del telefono.

## Ispirazione
Questo progetto è stato ispirato dall'articolo "Understanding Markov Chains" di Ben Hoyt e dal capitolo 3 del libro "The Practice of Programming" di Kernighan e Pike. In particolare, l'articolo di Hoyt fornisce una spiegazione chiara dell'algoritmo e delle sue applicazioni, che vanno oltre la semplice generazione di testo.

## Algoritmo
L'algoritmo inizia con un testo di input da cui generare l'output. Per ogni coppia di parole nel testo di input, registra una lista delle possibili parole che possono seguire la coppia. Una volta costruita questa struttura dati, è possibile generare output di qualsiasi lunghezza. Si inizia con una coppia di parole presente nell'input e si sceglie casualmente una delle possibili terze parole. Si procede poi spostandosi di parola in parola.

## Esempio
Per illustrare, utilizziamo un input piccolo come gli ultimi cinque dei Dieci Comandamenti dalla Bibbia del Re Giacomo. La struttura di "terze parole possibili" per alcune entrate iniziali sarebbe:

- shalt not: kill. | commit | steal. | bear | covet | covet
- Thou shalt: not | not | not | not | not

E così via. L'output generato rifletterà la struttura e il "sapore" del testo di input, aggiungendo un tocco di originalità.

## Implementazione in Python
Il codice è conciso e leggibile, composto da meno di 25 linee. Questo codice prevede che il numero di parole venga passato come argomento da riga di comando e che il testo di input venga fornito su stdin.

## Conclusione
L'algoritmo di catena di Markov, nonostante la sua semplicità, rivela come una struttura dati semplice e un generatore di numeri casuali possano produrre output affascinanti. Questo progetto è un esempio di come le scelte di design eleganti possano semplificare il codice e migliorare l'output.

## Licenza
Questo progetto è liberamente ispirato e basato su concetti esposti nell'articolo di Ben Hoyt e nel libro di Kernighan e Pike. Sei libero di utilizzare, modificare e distribuire il codice come preferisci.
