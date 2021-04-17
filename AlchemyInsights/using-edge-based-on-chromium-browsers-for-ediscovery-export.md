---
title: Utilizzo di Microsoft Edge basato sui browser Chromium per l'esportazione di Ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834375"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Utilizzo di Microsoft Edge basato sui browser Chromium per l'esportazione di Ediscovery

A causa di una modifica recente, i browser Microsoft Edge non ClickOnce il supporto per impostazione predefinita. Per continuare a usare lo strumento di esportazione di eDiscovery di Microsoft 365, è necessario utilizzare Microsoft Internet Explorer o abilitare il supporto ClickOnce in Microsoft Edge. 

Per abilitare ClickOnce supporto in Microsoft Edge in base a Chromium: 
1. Nel browser Microsoft Edge, visitare edge://flags/#edge-click-once.
2. Per l'opzione ClickOnce Support (Supporto ClickOnce) cambiare il valore da **Default** (Predefinito) o **Disabled** (Disabilitato) a **Enabled** (Abilitato). 
3. Nella parte inferiore della finestra del browser selezionare **Riavvia**. <br>
 La modifica avrà effetto dopo il riavvio di Microsoft Edge. 

Per informazioni su questo e sulla procedura per l'installazione dello strumento di esportazione, vedere: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).