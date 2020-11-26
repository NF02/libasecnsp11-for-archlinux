# libasecnsp11-for-archlinux
In questo repository sono presenti le instruzioni aggiornate per installare il driver per lo standard della tessera sanitaria athena per l'utilizzo con un lettore smartcard, per il TS-CNS.
## Come procedere?
prima di installare il pacchetto è necessario installare i segueti pacchetti:
- community/**pcsc-tools**;
- community/**pcsclite**;
- community/**pcsc-perl**.

Per installarli basta digitare il seguiente comando
```
sudo pacman -S pcsc-tools pcsclite pcsc-perl
```
### Driver del lettore miniLector EVO
Il lettore utilizzato nella regione Sardegna è il miniLectior EVO e il driver è disponibile sul sito del produttore, esso è accessibile cliccando <a href="https://www.bit4id.com/it/lettore-di-smart-card-minilector-evo/">qui</a> o nel repo è presente il PKGBUILD all'interno della cartella **libACR38Driver**.

Ricordo che se avete il lettore di smartcard integrato all'interno del vostro dispositivo non sarà necessario adoperare il suddetto lettore USB e quindi non ha senso installare il driver in questione, dovrete semplicemente installare la libreria **libasecnsp11** e seguire gli altri punti della guida.

### Installazione di libaseCnsP11
A questo punto è necessario clonare il repo e accedere alla directory con il comando:
```
git clone https://github.com/NF02/libasecnsp11-for-archlinux.git && cd libasecnsp11-for-archlinux
```
poi per avviare l'installazione con:
``` sh
makepkg -si
```
*Ovviamente per installare il pacchetto vi verrà richiesta la password di root e quindi i privilegi amministrativi.*

Dopo aver effettuato l'installazione i casi sono due, se il sistema è a 32bit il file "la libreria" sarà presente nel percorso **/lib/libaseCnsP11.so**, invece, nel caso di un sistema a 64bit esso sarà presente nel percorso prima citato con l'aggiunta della suo versione a 64bit all'interno della precorso **/lib64/libaseCnsP11.so**. Questa informazione vi sarà utile perché firefox richiede il caricamento del modulo (**Preferenze > Privacy e Sicurezza > Dispositivi di sicurezza**).

## Attenzione
Questa guida è pensata per utenti **Arch linux e derivate**, su altre distribuzioni l'installazione potrebbe variare in alcuni passaggi e nei nomi dei pacchetti, Per le distribuzioni basate su **debian o fedora** basta quardare sul sito della rispettiva regione per ottenere ulteriori informazioni. Ricordo che questa guida richiede comunque delle competenze in materia anche se basse quindi per quanto queste operazioni non sono rischiose, non sono responsabile dei potenziali che potreste creare alla vostra installazione o al vostro pc.
