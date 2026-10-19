# Cronologia degli Aggiornamenti — KRONOS Stock

Tutte le modifiche e gli aggiornamenti importanti di questo progetto saranno documentati in questo file.

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
