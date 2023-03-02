---
keywords: adobe experience cloud;Adobe Experience Cloud;device co-op;Device Co-op;fine del ciclo di vita
title: “Domande frequenti sulla fine del ciclo di vita di [!DNL Device Co-op]”
description: Scopri i piani di fine del ciclo di vita di Device Co-op.
exl-id: 015ba95c-0c8d-415e-969c-b8670494de98
source-git-commit: 180dd414dd0b595518f54cddc5b02ed06ecc0b16
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 95%

---

# Domande frequenti sulla fine del ciclo di vita di [!DNL Device Co-op]

Questo documento fornisce le risposte alle domande più frequenti sul piano di fine del ciclo di vita (EOL) di [!DNL Adobe Experience Cloud Device Co-op]. Quando questo piano entrerà in vigore, Adobe fornirà un avviso avanzato sulle [Note sulla versione di Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=it) e [Aggiornamento prioritario del prodotto](https://www.adobe.com/it/subscription/priority-product-update.html).

[!DNL Device Co-op] è stato un programma che consentiva ai partecipanti di collaborare per identificare meglio i consumatori in diversi punti di contatto digitali, garantendo al contempo il massimo livello di privacy e trasparenza.

## Domande frequenti

Di seguito è riportato un elenco di risposte alle domande frequenti relative al piano EOL di [!DNL Device Co-op].

## Perché [!DNL Device Co-op] è obsoleto?

Le imminenti modifiche nell’ambiente AdTech trasformeranno [!DNL Device Co-op] in una soluzione obsoleta nei prossimi anni. [!DNL Device Co-op] è composto per lo più da cookie di terze parti e l’annuncio di [!DNL Google's] che bloccherà i cookie di terze parti su [!DNL Google Chrome] entro il 2022 diminuirà l&#39;efficacia di [!DNL Device Co-op]. [!DNL Chrome] ha circa il 65% della quota di mercato del browser e altri principali browser hanno già implementato il blocco dei cookie di terze parti. Una volta che [!DNL Chrome] blocca i cookie di terze parti, la maggior parte dei cookie di terze parti verrà bloccata e [!DNL Device Co-op] sarà reso obsoleto.

## Perché Adobe cessa le registrazioni a [!DNL Device Co-op]?

Le registrazioni cessano per evitare il rischio di non soddisfare le aspettative dei clienti a causa dei prossimi cambiamenti del settore rispetto ai cookie di terze parti. [!DNL Device Co-op] impiega alcuni mesi per essere preparato e alcuni altri mesi per estrarre valore dal servizio. Qualsiasi ulteriore iscrizione a questo punto potrebbe comportare che i marchi non godano del pieno valore di [!DNL Device Co-op].

## A luglio 2022, Google ha annunciato la proroga della rimozione dei cookie di terze parti da Chrome al 2024. Questo influisce sui piani EOL di [!DNL Device Co-op]?

No, i piani EOL di [!DNL Device Co-op] di Adobe continueranno a rimanere invariati e non saranno prorogati.

## Possono registrarsi nuovi clienti?

A partire dall’11 giugno 2021, Adobe non accetterà più nuove registrazioni a [!DNL Device Co-op].

## Vengono rinnovati i contratti esistenti?

A partire dall’11 giugno 2021, Adobe non rinnoverà più i contratti [!DNL Device Co-op]. Se desideri continuare a utilizzare i servizi di [!DNL Device Co-op], puoi continuare a farlo in base ai termini della licenza corrente fino al termine del programma.

## Qual è la data di fine esatta del programma di [!DNL Device Co-op]?

Il programma di [!DNL Device Co-op] terminerà nel 2022. Il periodo e la data specifici dipendono da quando [!DNL Google] inizierà a bloccare i cookie di terze parti. I lavori di disattivazione dovrebbero iniziare nel settembre 2022.

## Quali applicazioni saranno influenzate dalla fine del ciclo di vita di Device Co-op?

Le seguenti applicazioni sono influenzate dalle procedure di fine vita di [!DNL Device Co-op]:

- [[!DNL Adobe Analytics]](https://experienceleague.adobe.com/docs/analytics.html?lang=it)
- [[!DNL Adobe Audience Manager]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/overview/aam-overview.html?lang=it)
- [[!DNL Adobe Advertising Cloud]](https://experienceleague.adobe.com/docs/advertising-cloud.html?lang=it)
- [[!DNL Adobe Target]](https://experienceleague.adobe.com/docs/target/using/introduction/intro.html?lang=it)

## Quali opzioni ho in alternativa a [!DNL Device Co-op]?

### [!DNL Analytics]

È possibile utilizzare [!DNL Analytics] [Cross-Device Analytics (CDA)](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html?lang=it) in quanto supporta sia il servizio Adobe Experience Platform Identity [Grafico privato](https://experienceleague.adobe.com/docs/analytics/components/cda/device-graph.html?lang=it) e [Unione basata sui campi](https://experienceleague.adobe.com/docs/analytics/components/cda/field-based-stitching.html?lang=it).

### [!DNL Audience Manager]

[!DNL Audience Manager] mantiene le integrazioni con partner grafici per dispositivi di terze parti, tra cui [!DNL LiveRamp] e [!DNL Tapad], anche se è necessario stabilire relazioni commerciali con i partner grafici direttamente, al fine di sfruttare [!DNL Audience Manager]. Tutti i clienti devono aggiornare le regole di unione profili Co-op per utilizzare opzioni diverse da [!DNL Device Co-op.]

### [!DNL Real-time Customer Data Platform]

Non sono previsti piani per modificare l&#39;attuale [!DNL Audience Manager Data Management Platform] (DMP). Tuttavia, l’obsolescenza dei cookie di terze parti probabilmente creerà problemi di scala per la maggior parte degli utenti DMP. Per aiutare i clienti a sviluppare le proprie pratiche di gestione dei dati, Adobe incoraggia la riduzione delle dipendenze dagli identificatori che verranno limitati nel prossimo anno. I team di marketing devono creare strategie per i dati di prime parti incentrate su identificatori durevoli che includono informazioni personali identificabili (PII) e che possono essere risolte con [!DNL Real-time Customer Data Platform] (Real-Time CDP).

[!DNL Real-time CDP] riduce le dipendenze da cookie di terze parti e da ID dispositivo espandendo il set di identificatori disponibili perché la creazione di un pubblico includa i PII. Alla base di [!DNL Real-time CDP] c’è il Profilo cliente in tempo reale, che riunisce i dati degli attributi delle persone con i dati comportamentali in tempo reale e consente agli esperti di marketing di creare segmenti di pubblico avanzati con controlli di governance dei dati brevettati. Come [!DNL Audience Manager], [!DNL Real-time CDP] fornisce informazioni approfondite e casi d’uso di personalizzazione, ma genera anche informazioni più dettagliate a livello di utente e può attivare il pubblico in una gamma più ampia di destinazioni che vanno da tecnologie pubblicitarie a tecnologie di marketing, compresi i paid media, i social media, le e-mail e i sistemi del cliente.

[!DNL Real-time CDP] includerà anche l’accesso a [Corrispondenza segmento Adobe Experience Platform (Beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=it), che consente ai brand di espandere i propri set di dati di prime parti tramite partnership e ottenere informazioni e personalizzazioni migliorate.

### [!DNL Target]

Non sono attualmente disponibili alternative per [!DNL Target] perché [!DNL Target] fornisce una funzionalità deterministica di unione delle identità tra dispositivi nota come `mbox3rdPartyId`, che funziona in modo simile all’ID cliente di Adobe. Questa funzionalità consente ai clienti di [!DNL Target] di unire profili e partecipazione all’attività tramite test e personalizzazione di [!DNL Target] eseguiti nei canali in entrata.

### Adobe Advertising Cloud

I clienti di [!DNL Advertising Cloud] non potranno più utilizzare [!DNL Device Co-op] per il targeting e la misurazione di tipi di pubblico tra dispositivi. Con [!DNL Advertising Cloud], sarà comunque possibile sfruttare la collaborazione di [!DNL Device Graph] di Adobe con [!DNL LiveRamp] per continuare a svolgere queste funzioni per quanto rientra nelle capacità e scalabilità di [!DNL LiveRamp's]. Devi lasciar terminare le campagne che utilizzano [!DNL Device Co-op], quindi passare al fornitore di grafici dei dispositivi [!DNL LiveRamp] o non sfruttare più il targeting basato sugli individui.

## Quali funzionalità e implementazioni esistenti possono aiutare la mia preparazione a un futuro senza cookie?

L’implementazione del servizio ID visitatore esistente potenzia Analytics [CDA](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html?lang=it). Se l’ID dichiarato esistente è un’e-mail con hash, può essere utilizzato per abilitare le seguenti funzionalità:

- [!DNL Audience Manager] [Destinazioni basate su persone](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/people-based/people-based-destinations-overview.html?lang=it).
- [Corrispondenza segmento di Experience Platform (beta)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match/overview.html?lang=it).

## Riuscirò a conservare i miei dati da [!DNL Device Co-op]?

Per gli utenti [!DNL Audience Manager] e [!DNL Advertising Cloud], i dati da [!DNL Device Co-op] non saranno disponibili per essere trasferiti a grafici di terze parti. I dati di [!DNL Device Co-op] verranno migrati solo per gli utenti [!DNL Analytics Ultimate] che utilizzano CDA con [!DNL Device Co-op] che passa all’unione basata sul campo. Tutte le altre soluzioni non effettueranno la migrazione dei dati.

## È obbligatorio adottare altre funzionalità?

Anche se l’adozione di altre funzionalità di Adobe non è obbligatoria, è necessario avviarne l’implementazione il prima possibile per avere a disposizione il tempo e un coordinamento adeguato prima che [!DNL Device Co-op] diventi obsoleto.

## Entro quando devo adottare soluzioni alternative, se scelgo di farlo?

L’adozione di altre funzionalità non è obbligatoria. Lo consigliamo solo se desideri continuare a gestire i casi di utilizzo per i quali utilizzavi [!DNL Device Co-op]. Se scegli di adottare altre funzionalità, devi farlo entro il 2022 (il momento esatto non è stato annunciato) prima del termine del programma [!DNL Device Co-op].

## Quanto tempo ci vorrà per l’adozione?

Questo dipenderà dalla funzionalità. Ad esempio, se un cliente Analytics Ultimate che utilizza Analytics tra dispositivi con [!DNL Device Co-op] desidera migrare al grafico in tempo reale per il dispositivo privato oppure all’unione basata sul campo, l’adozione richiederà un po’ di tempo.

## E per quanto riguarda [!UICONTROL Persone] metrica?

Con l&#39;esclusione del [!DNL Device Co-op], il [!UICONTROL Persone] La metrica non è più rilevante. Nel prossimo futuro (data da definire), rimuoveremo il [!UICONTROL Persone] metrica. A questo punto, i dati verranno reindirizzati al [!UICONTROL Visitatore univoco] in Analytics per evitare che progetti, segmenti e metriche calcolate si interrompano.

