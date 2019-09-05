---
title: Le etichette di riservatezza non vengono visualizzate
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: eea2d28b754ec87289984068b9e3330b9f10dd5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36744825"
---
# <a name="sensitivity-labels-not-appearing"></a>Le etichette di riservatezza non vengono visualizzate

Le etichette di riservatezza consentono di classificare e proteggere i contenuti sensibili. Per ulteriori informazioni su questa funzionalità, vedere [Overview of Sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Se le etichette di riservatezza sono state configurate ma non vengono visualizzate nelle app di Office, controllare quanto segue:

- Verificare che l'etichetta di riservatezza sia stata [pubblicata](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) per gli utenti e i gruppi desiderati.

- Verificare che l'utente stia utilizzando un'app che supporta le etichette di riservatezza: vedere [etichette di riservatezza nel documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Se si sta [eseguendo la migrazione delle etichette di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenere conto delle considerazioni riportate di [seguito](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Supporto per la prevenzione della perdita di dati (DLP): attualmente, solo le etichette di conservazione possono essere utilizzate come condizione nei criteri DLP.  Il supporto per le etichette di riservatezza in un criterio DLP non è ancora disponibile, ma ci stiamo lavorando.

Per ulteriori informazioni sui possibili problemi, vedere [problemi noti relativi alle etichette di riservatezza](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).