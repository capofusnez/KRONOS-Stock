⏳ KRONOS Stock
Sistema intelligente e multi-postazione per la gestione, sincronizzazione e scarico dei materiali sulle commesse aziendali.

🎯 Obiettivo del Software
KRONOS Stock è un'applicazione desktop sviluppata in Python (con interfaccia grafica nativa tkinter) progettata specificamente per reparti produttivi e officine industriali. Il software funge da ponte ad alta velocità tra il listino/inventario centrale del gestionale aziendale (file ERP) e le cartelle di commessa archiviate sul NAS di rete, automatizzando lo scarico dei materiali tramite lettore di codici a barre o ricerca testuale.

✨ Funzionalità Principali
1. Gestione Intelligente delle Commesse su NAS
Esplorazione Dinamica: Si collega direttamente alla struttura di rete principale del NAS, suddividendo automaticamente le commesse per anno e cartella.

Sincronizzazione in Tempo Reale (Pool di Scrittura Concorrente): Permette a più operatori di lavorare contemporaneamente da PC diversi sullo stesso file Excel di commessa senza rischiare corruzioni o sovrascritture accidentali.

Sistema di Blocco e Rilettura Fresca (FileLockManager): Se un PC sta aggiornando il file, le altre postazioni attendono in coda in modo trasparente e rileggono immediatamente lo stato aggiornato dal NAS prima di sommare le nuove quantità.

2. Scansione Barcode & Ricerca Intelligente
Scansione Immediata: Ottimizzato per lettori di codici a barre (Barcode Scanner). Premendo Invio dopo la scansione, il programma individua l'articolo e invia istantaneamente la quantità al file Excel.

Filtro Testuale Dinamico: Permette la ricerca rapida per codice o descrizione parziale all'interno dell'inventario del gestionale.

Gestione Voci Libere: Possibilità di inserire materiali al volo anche se non ancora censiti nel listino ERP principale.

3. Interfaccia Ergonomica e Moderna (GUI)
Design Dashboard Industriale: Palette di colori scuri e card pulite (Dark Header, accenti blu/verde/arancio) studiate per ridurre l'affaticamento visivo.

Layout Ottimizzato: Pulsanti d'invio posizionati strategicamente subito sotto i campi quantità per velocizzare le operazioni ripetitive degli operatori.

Gestione Materiali Registrati: Tabella in tempo reale dei componenti già scaricati con funzioni di modifica rapida della quantità e rimozione riga.

4. Controllo Versione & Aggiornamenti Automatici (GitHub Integration)
Verifica all'Avvio: Il programma interroga le API di GitHub per controllare se sono state pubblicate nuove Release.

Notifica Aggiornamenti: Avvisa l'operatore con le note di rilascio (release notes) se è disponibile una nuova versione dell'eseguibile.

🛠️ Stack Tecnologico
Linguaggio: Python

Interfaccia Grafica: tkinter + ttk

Manipolazione Dati ed Excel: pandas, openpyxl

Architettura di Rete: File locking temporizzato basato su file .lock per ambienti condivisi SMB/CIFS.

Packaging: Compilato in eseguibile unico stand-alone tramite PyInstaller (--onefile --noconsole).

Riferimenti da aggiornare nel codice Mag_Interattivo.py
Quando crei la repository KRONOS-Stock (o kronos-stock) su GitHub, assicurati di aggiornare le costanti all'inizio del file Python così:


---

## ⚖️ Licenza e Termini d'Uso
Copyright © 2026 **Veneta Finishing S.r.l.** — Tutti i diritti riservati.

**KRONOS Stock** è distribuito come software gratuito ad uso diretto.

- **Uso consentito:** È permesso scaricare, installare ed utilizzare liberamente l'eseguibile per scopi operativi e gestionali.
- **Restrizioni:** È severamente vietato riassemblare, decompilare, ri-commercializzare, vendere o ridistribuire il software sotto altro nome, marchio o licenza senza l'autorizzazione.**.
