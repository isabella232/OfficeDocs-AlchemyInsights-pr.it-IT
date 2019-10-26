---
title: 305 aumentare le dimensioni della cassetta postale di archiviazione
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36661804"
---
# <a name="increase-the-archive-mailbox-size"></a>Aumentare le dimensioni della cassetta postale di archiviazione

Office 365 [limita](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) le dimensioni delle cassette postali di archiviazione in base alla licenza assegnata all'account utente. Quando la cassetta postale di archiviazione raggiunge il 90% della dimensione consentita, l'utente riceve una notifica tramite posta elettronica. Quando una cassetta postale di archiviazione raggiunge il limite di dimensione, l'utente non può spostare più elementi nella cassetta postale di archiviazione. Office 365 non aumenterà le dimensioni di una cassetta postale di archiviazione dopo che è stato raggiunto il limite di dimensione. Al contrario, gli utenti possono eseguire le azioni seguenti per liberare spazio nella cassetta postale di archiviazione:

- Esportare gli elementi in un file. pst utilizzando Outlook.

- Eliminare gli elementi dalla cassetta postale di archiviazione.

Office 365 fornisce un' **archiviazione illimitata** per le licenze di Office 365 Enterprise E3 ed E5. Un amministratore deve abilitare questa funzionalità prima che la cassetta postale di archiviazione raggiunga la dimensione massima. Quando l'archiviazione illimitata è abilitata, possono essere necessari fino a 30 giorni prima che lo spazio libero venga aggiunto alla cassetta postale di archiviazione. Pertanto, è consigliabile che gli amministratori verifichino lo spazio disponibile nella cassetta postale di archiviazione, consentendo all'utente di continuare a utilizzare la cassetta postale di archiviazione durante la sua espansione. Per ulteriori informazioni, vedere [Overview of Unlimited Archiving in office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) e [Enable Unlimited Archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Per ulteriori informazioni sull'accesso alla cassetta postale di archiviazione da Outlook, vedere [requisiti di Outlook per l'accesso agli elementi in un archivio con espansione automatica](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Per configurare un criterio di conservazione che consente di spostare automaticamente gli elementi nella cassetta postale di archiviazione, vedere [set up an Archive and Deletion Policy for Mailboxes in your Office 365 Organization](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Nota**: gli archivi di espansione automatica non sono supportati per le cassette postali primarie su Exchange 2010.
