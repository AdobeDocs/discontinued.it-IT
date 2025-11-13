---
title: Test nascosto
description: Questo è un test nascosto
hide: true
hidefromtoc: true
landing-page-breadcrumb-title: Test AEM 6.5
landing-page-name: experience-manager-65
feature: Annotations
exl-id: e6e5ba1c-98a5-4d7d-9913-426df31bc7a3
source-git-commit: dde6a1c269865b6baec6e073a25a3dbd817d3d07
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# Test nascosto

Questo è un test nascosto. Sto aggiungendo `[` per assicurarmi che funzioni correttamente nel rendering v2.

12 novembre 2025

## Test video

### Video normale senza trascrizione: dovrebbe mostrare la trascrizione perché metadata.md è in discesa

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true)

### Con trascrizione impostata su true

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=true}

### Con la trascrizione impostata su false: la trascrizione video non deve essere visualizzata

>[!VIDEO](https://video.tv.adobe.com/v/332116?hidetitle=true){transcript=false}

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

