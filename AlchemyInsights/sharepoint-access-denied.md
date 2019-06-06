---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735742"
---
# <a name="troubleshoot-access-denied-messages"></a>Risoluzione dei problemi relativi ai messaggi di accesso negato

Se si riceve un messaggio di accesso negato quando si tenta di esplorare un sito di SharePoint Online, vedere gli articoli seguenti.

## <a name="add-and-license-the-user"></a>Aggiungere e concedere una licenza all'utente

Assicurarsi [di assegnare licenze agli utenti in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).

Assegnare le autorizzazioni

Se all'utente è stata assegnata una licenza di SharePoint ed è ancora in ricezione un messaggio di accesso negato, assicurarsi che disponga del [livello di autorizzazione appropriato assegnato](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).

Valutare la possibilità di utilizzare la funzionalità di richiesta di accesso

La funzionalità di [richiesta di accesso](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) consente agli utenti di richiedere l'accesso ai contenuti che attualmente non dispongono dell'autorizzazione per la vista. 

Consenti lo script personalizzato può causare problemi di accesso negato

Esistono alcuni scenari in cui la caratteristica "Consenti script personalizzato" può presentare un accesso negato. Per un elenco delle caratteristiche coinvolte, considerazioni sulla sicurezza e la possibilità di disabilitare la funzionalità. Visita, [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)

Nota: se un sito di OneDrive o di SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema di servizio temporaneo. [Controllare il dashboard dell'integrità dei servizi](https://portal.office.com/adminportal/home#/servicehealth).


  

