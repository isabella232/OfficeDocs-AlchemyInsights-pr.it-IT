---
title: Informazioni sull'identità in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664174"
---
# <a name="about-identity-in-yammer"></a>Informazioni sull'identità in Yammer

È consigliabile eseguire la procedura seguente per evitare problemi correlati all'identità:

1. Applicare l'identità di Office 365 dopo il provisioning degli account di Microsoft 365 per gli utenti in Azure AD per assicurarsi che tutti gli utenti accedano usando il proprio account di Microsoft 365 primario. Per alte informazioni, vedere [Applicare l'identità di Office 365 per gli utenti di Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Consolidare più reti di Yammer. Le configurazioni legacy di Yammer consentono la connessione di più reti Yammer a un unico tenant. Per ulteriori informazioni, vedere [Migrazione di rete: consolidare più reti Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. È anche possibile applicare la licenza di Yammer per impedire agli utenti di Yammer che non dispongano di una licenza. Per ulteriori informazioni, vedere [Gestire le licenze utente di Yammer in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Infine, controllare l'elenco degli utenti per le reti Yammer precedenti e sospendere gli utenti legacy. È consigliabile sospendere gli utenti, anziché eliminarli, perché l'eliminazione è irreversibile. Per altre informazioni, vedere [Controllare gli utenti di Yammer nelle reti connesse a Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Rimuovere gli utenti](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Configurando Yammer con questa procedura, è anche possibile configurare la rete Yammer per la modalità nativa di Microsoft 365. Per ulteriori informazioni, vedere [Configurare la rete Yammer per la modalità nativa di Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).