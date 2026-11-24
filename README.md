# Verificatore di SEO Mobile ed Ergonomia Smartphone

[![Test SEO Mobile](https://img.shields.io/badge/TAVARDT-Mobile%20SEO-5b3cf5.svg)](https://tools.tavardt.com/it/test-seo-mobile-google/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Audit di conformita viewport, leggibilita su schermi compatti e compatibilita mobile-first.

Sviluppato e gestito dalla divisione di architettura web di **TAVARDT**.

***

## Funzionalita del Verificatore SEO Mobile

* **Controllo Tag Meta Viewport**: Verifica della direttiva `width=device-width, initial-scale=1` e assenza di restrizioni allo zoom.
* **Ispezione del Layout Responsivo**: Individuazione di elementi rigidi che causano scorrimento orizzontale anomalo su dispositivi mobili.
* **Ergonomia dei Bersagli di Tocco**: Rilevamento di pulsanti e link con area cliccabile insufficiente o spaziatura non conforme.
* **Leggibilita dei Caratteri**: Analisi delle dimensioni del testo per garantire fruibilita immediata su schermi compatti.
* **Punteggio di Conformita Mobile-First**: Valutazione numerica da 0 a 100 con raccomandazioni tecniche mirate.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore senza dipendenze terze.

```bash
git clone https://github.com/TAVARDT-Italia/mobile-seo-tester-it.git
cd mobile-seo-tester-it
python mobile_seo_tester.py https://azienda.it
```

Esportazione in formato strutturato JSON:

```bash
python mobile_seo_tester.py https://azienda.it -json
```

***

## Strumento Ufficiale Online

Esegui un controllo approfondito direttamente via web:

* **Test di SEO Mobile Ufficiale**
* **[Portale Istituzionale TAVARDT](https://ag.tavardt.com/it/)**

***

## Consulenza e Supporto Tecnico

Per ottimizzare la presenza mobile in conformita con Linee Guida AgID di Accessibilita e Standard Google Mobile-First, contattare **TAVARDT**.

***

© 2026 TAVARDT. Tutti i diritti riservati.
