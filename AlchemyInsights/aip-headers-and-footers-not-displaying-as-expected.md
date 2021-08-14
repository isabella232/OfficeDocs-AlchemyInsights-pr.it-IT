---
title: 'AIP: intestazioni e piè di pagina non visualizzate come previsto'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: e3a0e5caccba87ddd8e4c786b5c8918494e709b6f4d5d60e7c31215a60b1d5d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951785"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: intestazioni e piè di pagina non visualizzate come previsto

Se si verificano problemi con i contrassegni visivi non visualizzati come previsto, vedere le seguenti linee guida:

1. Verificare di aver controllato [Quando vengono applicati i contrassegni visivi](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Per l’etichettatura di Office, controllare [Quando Office 365 applica il contrassegno di contenuto e la crittografia](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).
3. Se si vogliono rimuovere le intestazioni e i piè di pagina esistenti, controllare [Rimuovere intestazioni e piè di pagina da altre soluzioni di etichettatura](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).

Se i problemi persistono, è possibile raccogliere i log del client di Azure Information Protection e allegare i log esportati al ticket.

**Esportare i log di Azure Information Protection**

1. Aprire un documento di Office o creare un nuovo messaggio di posta elettronica in Outlook.
2. Fare clic su **Protezione/Riservatezza** > **Guida e feedback**.
3. Fare clic su **Esporta log**.
4. Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.

Per altre informazioni, vedere:

- [Come configurare un'etichetta per contrassegni visivi di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Consultare la documentazione di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisiti di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Guida introduttiva per Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Scaricare il client di Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
