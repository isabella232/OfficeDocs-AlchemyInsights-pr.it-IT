---
title: Problemi nell'aprire o scaricare file in Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146818"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problemi nell'aprire o scaricare file in Yammer

Classic Yammer supporta più opzioni per caricare i file in messaggi e gruppi. A seconda della configurazione della rete, per impostazione predefinita i file vengono archiviati in SharePoint.

La selezione file nel nuovo Yammer non supporta ancora tutte le opzioni disponibili nella versione classica di Yammer. Un aggiornamento futuro aggiungerà altre funzionalità. Per altre informazioni, vedere [Allegare un file o un'immagine a un post di conversazione di Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Non è possibile aprire o scaricare un file**  

Un file può essere caricato in Yammer, ma è anche possibile creare un collegamento a un file in SharePoint Online. Per risolvere il problema, è necessario prima di tutto determinare il percorso del file. Se il file è stato caricato in Yammer, avrà un URL *. yammer.com. Assicurarsi che gli URL e gli indirizzi IP necessari vengano sbloccati. Per altre informazioni, vedere il post di blog [Usare gli indirizzi IP hardcoded per Yammer non è consigliabile](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Verificare se un utente che è anche un amministratore globale può scaricare il file. Se il file è privato, potrebbe essere necessario usare la Modalità contenuto privato. Per altre informazioni, vedere [Monitorare il contenuto privato in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Guest e file di Yammer a livello di rete in SharePoint Online**  

[Gli utenti Guest a livello di rete in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) non usano Azure AD B2B e sono interni al servizio Yammer, quindi non possono accedere ai file di Yammer archiviati in SharePoint. Creare un utente AAD B2B esterno che possa accedere alle raccolte documenti in SharePoint Online usando tale identità. Per informazioni sul supporto futuro per guest di Azure AD B2B in Yammer, vedere [Supporto business-to-business (B2B) nell'anteprima di Yammer: condizioni per i clienti e domande frequenti](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).