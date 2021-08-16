---
title: Assegnare un ruolo del log di audit nel Centro sicurezza e conformità di Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 5ddfda8687fe3ae2467ad221c7c083f46239826e23b10b91732ea06fd4649f3e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54006174"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Assegnare un ruolo del log di audit nel Centro sicurezza e conformità di Office 365

Per eseguire ricerche nel log di controllo di Office 365, è necessario che a un amministratore sia stato assegnato il ruolo relativo ai **Log di audit di sola lettura** o il ruolo relativo ai **Log di audit** in Exchange Online. Questi ruoli vengono assegnati ai gruppi di ruoli Gestione conformità e Gestione organizzazione per impostazione predefinita. Gli amministratori globali di Office 365 e Microsoft 365 vengono aggiunti automaticamente come membri del gruppo di ruoli Gestione organizzazione.

Per abilitare un utente a eseguire ricerche con il livello minimo di privilegi, creare un gruppo di ruoli personalizzato in Exchange Online, aggiungere il ruolo relativo ai **Log di controllo di sola lettura** o ai **Log di controllo** e quindi aggiungere l'utente come membro del nuovo gruppo di ruoli.

Per altre informazioni, vedere [Gestire i gruppi di ruoli in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) e [Eseguire ricerche nel log di controllo nel Centro sicurezza e conformità](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).