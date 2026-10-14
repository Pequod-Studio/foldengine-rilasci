# FoldEngine — rilasci

Qui stanno solo i rilasci di FoldEngine per macOS: l'app firmata con Developer ID e notarizzata da Apple, e il manifesto firmato da
cui l'app installata controlla gli aggiornamenti. Il codice sorgente è in un repository privato.

- **Editore**: Alessandro Pedretti (Developer ID, team J9BKAB29A5). Identificativo dell'app: `com.alessandropedretti.foldengine`.
- **Verifica di un download**: ogni rilascio porta lo sha256 dell'archivio; Gatekeeper deve riportare «Notarized Developer ID».
- **Aggiornamenti**: l'app scarica `manifesto.json` dall'ultimo rilascio e lo accetta solo se la firma ECDSA P-256 corrisponde alla
  chiave pubblica compilata nell'app, se l'identificativo coincide e se il manifesto non è scaduto (durata massima 45 giorni). Il
  manifesto si rifirma ogni 30 giorni anche senza versioni nuove.

Copyright 2026 Alessandro Pedretti. Tutti i diritti riservati; nessuna licenza concessa oltre all'uso dell'app distribuita qui.
