# 📄 IPS — Individuazione Personale Scolastico

![Version](https://img.shields.io/badge/Versione-4.8-orange)
![License](https://img.shields.io/badge/Licenza-CC%20BY--NC--SA%204.0-blue)
![HTML](https://img.shields.io/badge/HTML-Single%20File-red?logo=html5)
![GitHub stars](https://img.shields.io/github/stars/sebastianobasile/ips)
![GitHub forks](https://img.shields.io/github/forks/sebastianobasile/ips)

**IPS** è un generatore di documenti ufficiali per l'**Individuazione del Personale Scolastico** a tempo determinato da graduatoria d'istituto per la segreteria che si occupa di assunzioni del personale. Funziona come **singolo file HTML** — nessuna installazione, nessun server, nessun database. Si apre direttamente nel browser.

Sviluppato da **Sebastiano Basile** — [superscuola.com](https://www.superscuola.com)
per il [3° I.C. Capuana-de Amicis](https://www.3iccapuana.edu.it), Avola (SR).

Se ti piace questo strumento [![Contributo volontario](https://img.shields.io/badge/Offrimi_un_caffè_☕-PayPal-blue)](https://paypal.me/superscuola)

---

## ✨ Funzionalità principali

- 📝 **Compilazione guidata** del documento con pannello laterale
- 👁️ **Anteprima in tempo reale** del documento finale (layout A4)
- 📥 **Esportazione PDF** con nome file automatico (`individuazione_COGNOME-NOME_DD-MM-AAAA.pdf`)
- 🔄 **Calcolo automatico** della durata del contratto in giorni
- 💾 **Salvataggio automatico** dei campi nel browser (localStorage) — i dati restano anche chiudendo la finestra
- 🔁 **Tasto reset** per pulire rapidamente i dati del personale mantenendo la configurazione
- ⚧ **Accordo grammaticale automatico** maschile/femminile (sig./sig.ra, nato/nata, ecc.)
- 👩‍💼 Supporto per **Personale Docente** e **Personale ATA** (Assistente Amministrativo, Collaboratore Scolastico)
- 📅 Data Generale con sincronizzazione automatica su Data Convocazione e Data Assunzione

---

## 🚀 Utilizzo

Non è richiesta alcuna installazione.

1. **Scarica** il file `index.html` (pulsante verde **"Code → Download ZIP"**, oppure clic destro → Salva)
2. **Aprilo** con qualsiasi browser moderno (Chrome, Edge, Firefox, Safari)
3. **Compila** il pannello a sinistra — il documento si aggiorna in tempo reale
4. Clicca **"SCARICA PDF (A4)"** per generare il PDF ufficiale

> Il file funziona **offline**, senza connessione internet, dopo il primo caricamento.

---

## ⚙️ Personalizzazione

Tutta la configurazione dell'istituto è concentrata nel blocco `:root` in cima al file HTML.
Aprilo con un editor di testo (Blocco Note, VS Code, ecc.) e modifica le variabili:

```css
:root {
    --nome-scuola: "NOME DEL TUO ISTITUTO";
    --sottotitolo-scuola: "Ordini di scuola · Indirizzo · Tel. · Sito web";
    --titolo-doc: "INDIVIDUAZIONE PERSONALE SCOLASTICO";
    --sub-titolo-doc: "per contratto a tempo determinato da graduatoria d'istituto";
    --ds-nome: "Prof. NOME <b>COGNOME</b>";
    --ds-firma: "Firma autografa sostituita a mezzo stampa<br>ai sensi dell'art. 3 comma 2 D.Lgs. n. 39/93";
    --font-size: 11.5pt;
}
```

| Variabile | Descrizione |
|---|---|
| `--nome-scuola` | Denominazione ufficiale dell'istituto (intestazione documento) |
| `--sottotitolo-scuola` | Ordini di scuola, indirizzo, telefono, sito web |
| `--titolo-doc` | Titolo principale del documento |
| `--sub-titolo-doc` | Sottotitolo (es. tipo di graduatoria) |
| `--ds-nome` | Nome e cognome del Dirigente Scolastico (supporta `<b>` per il grassetto) |
| `--ds-firma` | Testo sotto il nome del DS (formula legale firma sostitutiva) |
| `--font-size` | Dimensione del font del documento stampato |

---

## 📋 Campi del pannello di compilazione

### Dati generali e protocolli
- **Data Generale** — si propaga automaticamente a Data Convocazione e Data Assunzione se non impostate singolarmente
- Protocollo Generale, Protocollo Convocazione, Protocollo Assunzione
- Data Convocazione, Data Assunzione

### Anagrafica personale
- Sesso (Uomo / Donna) — gestisce automaticamente tutti gli accordi grammaticali nel testo
- Cognome e Nome
- Data di Nascita

### Dettagli incarico
- Tipologia: Personale Docente / ATA (Assistente Amm.) / ATA (Collaboratore Scolastico)
- Ordine di Scuola (solo per Docenti): Infanzia / Primaria / Secondaria
- Classe / Posto / Profilo

### Graduatoria e date
- Fascia: 1ª, 2ª, 3ª d'Istituto oppure Interpello
- Posizione in graduatoria e punteggio
- Ore settimanali
- Date di inizio e fine supplenza
- ASS. Amm. responsabile della pratica
- Altre note

---

## 🔒 Privacy e dati

Tutti i dati inseriti vengono salvati **esclusivamente nel browser locale** (localStorage) del computer utilizzato. Nessun dato viene trasmesso a server esterni. Chiudendo il browser i dati persistono; il tasto **"PULISCI CAMPI"** li rimuove completamente.

---

## 📄 Licenza

Distribuito con licenza **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)**.

- ✅ Puoi usarlo, modificarlo e ridistribuirlo liberamente
- ✅ Devi mantenere l'attribuzione all'autore originale
- ❌ Non puoi usarlo per scopi commerciali
- ❌ Le versioni modificate devono usare la stessa licenza

Consulta il file [LICENSE](LICENSE) per il testo completo.

---

## 🤝 Contribuire

Segnalazioni di bug e suggerimenti tramite le **Issues** di GitHub.
Per modifiche al codice, aprire una **Pull Request**.

---

## 👤 Autore

**Sebastiano Basile**
[superscuola.com](https://www.superscuola.com) · 3° I.C. Capuana-de Amicis — Avola (SR)
🌐 [www.3iccapuana.edu.it](https://www.3iccapuana.edu.it)

[![Contributo volontario](https://img.shields.io/badge/Offrimi_un_caffè_☕-PayPal-blue)](https://paypal.me/superscuola)
