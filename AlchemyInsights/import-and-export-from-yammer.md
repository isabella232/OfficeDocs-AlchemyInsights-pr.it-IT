---
title: Importare ed esportare da Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: 3ead2702c2fbd26b2e5596e26e9189c2f97baf93c93ec3cbd57f15c855b5128e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54001476"
---
# <a name="import-and-export-from-yammer"></a>Importare ed esportare da Yammer

**Importare**

Le opzioni di importazione utente variano a seconda che la rete Yammer sia disponibile o meno in [Modalità nativa per Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).

- **Modalità non nativa**: per importare gli utenti nei gruppi è necessario usare [Aggiungi dalla rubrica](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (massimo 100 utenti) nelle impostazioni del gruppo; per importare gli utenti nella rete, è invece necessario usare [Aggiorna in blocco](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) in Amministrazione rete.
- **Modalità nativa**: le operazioni di iscrizione a gruppi o reti devono essere eseguite dal [portale di amministrazione di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), dal [portale di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) oppure usando un'altra opzione di AD. Le reti in modalità nativa non hanno più accesso all'opzione Aggiorna in blocco e ad altre funzionalità legacy.

> [!IMPORTANT]
> Yammer non supporta mai l'importazione di contenuti da Amministrazione rete, neanche se la funzionalità di esportazione dati è stata usata in un'altra rete. I contenuti possono essere ripubblicati da soluzioni dei partner o dalle API REST di Yammer.

**Esportare**

L'opzione [Esporta i dati della rete in Amministrazione rete](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) consente di esportare contenuti da reti Yammer, inclusi messaggi e file. Poiché gli allegati possono essere di dimensioni notevoli, il completamento delle esportazioni potrebbe richiedere molto tempo. È consigliabile esportare le reti attive usando l'[API di esportazione dati](https://developer.yammer.com/docs/data-export-api) in blocchi giornalieri o settimanali. Il supporto tecnico Microsoft non fornisce script personalizzati per eseguire queste operazioni.

È disponibile un'apposita [esportazione GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) per esportare i contenuti per un singolo utente.