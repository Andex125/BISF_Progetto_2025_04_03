# BUSINESS INTELLIGENCE PER I SERVIZI FINANZIARI  
## Progetto di Laboratorio in Python  
**Versione del 3 aprile 2025**  
*antonio.candelieri@unimib.it*  
*silvio.bencini@unimib.it*

---

## 1. Informazioni Generali

Il progetto è finalizzato a mostrare le capacità acquisite in:
- acquisizione dei dati;
- visualizzazione;
- analisi esplorativa delle serie;
- analisi esplorativa di portafoglio;
- previsione di rendimenti.

Utilizzando le librerie Python introdotte nei laboratori (`pandas`, `matplotlib`, `numpy`, `scikit-learn`, `statsmodels`, ecc.). È possibile usare altre librerie compatibili con Python ≥ 3.8.  
**Il progetto è individuale.**

---

## 2. Dati da Utilizzare

Lo studente può scegliere tra:
- Almeno 6 **azioni** del mercato USA (S&P 500), rappresentative di 3 settori diversi, con scelta basata su notizie finanziarie.
- Almeno 6 **ETF settoriali** (S&P500 o simili come MSCI USA).

**Periodo da analizzare:**  
`31/05/2014 – 31/05/2024`

---

## 3. Documenti di Progetto

Da produrre:
- Jupyter Notebook con codice commentato;
- Presentazione (PowerPoint) da 10–15 minuti;
- Relazione completa con i seguenti capitoli:

  1. Sommario dei dati utilizzati
  2. Statistiche descrittive
  3. Analisi di previsione
  4. Beta di ciascun titolo
  5. Creazione portafoglio o simulazione strategia dinamica
  6. Conclusioni

**Scadenza:** una settimana prima della data dell’esame.  
**Invio a:**  
- silvio.bencini@unimib.it  
- antonio.candelieri@unimib.it

---

## 4. Schema del Documento Finale

### 1. Sommario dei Dati Utilizzati
- Descrizione dei titoli/ETF selezionati e motivazione;
- Funzioni per download dati (es. Yahoo Finance, Fama-French);
- Unione dati in un DataFrame;
- Visualizzazione grafica e anteprima dati.

### 2. Statistiche Descrittive
- Rendimento cumulato e annuo;
- Rendimenti semplici e logaritmici + grafico;
- Analisi: correlazioni, anomalie, eventi fuori media;
- Grafici diagnostici (istogramma, boxplot, QQ-plot);
- Statistiche annualizzate: media, varianza, deviazione, asimmetria, curtosi;
- Matrici di varianza/covarianza e correlazione;
- Scatter plots tra titoli/ETF e indice.

### 3. Analisi di Previsione
- Modello ARIMA:
  - 80 mesi: training
  - 30 mesi: test
  - 10 mesi: previsione (anche ricorsiva)
  - Confronto previsione vs. dati reali
  - Calcolo errore medio

### 4. Strategie di Trading e Backtesting – Analisi Tecnica
- Strategia con algoritmo per segnali buy/sell;
- Confronto con strategia “Buy & Hold”;
- (Opzionale) uso di variabili esogene (volume, VIX, Google Trends, ecc.)

### 5. CAPM
- Calcolo beta rispetto all’indice (`^GSPC`);
- Rendimento atteso (usando beta, rendimento atteso S&P500, T-Bill);
- Esposizione ai fattori di rischio Fama-French.

### 6. Strategie di Trading e Backtesting – Strategie Dinamiche
- Simulare una strategia fra:
  - Equal Weight
  - Stop Loss
  - CPPI
  - TPPI
- Confronto con “Buy & Hold”
- Discussione parametri e miglioramenti

### 7. Costruzione di Portafoglio
- Portafoglio ottimale (media-varianza), con 108 mesi di dati:
  - Metodo analitico e simulativo
  - Uso di rendimenti storici e attesi
- Calcolo beta del portafoglio
- Confronto portafoglio ottimale vs. portafoglio effettivo (peso uguale)

> ⚠️ **Nota:** i punti 6 e 7 sono alternativi.

---

