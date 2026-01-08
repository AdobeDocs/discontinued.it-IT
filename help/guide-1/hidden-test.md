---
title: Test nascosto
description: Questo è un test nascosto
hide: true
hidefromtoc: true
landing-page-breadcrumb-title: Test AEM 6.5
landing-page-name: experience-manager-65
feature: Annotations
exl-id: e6e5ba1c-98a5-4d7d-9913-426df31bc7a3
source-git-commit: d246aa050c2e8304709fadaddf93a6b70a661b82
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 3%

---

# Test nascosto

8 gennaio - Bob

Questo è un test nascosto. Sto aggiungendo `[` per assicurarmi che funzioni correttamente nel rendering v2.

## Apri in una nuova scheda {#section_92882928}

`[See What's new](auditor.md){target="_blank"} `

[Apri nella stessa scheda](auditor.md)

[Nuova scheda con spazio tra virgolette](auditor.md){target="_blank"} 

[Nuova scheda con ancoraggio](auditor.md){target=_blank}

[Nuova scheda senza spazio tra virgolette](auditor.md){target="_blank"}

[Nuova scheda con spazio senza virgolette](auditor.md){target=_blank} 

[Nuova scheda senza spazio senza virgolette](auditor.md){target=_blank}

[Nuova scheda con collegamento profondo](commerce-channels.md#channel-manager-extension){target="_blank"}

[Ancoraggio nuova scheda con collegamento profondo](https://experienceleague.adobe.com/it/docs/analytics/analyze/home#key-analytics-resources){target="_blank"}

[Nuova scheda con collegamento esterno](https://www.adobe.com){target="_blank"}

[Nuovo collegamento directory principale scheda](/help/guide-1/auditor.md){target="_blank"}


<table>
  <tr>
    <th>Con virgolette</a></th>
    <th>Senza virgolette</th>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com" target="_blank">Nuova scheda di Adobe</a></td>
    <td><a href="https://www.adobe.com" target="_blank">Nuova scheda di Adobe</td>
  </tr>
  <tr>
    <td><a href="https://www.adobe.com">Adobe senza nuova scheda</a></td>
    <td><a href="https://www.adobe.com">Adobe senza nuova scheda</td>
  </tr>
</table>

## Test commento

18 novembre 2025

<!-- ## Comment with basic text

This is a new line.

Second new line. -->


Commenta qui sotto. Se questa è l’ultima cosa che vedi in questo articolo, è dovuto alla sintassi del commento.

1. Fai clic su **[!UICONTROL Crea]**.

<!-- ## Create an exclusion using Advanced Search

You can also create exclusions using [!UICONTROL Advanced Search] on the [Catalog Search](/help/main/c-recommendations/c-products/catalog-search.md#save-as) page ( [!UICONTROL Recommendations] > [!UICONTROL Catalog Search] > [!UICONTROL Advanced Search]). 

![Save as dialog](/help/main/c-recommendations/c-products/assets/save-as.png)

After creating a search using "id > contains," for example, you can then click [!UICONTROL Save As] > [!UICONTROL Exclusion].

>[!IMPORTANT]
>
>The [!UICONTROL Advanced Search] functionality is case-insensitive; however, products returned at the time of delivery are based on case-sensitive search. This mismatch might lead to confusion. Ensure that you consider case-sensitivity when you create exclusions based on results using the Advanced Search functionality. For example, if you perform a search for "Holiday," that initial search lists results containing "Holiday" and "holiday." If you then create an exclusion with the intent to exclude products containing "holiday," only products containing "holiday" are excluded. Products containing "Holiday" are not excluded. -->

Questa riga è dopo il commento.

## Test video

### Video normale senza trascrizione: dovrebbe mostrare la trascrizione perché metadata.md è in discesa

>[!VIDEO](https://video.tv.adobe.com/v/3409659?captions=ita&hidetitle=true)

### Con trascrizione impostata su true

>[!VIDEO](https://video.tv.adobe.com/v/3409659?captions=ita&hidetitle=true){transcript=true}

### Con la trascrizione impostata su false: la trascrizione video non deve essere visualizzata

>[!VIDEO](https://video.tv.adobe.com/v/3409659?captions=ita&hidetitle=true){transcript=false}

## Collegamenti relativi

* [Panoramica](overview.md)
* [Cerca e promuovi](search-promote.md)
* [Social](social.md)

## Collegamento profondo esplicito

[panoramica aggiuntiva (root)](/help/guide-1/overview.md#additional-products)

[panoramica aggiuntiva](overview.md#additional-products)

## Test testo al passaggio del mouse {#this-is-a-heading-anchor}

Nessun testo al passaggio del mouse

```
![alt text](assets/maui-flip.jpg)
```

![testo alternativo](assets/maui-flip.jpg)


Sì al passaggio del mouse

```
![alt text](assets/maui-flip.jpg "Hover text")
```

![Testo alternativo](assets/maui-flip.jpg "Testo al passaggio del mouse")

## Diapositiva

Sintassi:

```
>[!SLIDE](analyze-project)
https://experienceleague-stage.adobe.com/en/slides/analyze-project
```

Rendering:

<!--
>[!SLIDE](analyze-project)
-->

Bob: rimuovi il commento della diapositiva dopo aver verificato l’elemento relativo alla posizione dell’argomento.

