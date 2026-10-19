# Cronologia degli Aggiornamenti — KRONOS Stock

Tutte le modifiche e gli aggiornamenti importanti di questo progetto saranno documentati in questo file.

---

## [1.1.3] - 2026-10-19

### 🚀 Novità e Miglioramenti
- **Riconoscimento OCR Avanzato**: Ottimizzato il motore di ricerca per la tolleranza degli errori di scansione (gestione automatica delle sequenze visive complesse come Z/2 e O/0 su etichette industriali).
- **Ricerca con Prefissi Aziendali**: Aggiunto il supporto alla corrispondenza parziale per identificare l'articolo ufficiale a partire da codici parziali scansionati via webcam.
- **Supporto Articoli Liberi**: Ripristinata la possibilità di registrare sulla commessa codici o materiali di consumo non censiti nell'inventario ERP gestionale.
- **Controllo Manuale dello Scarico**: Eliminato l'invio automatico non richiesto alla commessa; l'operatore mantiene il pieno controllo per verificare codice e quantità prima di confermare.
- **Interfaccia Sincronizzata**: Garantita la visibilità persistente del codice letto o identificato all'interno della barra di ricerca.
- **Compatibilità Report ERP**: Ottimizzato il filtro di lettura dei dati per saltare automaticamente le righe di intestazione nei report di giacenza aziendali.

---

## [1.1.2] - 2026-10-18

### 🚀 Novità e Miglioramenti
- **Doppia Scansione Webcam (Barcode & OCR)**: Introdotta interfaccia nativa Tkinter per scansione da webcam compatibile con OpenCV 5.0.
- **Pulsanti Dedicati**: Separazione delle modalità di acquisizione in "Barcode" e "OCR Testo".
- **Correzione Base OCR**: Filtro automatico per scambi tra 0 e O.
- **Compilazione Standalone**: Ottimizzazione parametri PyInstaller per pacchettizzazione librerie ML in singolo eseguibile portable.

---


## [1.1.1] — 2026-06-06
### 🚀 Novità e Miglioramenti
* **Applicazione Portable:** Confermata la modalità portable senza necessità di installazione.
* **Configurazione Automatica:** Generazione automatica del file di impostazioni (`config.json`) nella stessa cartella dell'eseguibile al primo avvio.
* **Interfaccia e Windows:** Corretta la visualizzazione dell'icona ufficiale sia sulla finestra principale che sulla barra delle applicazioni di Windows tramite AppUserModelID dinamico.
* **Stabilità:** Ottimizzata la velocità di lettura/scrittura dei dati di magazzino e risolti piccoli bug di avvio.

---

## [1.1.0] — 2026-06-01
### 🚀 Novità e Miglioramenti
* **Architettura Modulare:** Ristrutturazione completa del codice sorgente in moduli separati (`main.py`, `gui.py`, `excel_handler.py`, `updater.py`, `config.py`) per una maggiore manutenibilità.
* **Aggiornamento OTA:** Integrato il sistema di controllo e notifica automatica dei nuovi aggiornamenti tramite GitHub.
* **Gestione Excel:** Ottimizzate le funzioni di interazione con i file di magazzino tramite `pandas` e `openpyxl`.

---

## [1.0.0] — 2026-05-15
### 🚀 Rilascio Iniziale
* Prima versione stabile di **KRONOS Stock** per la gestione delle giacenze di magazzino per Veneta Finishing S.r.l.
