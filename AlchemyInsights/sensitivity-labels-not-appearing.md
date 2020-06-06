---
title: Le etichette di riservatezza non vengono visualizzate
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: df64022f6ad684e2af3eac080068536b7a167b74
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581019"
---
# <a name="sensitivity-labels-not-appearing"></a>Le etichette di riservatezza non vengono visualizzate

Le etichette di riservatezza consentono di classificare e proteggere i contenuti sensibili. Possono essere creati in Microsoft 365 Compliance Center, Microsoft 365 Security Center o Microsoft 365 Security & Compliance Center in Classification > Sensitivity labels. Per ulteriori informazioni su questa funzionalità, vedere [Overview of Sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Se le etichette di riservatezza sono state configurate ma non vengono visualizzate nelle app Microsoft 365, controllare quanto segue:

- Verificare che l'etichetta di riservatezza sia stata [pubblicata](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) per gli utenti e i gruppi desiderati.

- Verificare che l'utente stia utilizzando un'app che supporta le etichette di riservatezza: vedere [etichette di riservatezza nel documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Se si sta [eseguendo la migrazione delle etichette di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), tenere conto delle considerazioni riportate di [seguito](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Supporto per la prevenzione della perdita di dati (DLP): attualmente, solo le etichette di conservazione possono essere utilizzate come condizione nei criteri DLP.  Il supporto per le etichette di riservatezza in un criterio DLP non è ancora disponibile, ma ci stiamo lavorando.

- Quando la crittografia è abilitata su un'etichetta di riservatezza, è possibile scegliere di:
    - Assegnare le autorizzazioni adesso
    - Consentire agli utenti di assegnare le autorizzazioni


Per ulteriori informazioni sui possibili problemi, vedere [problemi noti relativi alle etichette di riservatezza](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).