---
title: OneDrive for Business Web OneDrive reindirizza a approfondire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571214"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Reindirizzato a approfondire dopo aver fatto clic su OneDrive

Consultare la [Guida alla risoluzione dei problemi](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)dettagliata.

Per risolvere il problema, l'amministratore di Office 365 deve concedere agli utenti il diritto di creare il sito personale. Ciò è dovuto al fatto che la pagina di OneDrive for business viene creata nei siti personali.

Per concedere questo diritto, eseguire la procedura seguente:

1. Nell'interfaccia di amministrazione di SharePoint, fare clic su **profili utente**.

2. Nella sezione **utenti** fare clic su **Gestisci autorizzazioni utente**.

3. Aggiungere gli utenti che richiedono le autorizzazioni per creare il sito di siti personali. Per impostazione predefinita, questa impostazione è impostata su **tutti tranne gli utenti esterni**.

4. Dopo aver aggiunto l'utente, gli utenti o il gruppo, assicurarsi che l'utente, gli utenti o il gruppo aggiunto siano selezionati, scorrere fino alla sezione **autorizzazioni** e quindi selezionare la casella di controllo accanto a **Crea sito personale (obbligatorio per l'archiviazione personale, newsfeed e contenuto seguito)**.

5. Fare clic su **OK**, quindi passare alla pagina OneDrive per creare il sito.
