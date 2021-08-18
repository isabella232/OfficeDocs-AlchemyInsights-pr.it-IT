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
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331127"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificare l'attività delle regole di Posta in arrivo nei log di controllo

È possibile utilizzare la ricerca nei log di controllo nel Centro conformità Microsoft 365 per visualizzare gli eventi delle regole di Posta in arrivo (creazione, modifica ed eliminazione di regole di Posta in arrivo).

1. Eseguire uno dei seguenti passaggi:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività**: selezionare uno o più dei valori seguenti:
     - **New-InboxRule Crea regola di posta in arrivo da Outlook Web App**
     - **Set-InboxRule Modifica la regola da Outlook Web App**.
     - **Aggiornare le regole della posta in arrivo Outlook client**

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. Le informazioni sulle impostazioni delle regole di Posta in arrivo vengono visualizzate nel **campo** Parametri.

Per ulteriori informazioni, vedere [Determining if a user created an Inbox rule](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
