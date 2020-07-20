# libasecnsp11-for-archlinux
In questo repository sono presenti le instruzioni aggiornate per installare il driver per i lettori smartcard che vengono utilizzati per leggere le tessere sanitarie.
## Come procedere?
prima di installare il pacchetto è necessario installare i segueti pacchetti:
- community/pcsc-tools;
- community/pcsclite;
- community/pcsc-perl.

Per installarli basta digitare il seguiente comando
```
sudo pacman -S pcsc-tools pcsclite pcsc-perl
```

## Attenzione
Questa guida è pensata per utenti **Arch linux e derivate**, su altre distribuzioni l'installazione potrebbe variare in alcuni passaggi e nei nomi dei pacchetti, Per le distribuzioni basate su **debian o fedora** basta quardare sul sito della rispettiva regione per ottenere ulteriori informazioni. Ricordo che questa guida richiede comunque delle competenze in materia anche se basse quindi per quanto queste operazioni non sono rischiose, non sono responsabile dei potenziali che potreste creare alla vostra installazione o al vostro pc.
