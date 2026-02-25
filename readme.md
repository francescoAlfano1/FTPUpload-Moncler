Nome progetto: FTPUpload Moncler – Upload SFTP automatico verso server Moncler
Tecnologia: VB.NET — libreria WinSCP.NET (Winscpnet.dll); procedura I/E di Business Cube
Tipo: Funzione di integrazione ERP — upload file via SFTP verso sistema cliente
Descrizione:
Funzione integrata nel gestionale Business Cube che automatizza il trasferimento di file verso il server SFTP del cliente Moncler. I parametri di connessione (hostname, porta, credenziali, fingerprint SSH) vengono letti dinamicamente dalle impostazioni aziendali di Business Cube tramite GetSettingBus, rendendo la configurazione modificabile senza toccare il codice. Il file viene trasferito in modalità binaria nella cartella /OUT/ del server remoto.
Funzionalità principali:

Connessione SFTP sicura tramite WinSCP.NET con autenticazione SSH
Lettura parametri di connessione dalle impostazioni aziendali Business Cube (no credenziali hardcoded)
Trasferimento file in modalità binaria
Log dell'esito di ogni trasferimento tramite oCleImex.WriteLog
Gestione errori con logging dell'eccezione e restituzione esito booleano

Punti di forza da evidenziare:

Integrazione B2B con sistema di un cliente enterprise (Moncler)
Configurazione esternalizzata e sicura tramite settings ERP
Utilizzo di libreria professionale per SFTP (WinSCP.NET)

Contesto d'uso: Ambito EDI / integrazione B2B, invio automatico di file verso il sistema informatico di Moncler dall'interno del gestionale Business Cube.
