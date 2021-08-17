---
title: Identificare l'attività delle regole di Posta in arrivo nei log di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891299"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificare l'attività delle regole di Posta in arrivo nei log di controllo

È possibile utilizzare la ricerca nei log di controllo nel Centro conformità Microsoft 365 per visualizzare gli eventi delle regole di Posta in arrivo (creazione, modifica ed eliminazione di regole di Posta in arrivo).

1. Esegui uno dei seguenti passaggi:
   - Nell'Centro conformità Microsoft 365 <https://compliance.microsoft.com> in , passare a **Soluzioni** \> **Controllo**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://compliance.microsoft.com/auditlogsearch> .
   - Nel portale di Microsoft 365 Defender <https://security.microsoft.com> all'indirizzo , passare a **Controlla**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://security.microsoft.com/auditlogsearch> .

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - **Attività**: selezionare uno o più dei valori seguenti:
     - **New-InboxRule Crea regola di posta in arrivo da Outlook Web App**
     - **Set-InboxRule Modifica la regola da Outlook Web App**.
     - **Aggiornare le regole della posta in arrivo Outlook client**

3. Al termine, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova **pagina Di ricerca di** controllo.

4. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. Le informazioni sulle impostazioni delle regole di Posta in arrivo vengono visualizzate nel **campo** Parametri.

Per ulteriori informazioni, vedere [Determining if a user created an Inbox rule](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
