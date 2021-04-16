---
title: OneDrive for Business Web OneDrive reindirizza a Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799993"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Reindirizzato a Delve dopo aver fatto clic su OneDrive

Vedi la nostra guida dettagliata [alla risoluzione dei problemi.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Per risolvere il problema, l'amministratore deve concedere agli utenti il diritto di creare il sito siti personali. Ciò è dovuto al fatto che la pagina di OneDrive for Business viene creata nei siti personali.

Per concedere questo diritto, attenersi alla seguente procedura:

1. Nell'interfaccia di amministrazione di SharePoint fare clic **su profili utente.**

2. Nella sezione **Utenti** fare clic **su Gestisci autorizzazioni utente.**

3. Aggiungere gli utenti che richiedono autorizzazioni per creare il sito siti personali. Per impostazione predefinita, questa impostazione è impostata su **Tutti tranne gli utenti esterni.**

4. Dopo aver aggiunto l'utente, gli utenti o il gruppo, assicurarsi che l'utente, gli utenti o il gruppo aggiunto sia selezionato, scorrere fino alla sezione autorizzazioni e quindi selezionare la casella di controllo accanto a Crea sito personale (necessario per l'archiviazione  **personale, il newsfeed** e il contenuto seguito) .

5. Fare **clic su OK** e quindi fare in modo che l'utente navigare alla pagina di OneDrive per creare il sito.
