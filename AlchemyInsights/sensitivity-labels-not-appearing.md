---
title: Etichette di riservatezza non visualizzate
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061436"
---
# <a name="sensitivity-labels-not-appearing"></a>Etichette di riservatezza non visualizzate

Le etichette di riservatezza consentono di classificare e proteggere i contenuti sensibili. Possono essere creati nel Centro sicurezza Centro conformità Microsoft 365, Microsoft 365 & o nel Centro sicurezza Microsoft 365 conformità in Classificazione > Etichette di riservatezza. Per ulteriori informazioni su questa funzionalità, vedere [Panoramica delle etichette di riservatezza.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Se hai configurato le etichette di riservatezza ma non vengono visualizzate nelle app Microsoft 365, controlla quanto segue:

- Verificare che l'etichetta di riservatezza sia stata [pubblicata](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) per gli utenti e i gruppi desiderati.

- Verificare che l'utente utilizzi un'app che supporta le etichette di riservatezza. Vedere [etichette di riservatezza nel documento.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Se si esegue la [migrazione delle etichette di Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)tenere presenti le considerazioni [elencate qui.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Supporto per la prevenzione della perdita dei dati ( DLP): attualmente, solo le etichette di conservazione possono essere utilizzate come condizione nei criteri DLP.  Il supporto per le etichette di riservatezza in un criterio DLP non è ancora disponibile, ma ci stiamo lavorando.

- Quando la crittografia è abilitata su un'etichetta di riservatezza, puoi scegliere tra:
    - Assegnare le autorizzazioni adesso
    - Consentire agli utenti di assegnare le autorizzazioni


Per ulteriori informazioni sui possibili problemi, vedere [Problemi noti con le etichette di riservatezza.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)