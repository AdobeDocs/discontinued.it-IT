---
title: Domande frequenti sulla fine del ciclo di vita di Adobe Media SDK (versioni 1.x e 2.x)
description: Risposte alle domande frequenti sulla fine del ciclo di vita di Adobe Media SDK versioni 1.x e 2.x (precedentemente Video Heartbeat Library).
source-git-commit: d014c200dd926ccf0116faa50c4bffb1d234e926
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 0%

---


# Domande frequenti sulla fine del ciclo di vita di Adobe Media SDK (versioni 1.x e 2.x)

Adobe Media SDK **2.x ha raggiunto la fine del supporto il 31 agosto 2021**. Video Heartbeat Library (VHL) **1.x è obsoleto** e non è più supportato da diversi anni.

## Cosa succede?

La Video Heartbeat Library (VHL) originale, in seguito rinominata Media SDK, forniva il tracciamento lato client per l’analisi audio e video. Adobe ha convertito le funzionalità di tracciamento in implementazioni più recenti e funzionali:

* **Media SDK 3.x (solo Analytics):** Attualmente supportato. Tiene traccia dei contenuti multimediali utilizzando l’API Media Collection. Consigliato per gli utenti 2.x esistenti che non possono ancora passare ad Edge Network.
* **Streaming Media for Edge Network (consigliato):** L&#39;implementazione corrente consigliata. Utilizza l’API Adobe Experience Platform Web SDK, Mobile SDK o Media Edge per inviare dati multimediali tramite Edge Network, abilitandone l’utilizzo in Adobe Analytics, Customer Journey Analytics, Real-Time CDP e Adobe Journey Optimizer.

## Cosa è incluso nella fine del ciclo di vita e cosa non lo è?

**Fine del ciclo di vita (non più supportata):**

* Video Heartbeat Library (VHL) 1.x — tutte le piattaforme (Android, iOS, JavaScript, Apple TV, Chromecast, Roku, TVML)
* Media SDK 2.x — Android, iOS, JavaScript

**Non termina il ciclo di vita (ancora supportato):**

* Media SDK 3.x — JavaScript, Chromecast, Roku (solo Analytics)
* Streaming Media for Edge Network — tutte le piattaforme supportate

## Perché le versioni 1.x e 2.x sono state ritirate?

A partire dalla versione 3.0, Media SDK è stato riprogettato per utilizzare direttamente l’API Media Collection, eliminando la necessità di un modello delegato e semplificando la creazione del tracker. I precedenti SDK 1.x e 2.x si basavano su un’architettura server heartbeat che da allora è stata sostituita.

Adobe ha inoltre introdotto l’implementazione di Edge Network per fornire una singola pipeline di raccolta dati in grado di alimentare più applicazioni Adobe a valle, che gli SDK heartbeat legacy non potevano supportare.

## Dove posso trovare la documentazione archiviata?

La documentazione legacy è stata archiviata su GitHub ed è disponibile come riferimento:

