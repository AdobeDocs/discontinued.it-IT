---
keywords: Device-graph;fine del ciclo di vita
title: Device Graph
description: Scopri i piani di fine del ciclo di vita per il grafico dei dispositivi.
source-git-commit: 6d27883347049957d35070dd5c5bf5b223144470
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 2%

---

# Fine del grafico dei dispositivi

>[!WARNING]
>
>Il grafico dei dispositivi in Analytics tra dispositivi non è più disponibile dal **31 dicembre 2025**. Cambiare qualsiasi suite di rapporti virtuali abilitata per Device Graph al [metodo basato sui campi](https://experienceleague.adobe.com/en/docs/analytics/components/cda/field-based-stitching).

Analytics tra dispositivi ha utilizzato Private Graph per unire i dati. Private Graph è un archivio di ID dispositivo con hash specifico per la tua organizzazione. CDA comunica regolarmente con il grafico dei dispositivi per collegare i dispositivi.

## Prerequisiti specifici per il grafico dei dispositivi

Se intendevi implementare Analytics tra dispositivi utilizzando il metodo del grafico dei dispositivi, erano necessari i seguenti elementi.

>[!WARNING]
>
>Il mancato rispetto di tutti i prerequisiti potrebbe comportare l’impossibilità di abilitare Cross-Device Analytics o risultati errati durante l’unione dei dati.

* L&#39;organizzazione deve utilizzare il [grafo privato del servizio Adobe Experience Platform Identity](https://business.adobe.com/products/experience-platform/identity-service.html). Vedi anche la [home page](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html) nella guida utente del servizio Identity.
* L&#39;implementazione deve utilizzare la versione più recente del servizio Experience Cloud ID (ECID). Consulta la [home page](https://experienceleague.adobe.com/docs/id-service/using/home.html) nella guida utente del servizio ID. È probabile che il servizio ID sia già stato distribuito per la maggior parte delle implementazioni che utilizzano [Tag](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=it) in Adobe Experience Platform.
* L&#39;implementazione deve chiamare la funzione `setCustomerIDs` (o equivalente a SDK) ogni volta che un utente può essere identificato, ad esempio quando un utente effettua l&#39;accesso o apre un messaggio e-mail. Questo requisito si applica a tutte le piattaforme, incluse le app mobili se utilizzate. Vedi [`setCustomerIDs`](https://experienceleague.adobe.com/docs/id-service/using/id-service-api/methods/setcustomerids.html) nella guida utente del servizio ID.

## Limitazioni specifiche del grafico dei dispositivi

* Gli ID legacy di Analytics non sono supportati. Solo i visitatori con Experience Cloud ID sono uniti.
* Se l’organizzazione utilizza un grafico privato, i nuovi dispositivi richiedono fino a 24 ore per essere uniti.
* I grafici dei dispositivi di terze parti non sono supportati.
