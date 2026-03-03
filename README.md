# 📊 Analisi Sportiva Serie A 2025/26

![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-FF6F00?style=for-the-badge&logo=pandas&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## 🔗 **Apri il file interattivo**
👉 **[Apri il file completo su Google Sheets](https://docs.google.com/spreadsheets/d/1s3lB9q1InfBarTQk0h4Rh0j9BRlNMBouuNawhfRn3no/edit?usp=sharing)**

⚠️ **Nota**: Il file è pubblicato sul web. Per modificarlo:
> 1. Apri il link
> 2. Clicca su **"Apri in Google Fogli"** in alto
> 3. Vai su **File → Crea una copia** e salvalo sul tuo Drive

👉 **[Clicca qui per visualizzare la Dashboard](dashboard.png)**
---

## 📋 **Descrizione del progetto**

Questo progetto contiene un'analisi della **Serie A 2025/26**, con dati aggiornati fino alla 10ª giornata. Il file Google Sheets è strutturato in quattro fogli interconnessi che si aggiornano automaticamente.

### ⚽ **Funzionalità principali**

| Foglio | Descrizione |
|--------|-------------|
| **📅 Dati** | Tutti i risultati delle partite con calcolo automatico dell'esito (1/X/2) |
| **🏆 Classifica** | Classifica dinamica con punti, gol fatti/subiti, vittorie, pareggi, sconfitte |
| **📈 Dashboard** | Statistiche interattive, media gol, prime 5 squadre, confronto testa a testa |
| **⚙️ Config** | Info squadre (allenatori, stadi, capacità) e classifica marcatori |

### 🔍 **Cosa puoi fare**
- ✅ Visualizzare la classifica aggiornata in tempo reale
- ✅ Confrontare due squadre (es. Inter vs Milan)
- ✅ Analizzare la media gol per partita
- ✅ Scoprire la squadra con più punti e più spettatori
- ✅ Consultare la tabella marcatori con medie realizzative

---

## 🛠️ **Competenze dimostrate**

| Competenza | Implementazione |
|------------|-----------------|
| **Formule avanzate** | CONTA.PIÙ.SE, SOMMA.PIÙ.SE, CERCA.VERT, INDICE, CONFRONTA, GRANDE |
| **Dashboard interattiva** | Confronto dinamico tra squadre con validazione dati |
| **Automazione** | Classifica che si aggiorna automaticamente inserendo nuovi risultati |
| **Organizzazione dati** | 4 fogli collegati tra loro con struttura professionale |
| **Pubblicazione web** | File pubblicato e accessibile da chiunque senza login |
---

## 🚀 **Come utilizzare il progetto**

### Per visualizzare (senza account Google):
1. Clicca sul link in alto
2. Esplora i vari fogli e la dashboard

### Per modificare e personalizzare:
1. Apri il link e clicca **"Apri in Google Fogli"**
2. **File → Crea una copia** (salvalo sul tuo Drive)
3. Aggiungi nuove partite nel foglio **"Dati"**
4. Tutto si aggiornerà automaticamente! ✨

---

## 📊 **Struttura del file**

### 📅 Foglio Dati
- **Colonne**: Data, Giornata, Squadra Casa, Squadra Trasferta, Gol Casa, Gol Trasferta, Esito, Spettatori
- **Formula esito**: `=SE(E2>F2;"1";SE(E2<F2;"2";"X"))`

### 🏆 Foglio Classifica
- **Punti**: `=(CONTA.PIÙ.SE(Dati!C:C; B3; Dati!G:G; "1")*3) + (CONTA.PIÙ.SE(Dati!D:D; B3; Dati!G:G; "2")*3) + (CONTA.PIÙ.SE(...))`
- **Gol Fatti**: `=SOMMA.SE(Dati!C:C;B3;Dati!E:E)+(SOMMA.SE(Dati!D:D;B3;Dati!F:F))`
- **Vittorie/Pareggi/Sconfitte**: conteggi condizionali con CONTA.PIÙ.SE

### 📈 Foglio Dashboard
- **KPI principali**: totale partite, media gol, squadra top
- **Classifica prime 5**: con formule GRANDE + INDICE + CONFRONTA
- **Confronto squadre**: CERCA.VERT dinamico

### ⚙️ Foglio Config
- Anagrafica squadre (Allenatore, Stadio, Capacità)
- Classifica marcatori con media gol
