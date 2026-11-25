# Verificatore di SEO Mobile ed Ergonomia Smartphone

[![Test SEO Mobile](https://img.shields.io/badge/TAVARDT-Mobile%20SEO-5b3cf5.svg)](https://tools.tavardt.com/it/test-seo-mobile-google/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Audit di conformita mobile-first, configurazione del tag viewport, larghezze rigide, leggibilita dei caratteri ed ergonomia touch.

***

## Vettori di Rischio e Impatto Operativo nell Esperienza Mobile

I siti privi di una corretta dichiarazione del viewport falliscono l indicizzazione mobile-first di Google e subiscono pesanti cali organici in Italia. Errori di impaginazione responsive forzano lo scorrimento orizzontale e allontanano gli utenti.

Bloccare lo zoom dell utente viola gli standard internazionali di accessibilita e penalizza chi necessita di ingrandire i contenuti. Larghezze fisse superiori allo schermo e testi troppo piccoli incrementano la frequenza di rimbalzo.

***

## Funzionalita Centrali di Audit Tecnico

* **Analisi della Direttiva Viewport**: Verifica la presenza del tag meta, l adattamento alle dimensioni del dispositivo e il blocco dello zoom, deducendo fino a 45 punti se mancante.
* **Rilevamento dello Scorrimento Orizzontale**: Individua elementi CSS con larghezza fissa oltre 450px che provocano lo sforamento visivo su smartphone.
* **Audit di Leggibilita Tipografica**: Segnala dimensioni di testo inferiori a 12px, applicando penalita fino a 15 punti per contenuti illeggibili.
* **Quantificazione dei Punti di Tocco**: Mappa link, bottoni e campi modulo per valutare l ergonomia e la corretta spaziatura su display touch.
* **Validazione dell Icona Touch (Apple Touch Icon)**: Accerta la configurazione dell icona dedicata nella testata HTML, deducendo 5 punti se non rilevata.
* **Valutazione di Ergonomia Mobile**: Calcola un punteggio da 0 a 100 categorizzato in SATISFACTORY, ADVISORY o UNSATISFACTORY.
* **Emulazione Smartphone Reale**: Esegue richieste HTTP con l esatto User-Agent di Safari su iPhone per un esame aderente al contesto operativo.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore senza dipendenze esterne aggiuntive.

```bash
git clone https://github.com/TAVARDT-Italia/mobile-seo-tester-it.git
cd mobile-seo-tester-it
python mobile_seo_tester.py https://azienda.it
```

Per generare l output in formato strutturato JSON per pipeline di integrazione continua:

```bash
python mobile_seo_tester.py https://azienda.it -j
```

***

## Domande Frequenti (FAQ Tecnico)

### 1. Quale impatto ha un tag viewport assente o malformato sull indicizzazione mobile?
I motori di ricerca analizzano le pagine web attraverso la simulazione completa di uno schermo per smartphone. In assenza della meta viewport impostata su device-width, la pagina viene mostrata in versione desktop subendo severe penalizzazioni di ranking.

### 2. Per quale motivo viene sanzionato il blocco dello zoom tramite user-scalable=no?
Impedire l ingrandimento manuale ostacola gravemente la fruizione per gli utenti con difficolta visive secondo le linee guida WCAG. Gli algoritmi dei motori considerano questo blocco un grave difetto di usabilita e riducono il punteggio qualitativo.

### 3. Come danneggiano la navigazione mobile i contenitori con larghezza fissa superiore a 450px?
Gli elementi con larghezza fissa oltre 450px oltrepassano i limiti fisici dei display mobili e generano un fastidioso scorrimento laterale. Questo disallineamento distrugge la continuita responsive e porta alla bocciatura nei controlli di idoneita per dispositivi mobili.

### 4. Quali rischi comportano le definizioni di testo inferiori a 12px?
I caratteri piu piccoli di 12px risultano faticosi da decifrare sui display ad alta risoluzione degli smartphone. L analisi applica detrazioni di punteggio per assicurare che i testi principali siano fruibili senza dover ricorrere a ingrandimenti continui.

### 5. Perche e determinante dichiarare l icona apple-touch-icon nel codice sorgente?
L attributo apple-touch-icon consente ai dispositivi mobili di mostrare un icona nitida e personalizzata quando il portale viene aggiunto alla schermata home. L omissione genera icone segnaposto di bassa qualita che sminuiscono l identita visiva aziendale.

***

## Consulenza in SEO Mobile e Architettura Responsive

Per grandi architetture digitali che richiedono la piena conformita a Google Mobile-First Indexing e standard W3C, consultate il team di **TAVARDT**.

***

## Collegamenti Utili

* **Portale Istituzionale:** https://ag.tavardt.com/it/
* **Suite di Diagnostica:** https://tools.tavardt.com/it/
* **Contatto Tecnico:** https://ag.tavardt.com/it/contatto/

***

### Licenza
Distribuito sotto Licenza MIT. Consultare il file LICENSE per i dettagli completi.

***

© 2026 TAVARDT. Tutti i diritti riservati.
