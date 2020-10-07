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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366432"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitoraggio dell'accesso condizionale per Exchange

Gli utenti a cui viene assegnato l'accesso condizionale ricevono un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il testo, è consigliabile eseguire una o più delle soluzioni seguenti:

- Se si presume che il dispositivo venga registrato, avvisare l'utente di accedere all'app portale aziendale e verificare che venga visualizzato nel portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Monitor fare clic su conformità dispositivo. Visualizzare il rapporto di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Gestisci fare clic su criteri. Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente. Se non è stato assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.
- Modificare l'assegnazione di accesso condizionale dell'utente.

1. Nel portale di Azure passare ai **Intune**  >  criteri di**accesso condizionale**di Intune  >  **Policies**.
2. Selezionare un criterio dall'elenco.
3. Fare clic su utenti e gruppi.
4. Per assegnare un determinato criterio a un utente, aggiungerli all'elenco Includi. Per assicurarsi che una persona venga omessa dal criterio, aggiungerla all'elenco Escludi.

Collegamenti utili:

[Panoramica della conformità del dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi relativi all'autorità di certificazione](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Risoluzione dei problemi relativi ai criteri](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoraggio della conformità del dispositivo Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: questi passaggi sono utili solo per la risoluzione dei problemi relativi all'accesso condizionale delle funzionalità di Azure Active Directory. È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange. Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [qui](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
