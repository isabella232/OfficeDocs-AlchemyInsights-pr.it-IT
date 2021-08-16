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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056494"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Si sta ricevendo l'errore "Non è stato possibile trovare una cassetta postale per" in Outlook sul web?

Se si utilizza Outlook sul web e non è possibile trovare una cassetta postale per errore, **l'account** utilizzato per connettersi a Outlook sul web non dispone di una licenza Exchange Online e pertanto non è associata alcuna cassetta postale all'account. L'amministratore può assegnare una licenza all'account seguendo questa procedura:

1. Aprire il [interfaccia di amministrazione di Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e passare a **Utenti attivi** nella **sezione Utenti** e selezionare l'utente che sta visualizzato l'errore.

2. Nella pagina utente visualizzata passare  alla sezione Licenze e  app, selezionare il valore percorso appropriato e assegnare una licenza che contiene Exchange Online (espandere la licenza per visualizzarne i dettagli). Al termine, fai clic su **salvare le modifiche**.

In alcuni casi, se la licenza è già assegnata a un account utente, la rimozione e la riassegnazione della licenza consentono di risolvere il problema e di eseguirne il provisioning nel sistema: 

- Verificare se le sottoscrizioni M365 Exchange Online (e altre, se disponibili) sono correnti e non sono scadute di recente.

Dopo aver verificato che l'abbonamento non è scaduto e che all'account utente sia stata assegnata una licenza valida, il provisioning della licenza può richiedere fino a 24 ore, quindi potrebbe essere necessario attendere la risoluzione del problema. Per altre info, vedi [Assegnare e gestire le licenze.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)