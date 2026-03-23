---
title: About
layout: about
permalink: /about.html
---

{% include feature/jumbotron.html objectid="croce-desiderio" %}

{% include feature/nav-menu.html sections="Il Progetto;Metodologia;Criteri di Selezione;Struttura dei Metadati;Tecnologie;Fonti e Bibliografia;Autore" %}

## Il Progetto

**Mille** è una biblioteca digitale dedicata alla documentazione e alla valorizzazione delle arti decorative del Medioevo italiano. La collezione raccoglie oggetti museali — gioielli, tessuti, smalti, vetri — conservati presso musei e istituzioni culturali italiane, descrivendoli attraverso schede strutturate con metadati uniformi.

Il nome *Mille* evoca il primo millennio della cultura europea e il Medioevo come periodo di straordinaria produzione artigianale e artistica, spesso sottorappresentato rispetto al Rinascimento. La biblioteca vuole restituire visibilità a questi oggetti, rendendoli accessibili a un pubblico ampio attraverso un'interfaccia digitale sobria e navigabile.

Il progetto è stato realizzato nell'ambito del corso di **Informatica Umanistica** (Università di Bologna) e si propone come applicazione pratica dei principi delle Digital Humanities applicati al dominio del patrimonio culturale museale.

### Obiettivi

- Costruire una collezione digitale strutturata di oggetti delle arti decorative medievali italiane
- Rendere accessibili e navigabili i metadati descrittivi degli oggetti museali
- Sperimentare i principi dell'architettura dell'informazione applicata al patrimonio culturale
- Pubblicare la risorsa sul Web tramite GitHub Pages in formato bilingue (italiano/inglese)

---

## Metodologia

Il progetto ha seguito le fasi classiche del **project management plan**: brief, benchmark, documento di progetto, produzione, sviluppo, testing e pubblicazione.

Per ogni oggetto è stata definita una struttura di metadati uniforme, derivata dagli standard catalografici museali italiani (ICCD — Istituto Centrale per il Catalogo e la Documentazione) e adattata al formato richiesto da CollectionBuilder-GH. I campi includono: denominazione, datazione, tipologia, materiali e tecnica, dimensioni, museo di conservazione, numero di inventario, provenienza e fonti bibliografiche.

La scelta di CollectionBuilder-GH come framework di pubblicazione risponde all'obiettivo di massimizzare l'accessibilità e l'interoperabilità della risorsa: il sito è statico, pubblicato su GitHub Pages, e i metadati sono scaricabili in formato CSV e JSON dalla sezione [Data]({{ '/data.html' | relative_url }}).

---

## Criteri di Selezione

La selezione dei quattro oggetti inclusi nella collezione è stata guidata da criteri espliciti, con l'obiettivo di rappresentare la pluralità delle arti decorative medievali italiane senza pretesa di esaustività.

**A — Arco cronologico medievale**
Tutti gli oggetti sono databili tra il IX e il XIV secolo, coprendo sia l'Alto che il Basso Medioevo italiano.

**B — Diversità di tipologie e materiali**
La selezione copre quattro categorie distinte: oreficeria gemmata, altare in smalto cloisonné, tessile ricamato, vetro soffiato smaltato. Questo permette alla collezione di funzionare come campionario rappresentativo delle arti decorative del periodo.

**C — Conservazione presso musei italiani pubblici**
Tutti gli oggetti sono conservati presso istituzioni museali italiane pubbliche o ecclesiastiche, con documentazione catalografica verificabile.

**D — Disponibilità di fonti primarie verificabili**
Per ciascun oggetto esistono fonti primarie verificabili — siti dei musei, cataloghi scientifici, monografie — che garantiscono l'accuratezza delle informazioni nelle schede.

**E — Rilevanza storico-artistica**
Gli oggetti selezionati sono considerati dalla letteratura scientifica come esempi significativi della produzione artistica medievale italiana, citati nei principali manuali di storia dell'arte medievale.

---

## Struttura dei Metadati

Ogni oggetto nella collezione è descritto attraverso i seguenti campi, conformi alle linee guida di CollectionBuilder-GH e agli standard catalografici ICCD:

