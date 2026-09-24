---
title: Fine del ciclo di vita dell’API Adobe Analytics 1.4
description: L’autenticazione API Adobe Analytics 1.4 e WSSE ha raggiunto la fine del ciclo di vita il 31 agosto 2026. Scopri cosa è interessato e come effettuare la migrazione alle API di Analytics 2.0.
source-git-commit: 4056ba0953e81a279d25b15449c7b41a4a5eb7f9
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 1%
---
# Fine del ciclo di vita dell’API Adobe Analytics 1.4

A decorrere dal **31 agosto 2026**, Adobe ha ritirato l&#39;autenticazione API Adobe Analytics 1.4 e WSSE. Tutti gli endpoint che utilizzano questa versione dell’API non sono più accessibili e le integrazioni basate su di essa non funzionano più.

Le API di Adobe Analytics 1.4 hanno fornito un’ampia gamma di azioni, come reporting, classificazioni, feed di dati, segmenti, metriche calcolate, origini dati e configurazione della suite di rapporti. Sono state sostituite dalle [API di Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0), che ti consentono di eseguire quasi tutte le azioni disponibili nell&#39;interfaccia utente di Adobe Analytics, incluso il reporting e la gestione di componenti come segmenti e metriche calcolate. Se hai un&#39;integrazione che deve ancora essere aggiornata, segui la guida per [Migrazione alle API di Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/guides/migration).

## Cosa ha raggiunto la fine del ciclo di vita

Questa fine del ciclo di vita influisce direttamente sulle seguenti funzionalità API 1.4. Esegui la migrazione di ogni flusso di lavoro interessato alle [API di Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0):

* Generazione rapporti (inclusi rapporti Data Warehouse, in tempo reale, percorsi e di riepilogo)
* Configurazione e amministrazione della suite di rapporti
* Classificazioni
* Segmenti
* Metriche calcolate
* Origini dati
* Feed dati
* Segnalibri e metodi aziendali (endpoint)

Ritira anche l&#39;**autenticazione Adobe Analytics WSSE** (vedi [autenticazione WSSE](#wsse-authentication) di seguito).

>[!IMPORTANT]
>
>Questa fine del ciclo di vita *non* influisce sulla raccolta dati. Non influisce sulle soluzioni di assegnazione tag come Tag (precedentemente Adobe Launch), Web SDK e AppMeasurement. Anche l&#39;API di inserimento dati [1&rbrace; è *non* ritirata. &#x200B;](#data-insertion-api)Tuttavia, se utilizzi le API di origini dati o classificazioni 1.4 per migliorare i dati, devi migrare tali flussi di lavoro alle API di Adobe Analytics 2.0.

## Autenticazione WSSE

L’autenticazione WSSE è un protocollo di autenticazione legacy supportato dalle API di Analytics 1.4. È stato sostituito dalle opzioni di autenticazione basate su OAuth fornite in [Adobe Developer Console](https://developer.adobe.com/console/home). I progetti che utilizzano l’autenticazione WSSE devono aggiornare le proprie credenziali a quelle fornite in Adobe Developer Console.

Per eseguire la migrazione, accedi a [Adobe Developer Console](https://developer.adobe.com/console/home) e crea un progetto per l&#39;integrazione API di Analytics 2.0. Selezionare il metodo di autenticazione **Utente OAuth** o **Server-to-Server OAuth**.

## API di inserimento dati

L&#39;API di inserimento dati è **not** parte di questa fine del ciclo di vita. La relativa documentazione è stata spostata nel sito [API di raccolta dati di Adobe Analytics](https://developer.adobe.com/analytics-collection-apis/), insieme agli altri metodi di raccolta lato server:

* [API di inserimento dati](https://developer.adobe.com/analytics-collection-apis/methods/data-insertion/): invia i dati evento un hit alla volta, come stringa di query (richiesta immagine) o XML `POST`.
* [API di inserimento dati in blocco](https://developer.adobe.com/analytics-collection-apis/methods/bulk-data-insertion/): carica batch di dati di chiamata al server come file. Per le nuove implementazioni lato server, Adobe consiglia di utilizzare l’API di inserimento dati in blocco.

## Domande frequenti

+++Questo influisce sui miei progetti Adobe Developer esistenti per le API di Analytics?

Sono interessati tutti i progetti esistenti che utilizzano le API di Analytics 1.4. È necessario migrare tali integrazioni alle [API di Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/).

+++

+++Ho condiviso le mie credenziali di Adobe con un altro prodotto o applicazione che utilizza le API di Analytics. Sono interessati?

Il prodotto o l’applicazione che utilizza le credenziali WSSE o chiama le API di Analytics 1.4 ne risente e deve eseguire la migrazione. Rivolgiti al fornitore del prodotto o dell’applicazione per informazioni dettagliate sui piani di migrazione e sulla tempistica.

+++

+++Come posso determinare quale API utilizza il mio progetto?

L’URL di base chiamato dal progetto determina la versione API utilizzata. Le API di Adobe Analytics 1.4 utilizzavano i seguenti URL di base:

* `https://api.omniture.com`
* `https://api3.omniture.com`
* `https://api4.omniture.com`
* `https://api5.omniture.com`

Le [API di Adobe Analytics 2.0](https://developer.adobe.com/analytics-apis/docs/2.0/) utilizzano il seguente URL di base:

* `https://analytics.adobe.io`

Se uno dei tuoi progetti API chiama `api*.omniture.com`, utilizza le API Adobe Analytics 1.4 ritirate e deve effettuare la migrazione alle API 2.0.

+++

+++Questa fine del ciclo di vita influisce sulla raccolta dei dati?

No. Questa fine del ciclo di vita **non** influisce sulla raccolta diretta dei dati, ad esempio Tags, Web SDK, AppMeasurement o l&#39;API di inserimento dati. Tuttavia, se utilizzi le API di origini dati o classificazioni 1.4 per migliorare i dati, devi migrare tali flussi di lavoro alle API di Adobe Analytics 2.0.

+++

Se hai ulteriori domande su questa fine del ciclo di vita a cui non hai risposto in questa pagina, contatta il tuo Adobe Account Team.
