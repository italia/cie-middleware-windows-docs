Altre distribuzioni
====================

Nel caso di altre distribuzioni occorre scaricare il file
cie-Software_<VERSIONE>.zip (es. cie-Software_1.1h_x86_64.tar.gz).

Effettuato il download, occorre aprire un terminale e digitare il
seguente comando, dopo essersi posizionati nella directory dove è stato
scaricato il pacchetto di installazione:

*tar xvzf <NOME_FILE>.tar.gz*

Completata l’estrazione dell’archivio occorrerà copiare i files
costituenti il Software nelle seguenti cartelle:

1. Cartella “CIEID” nel percorso /usr/share/

2. File “libcie-pkcs11.so” nel percorso /usr/local/lib/

3. File “CIE_ID”.desktop nel percorso /usr/share/applications/

Digitare pertanto i seguenti comandi:

1. *sudo cp -rp CIEID /usr/share/.*

2. *sudo cp -rp libcie-pkcs11.so /usr/local/lib/.*

3. *sudo cp -rp CIE_ID.desktop /usr/share/applications/.*

avendo cura di confermare con INVIO e di fornire quando richiesto la
password di root.

Se si intende utilizzare il Software all’interno di applicazioni terze
diverse dal browser, è necessario, prima di avviare l’applicazione,
procedere alla corretta impostazione della variabile d’ambiente
LD_LIBRARY_PATH, utilizzando questo comando.

*export LD_LIBRARY_PATH=/usr/local/lib*

seguito da INVIO.
