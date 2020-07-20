# libasecnsp11-for-archlinux
In questo repository sono presenti le instruzioni aggiornate per installare il driver per lo standard della tessera sanitaria athena per l'utilizzo con un lettore smartcard, per il TS-CNS.
## Come procedere?
prima di installare il pacchetto è necessario installare i segueti pacchetti:
- community/pcsc-tools;
- community/pcsclite;
- community/pcsc-perl.

Per installarli basta digitare il seguiente comando
```
sudo pacman -S pcsc-tools pcsclite pcsc-perl
```
### driver del lettore miniLector EVO
Il lettore utilizzato nella regione Sardegna è il miniLectior EVO e il driver è disponibile sul sito del produttore, esso è accessibile cliccando <a href="https://www.bit4id.com/it/lettore-di-smart-card-minilector-evo/">qui</a>. 
## Attenzione
Questa guida è pensata per utenti **Arch linux e derivate**, su altre distribuzioni l'installazione potrebbe variare in alcuni passaggi e nei nomi dei pacchetti, Per le distribuzioni basate su **debian o fedora** basta quardare sul sito della rispettiva regione per ottenere ulteriori informazioni. Ricordo che questa guida richiede comunque delle competenze in materia anche se basse quindi per quanto queste operazioni non sono rischiose, non sono responsabile dei potenziali che potreste creare alla vostra installazione o al vostro pc.
