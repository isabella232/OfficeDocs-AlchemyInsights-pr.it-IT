---
title: Monitoraggio dell'accesso condizionale
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708678"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitoraggio dell'accesso condizionale per Exchange

Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il problema, è consigliabile utilizzare una o più delle soluzioni seguenti:

- Se si presume che il dispositivo sia registrato, consigliare all'utente di passare all'app Portale aziendale e verificare che venga visualizzato nel portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Monitoraggio fare clic su Conformità dispositivo. Visualizzare il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Gestisci fare clic su Criteri. Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente. Se non viene assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.
- Modificare l'assegnazione di accesso condizionale dell'utente.

1. Nel portale di Azure passare a **Criteri di accesso** condizionale  >  **di**  >  Intune.
2. Selezionare un criterio dall'elenco.
3. Fare clic su Utenti e gruppi.
4. Per impostare come destinazione un determinato criterio presso un utente, aggiungerlo all'elenco Includi. Per assicurarsi che una persona sia omessa dal criterio, aggiungerla all'elenco Escludi.

Collegamenti utili:

[Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi dell'autorità di certificazione](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Criteri per la risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoraggio della conformità dei dispositivi Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: questi passaggi sono utili solo per la risoluzione dei problemi relativi alla funzionalità accesso condizionale di Azure Active Directory. È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange. Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [qui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