| Campo | Descrizione |
|---|---|
| `objectid` | Identificatore univoco dell'oggetto (slug) |
| `title` | Denominazione convenzionale dell'oggetto |
| `filename` | Nome del file immagine associato |
| `date` | Datazione (formato AAAA) |
| `description` | Descrizione estesa dell'oggetto |
| `subject` | Soggetti e parole chiave (separati da punto e virgola) |
| `location` | Città del museo di conservazione |
| `latitude` / `longitude` | Coordinate geografiche del museo |
| `source` | Museo e città di conservazione |
| `creator` | Autore o manifattura dell'oggetto |
| `museo` | Nome esteso del museo |
| `materiali` | Materiali e tecnica di produzione |
| `tipologia` | Categoria tipologica dell'oggetto |
| `periodo` | Periodo storico (Alto/Basso Medioevo) |
| `rights` | Informazioni sul copyright |

I metadati sono disponibili per il download nella sezione [Data]({{ '/data.html' | relative_url }}) in formato CSV e JSON.

---

## Tecnologie

Il sito è realizzato con **CollectionBuilder-GH**, un framework open source sviluppato dall'Università dell'Idaho per la creazione di biblioteche digitali leggere su GitHub Pages.

- **CollectionBuilder-GH** — framework di pubblicazione
- **GitHub Pages** — hosting statico gratuito con controllo versione
- **Jekyll** — generatore di siti statici (usato internamente da CollectionBuilder)
- **Bootstrap** — framework CSS per il layout responsive (integrato in CollectionBuilder)
- **Leaflet.js** — libreria per la mappa interattiva (integrata in CollectionBuilder)

Il sito è interamente statico: non richiede database, server o CMS. Tutti i dati sono contenuti nel file CSV e nel repository GitHub, garantendo la massima portabilità e longevità della risorsa.

Il codice sorgente è disponibile pubblicamente su [GitHub](https://github.com).

---

## Fonti e Bibliografia

### Fonti primarie (musei)

- **Museo di Santa Giulia, Brescia** — [museidibrescia.it](https://www.museidibrescia.it)
- **Basilica di Sant'Ambrogio, Milano** — [basilicasantambrogio.it](https://www.basilicasantambrogio.it)
- **Museo del Tesoro del Duomo, Vercelli** — [tesorodelduomo.vercelli.it](https://www.tesorodelduomo.vercelli.it)
- **Museo Nazionale del Bargello, Firenze** — [bargellomusei.beniculturali.it](https://www.bargellomusei.beniculturali.it)

### Manuali di riferimento del corso

- F. Tomasi, *Metodologie informatiche e discipline umanistiche*, Carocci, Roma 2008, cap. 1–5
- F. Tomasi, *Organizzare la conoscenza: Digital Humanities e Web semantico*, Editrice Bibliografica, Milano 2022, cap. 1 e 6

### Letteratura scientifica

- P. Williamson, *Medieval Ivory Carvings: Early Christian to Romanesque*, V&A Publishing, London 2010
- M. M. Gauthier, *Émaux du Moyen Âge occidental*, Office du Livre, Fribourg 1972
- C. Frugoni (a cura di), *Il Medioevo sulle nasi*, Il Mulino, Bologna 2001

### Risorse digitali

- **Europeana** — [europeana.eu](https://www.europeana.eu) — aggregatore europeo del patrimonio culturale digitale
- **ICCD — Istituto Centrale per il Catalogo e la Documentazione** — [iccd.beniculturali.it](https://www.iccd.beniculturali.it)
- **CollectionBuilder Documentation** — [collectionbuilder.github.io/cb-docs](https://collectionbuilder.github.io/cb-docs)

---

## Autore

Questo sito è stato realizzato come progetto finale del corso di **Informatica Umanistica**, Università di Bologna, anno accademico 2025–2026.

**Corso:** Informatica Umanistica  
**Docente:** Prof.ssa Francesca Tomasi  
**Università:** Alma Mater Studiorum — Università di Bologna  
**Anno accademico:** 2025–2026  

Il codice sorgente e i metadati sono disponibili pubblicamente su [GitHub](https://github.com) con licenza aperta.