| Versione | Stato | Documentazione archiviata |
|---|---|---|
| 1.x (Video Heartbeat Library) | Obsoleta | [`video-heartbeat` archivio GitHub](https://github.com/Adobe-Marketing-Cloud/video-heartbeat/tree/master/docs) |
| 2.x (Media SDK) | Fine del supporto 31 agosto 2021 | [`media-sdks` archivio GitHub](https://github.com/Adobe-Marketing-Cloud/media-sdks/blob/master/docs/2.x/README.md) |

## Quali sono le opzioni di transizione?

**Opzione 1: migrazione a Media SDK 3.x (solo Analytics)**

Se utilizzi la versione 2.x e utilizzi esclusivamente Adobe Analytics, la migrazione a 3.x è il percorso più semplice. Per un confronto API completo ed esempi di codice, consulta la [guida alla migrazione da 2.x a 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html).

**Opzione 2: migrazione a Streaming Media per Edge Network (consigliata)**

Per le nuove implementazioni o quando desideri utilizzare i dati in più applicazioni Adobe, utilizza Adobe Experience Platform Edge Network:

* [Media Edge Web SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-web-sdk.html)
* [SDK mobile di Media Edge](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [API di Media Edge](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge-api.html)

## Domande frequenti

+++**Il supporto per gli SDK Roku e Chromecast sarà interessato?**

No. Gli SDK Roku e Chromecast rimangono disponibili e supportati come parte di Media SDK 3.x (solo Analytics). Questa fine del ciclo di vita riguarda solo le versioni 1.x e 2.x.

+++

+++**Le implementazioni di Media Analytics JavaScript SDK saranno interessate?**

No. I clienti che utilizzano JavaScript SDK per Media Analytics possono continuare a utilizzare l’estensione SDK o tag autonoma.

+++

+++**Sono ancora in Media SDK 2.x. Cosa devo fare?**

Per tutti i nuovi progetti, Adobe consiglia di migrare all’implementazione di Edge Network. Se hai bisogno di un passaggio intermedio, [Esegui la migrazione da JavaScript SDK 2.x a 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html), quindi pianifica il passaggio ad Edge Network.

+++

+++**Qual è il livello di impegno per la migrazione a un&#39;implementazione supportata?**

L’impegno di migrazione dipende dall’implementazione di ogni cliente e varia. Dopo aver esaminato la documentazione sulla migrazione, rivolgiti alla consulenza o all’assistenza clienti per richiedere supporto aggiuntivo:

* [Implementare contenuti multimediali in streaming utilizzando Mobile Edge SDK: Android e iOS](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html)
* [Migrazione da JavaScript SDK 2.x a 3.x](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/migrate-js-2x-to-3x.html)

+++

+++**È necessario utilizzare i tag di Adobe Experience Platform come sistema di gestione dei tag?**

Per le implementazioni delle app mobili, i tag di Experience Platform non vengono utilizzati come sistemi di gestione dei tag analogamente a quanto avviene per il web. L’interfaccia utente Tag è necessaria per configurare le estensioni SDK. È simile a come l’interfaccia utente di Adobe Mobile Services è stata utilizzata per configurare il SDK Mobile v4. Tag fornisce istruzioni di installazione personalizzate in base all’estensione scelta.

+++

+++**Questa fine del supporto influisce su SDK per tvOS?**

Sì. Per tvOS (versione 10+) l’implementazione consigliata è quella di migrare a Streaming Media per Edge Network utilizzando Adobe Experience Platform Mobile SDK. Per ulteriori informazioni, vedere [Implementare contenuti multimediali in streaming utilizzando l&#39;Edge SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) per dispositivi mobili.

+++

+++**Questa fine del supporto influisce su SDK per Fire TV e Android TV?**

Sì. Per Fire TV e Android TV, l’implementazione consigliata è quella di migrare a Streaming Media per Edge Network utilizzando Adobe Experience Platform Mobile SDK. Per ulteriori informazioni, vedere [Implementare contenuti multimediali in streaming utilizzando l&#39;Edge SDK](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/edge-mobile-sdk.html) per dispositivi mobili.

+++

+++**Dove posso trovare le informazioni sulla fine del ciclo di vita di Mobile v4 SDK?**

Consulta le [Domande frequenti sulla fine del ciclo di vita di Mobile Services](mobile-services.md). La piattaforma Mobile Services e gli SDK Mobile v4 hanno raggiunto la fine del ciclo di vita il 31 dicembre 2022.

+++

+++**Dove posso andare in caso di domande?**

Contatta il team del tuo account Adobe o l’Assistenza clienti di Adobe per assistenza sulla migrazione.

+++

>[!MORELIKETHIS]
>
>* [Panoramica sull&#39;implementazione di Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/overview.html?lang=it)
>* [Contenuti multimediali in streaming per Edge Network](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/edge/implementation-edge.html?lang=it)
>* [Media SDK 3.x — Installazione di JavaScript](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/media-sdk/setup/web-implementation.html?lang=it)
