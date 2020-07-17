---
title: Informazioni sull'identità in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146774"
---
# <a name="about-identity-in-yammer"></a>Informazioni sull'identità in Yammer

È consigliabile eseguire la procedura seguente per evitare problemi correlati all'identità:

1. Applicare l'identità di Office 365 dopo il provisioning degli account di Microsoft 365 per gli utenti in Azure AD per assicurarsi che tutti gli utenti accedano usando il proprio account di Microsoft 365 primario. Per alte informazioni, vedere [Applicare l'identità di Office 365 per gli utenti di Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Consolidare più reti di Yammer. Le configurazioni legacy di Yammer consentono la connessione di più reti Yammer a un unico tenant. Per ulteriori informazioni, vedere [Migrazione di rete: consolidare più reti Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. È anche possibile applicare la licenza di Yammer per impedire agli utenti di Yammer che non dispongano di una licenza. Per ulteriori informazioni, vedere [Gestire le licenze utente di Yammer in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Infine, controllare l'elenco degli utenti per le reti Yammer precedenti e sospendere gli utenti legacy. È consigliabile sospendere gli utenti, anziché eliminarli, perché l'eliminazione è irreversibile. Per altre informazioni, vedere [Controllare gli utenti di Yammer nelle reti connesse a Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) e [Rimuovere gli utenti](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Configurando Yammer con questa procedura, è anche possibile configurare la rete Yammer per la modalità nativa di Microsoft 365. Per ulteriori informazioni, vedere [Configurare la rete Yammer per la modalità nativa di Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).