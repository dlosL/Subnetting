# Subnetting sull'applicazione Filius

#### Strumenti utilizzati

1 Router;
2 Switch;
4 Server

#### Cosa rappresenta il disegno della rete?
Il disegno di rete rappresenta il subnetting, che è una tecnica utilizzata per suddividere una rete IP in sotto-reti più piccole. La suddivisione della rete consente di gestire in modo più efficiente gli indirizzi IP.

Nel caso specifico di una rete IP che prevede la creazione di 2 sotto-reti, il primo passo consiste nell'assegnare un blocco di indirizzi IP alla rete. Il blocco di indirizzi IP può essere rappresentato da una serie di numeri separati da punti, come ad esempio 192.168.1.0/24, dove il valore 24 rappresenta il numero di bit utilizzati per definire la maschera di rete.

Per suddividere il blocco di indirizzi in 2 sotto-reti, è necessario utilizzare una maschera di sottorete che consenta di definire la dimensione di ogni sotto-rete. In questo caso, la maschera di sottorete dovrebbe avere almeno 1 bit aggiuntivo rispetto alla maschera di rete originale per consentire la creazione di 2 sotto-reti. Quindi, la maschera di sottorete diventa 255.255.255.128, che corrisponde a una lunghezza di prefisso di 25 bit.

Con questa nuova maschera di sottorete, la rete IP può essere suddivisa in 2 sotto-reti di dimensioni uguali. L'indirizzo di rete per ciascuna sotto-rete può essere calcolato applicando la maschera di sottorete all'indirizzo di rete originale. Ad esempio, se l'indirizzo di rete originale è 192.168.1.0, i primi 25 bit dell'indirizzo rappresentano l'indirizzo di rete e gli ultimi 7 bit rappresentano gli indirizzi host disponibili in ogni sotto-rete.
Quindi, le 2 sotto-reti avranno gli indirizzi di rete 192.168.1.0 e 192.168.1.128. Ognuna di queste sotto-reti potrà ospitare fino a 126 dispositivi, dal momento che 2 degli 128 indirizzi host disponibili in ogni sotto-rete saranno riservati per l'indirizzo di rete e l'indirizzo di broadcast.

Il subnetting di 2 sotto-reti consente di ottimizzare l'utilizzo degli indirizzi IP, evitando così il rischio di esaurimento degli indirizzi disponibili. Inoltre, la suddivisione della rete in sotto-reti più piccole consente di migliorare le prestazioni della rete, riducendo il traffico di broadcast e migliorando la sicurezza complessiva della rete stessa.
