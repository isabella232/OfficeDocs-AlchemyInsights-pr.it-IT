---
title: Problemi relativi alle prestazioni-SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511152"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti

Se un sito di OneDrive o di SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo. [Controllare il dashboard dell'integrità dei servizi](https://portal.office.com/adminportal/home#/servicehealth).

**Aggiungere e concedere una licenza all'utente**

Assicurarsi [di assegnare le licenze agli utenti in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Assegnare le autorizzazioni**

Se all'utente è stata assegnata una licenza di SharePoint ed è ancora in ricezione un messaggio di accesso negato, assicurarsi che disponga del [livello di autorizzazione appropriato](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assegnato.

**Valutare la possibilità di utilizzare la funzionalità di richiesta di accesso**

La [funzionalità di richiesta di accesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) consente agli utenti di richiedere l'accesso ai contenuti che attualmente non dispongono dell'autorizzazione per la vista.

**Consenti lo script personalizzato può causare problemi di accesso negato**

Esistono alcuni scenari in cui la caratteristica *Consenti script personalizzato* potrebbe presentare un accesso negato. Per un elenco delle caratteristiche coinvolte, considerazioni sulla sicurezza e la possibilità di disabilitare la funzionalità. Visitare [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

