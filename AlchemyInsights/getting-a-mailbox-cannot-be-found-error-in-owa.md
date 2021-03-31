---
title: 126 Errore impossibile trovare una cassetta postale in OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426666"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Ottenere un errore di cassetta postale non trovato in Outlook sul Web?

Se si utilizza Outlook sul Web e non è possibile trovare una cassetta postale per errore, **l'account** utilizzato per connettersi a Outlook sul Web non dispone di una licenza di Exchange Online e pertanto nessuna cassetta postale è associata all'account. L'amministratore può assegnare una licenza al tuo account seguendo questi passaggi:

1. Aprire [l'interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e passare **a** Utenti attivi nella sezione Utenti e selezionare l'utente che sta visualizzato l'errore. 

2. Nella pagina utente visualizzata passare  alla sezione Licenze e  app, selezionare il valore percorso appropriato e assegnare una licenza contenente Exchange Online (espandere la licenza per visualizzarne i dettagli). Al termine, fai clic su **salvare le modifiche**.

In alcuni casi, se la licenza è già assegnata a un account utente, la rimozione e la riassegnazione della licenza consentono di risolvere il problema e di eseguirne il provisioning nel sistema: 

- Verificare se le sottoscrizioni M365 Exchange Online (e altre, se disponibili) sono correnti e non sono scadute di recente.

Dopo aver verificato che l'abbonamento non è scaduto e che all'account utente sia stata assegnata una licenza valida, il provisioning della licenza può richiedere fino a 24 ore, quindi potrebbe essere necessario attendere la risoluzione del problema. Per altre info, vedi [Assegnare e gestire le licenze.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)