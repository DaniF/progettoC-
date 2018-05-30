# Progetto esame Programmazione C++
## Daniela Frison VR413225
### Descrizione:
Ho implementato un metodo per risolvere un problema di soddisfacibilita'(SAT); il problema e' definito in formato CNF, cioe' e' dato da un insieme di clausole in AND tra loro; una clausola (es. "A B C" o "1 2 3") e' composta da un numero finito di letterali, ovvero un numero finito di variabili; vale la regola che almeno una delle variabili deve essere soddisfatta( e' come scrivere "A OR B OR C" o "1 OR 2 OR 3"). Ogni variabile e' presente positiva o negata(la negazione corrisponde ad inserire un NOT davanti alla variabile, e si trova scritta coma "~A" o "-1"). 
Lo scopo del programma è trovare un assegnamento valido per cui ogni clausola del problema sia soddisfatta, cioe' abbia almeno un letterale VERO(o FALSO se il letterale e' presente nella clausola in forma negata).

### Classi utilizzate:
Il progetto e' suddiviso in varie classi:
..* Clausola: una clausola e' costituita da un inisieme di interi
..* ClausolaAlfabetica: una sottoclasse di clausola che permette di leggere la clausola in formato alfabetico e di trasformarla in formato numerico
..* View: utilizzata per interfacciarsi con l'utente e con i file contenenti degli esempi di problema da risolvere
..* Letterale: rappresentano le variabili(interi) delle clausole, permettono di salvare il valore assegnato alle variabili per risolvere il problema
..* main: mostra unpossibile utilizzo delle classi.

### Implementazione dei requisiti richiesti:
..* polimorfismo: viene applicato nella classe Clausola attraverso la funzione to_string()
..* template di funzione: si trova nella classe View attraverso la funzione stampa
..* template di classe: si trova nel main, attraverso la struttura Insieme
..* namespace: si trova nel main, ci sono namespace uguali_senza_segno e uguali_con_segno
..* constexpr: nella classe View, funzione stampa
..* auto: nel main, come variabili nei for
..* explicit: in Clausola, nel costruttore
..* override: in ClausolaAlfabetica, nella funzione to_string
..* memoria dinamica: in Clausola, nel campo _c.

### Compilazione


