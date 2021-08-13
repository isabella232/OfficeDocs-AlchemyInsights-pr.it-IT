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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975105"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitoraggio dell'accesso condizionale per Exchange

Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il problema, è consigliabile una o più delle soluzioni seguenti:

- Se si presume che il dispositivo sia registrato, avvisa l'utente di passare all'app Portale aziendale e verificare che venga visualizzato nella Portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Monitor fai clic su Conformità dispositivo. Visualizza il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme.
- Nel portale di Azure passare a Intune > conformità del dispositivo. In Gestisci fare clic su Criteri. Nell'elenco dei criteri di conformità, verificare che al dispositivo dell'utente sia assegnato un profilo. Se non viene assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.
- Modificare l'assegnazione di accesso condizionale dell'utente.

1. Nel portale di Azure passare a **Criteri**  >  **di accesso condizionale di** Intune  >  .
2. Selezionare un criterio dall'elenco.
3. Fare clic su Utenti e gruppi.
4. Per scegliere come destinazione un determinato criterio presso un utente, aggiungerlo all'elenco Includi. Per assicurarsi che una persona sia omessa dal criterio, aggiungerla all'elenco Escludi.

Collegamenti utili:

[Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi relativi a CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Criteri di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitoraggio della conformità dei dispositivi intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Nota: questi passaggi sono utili solo per la risoluzione dei problemi Azure Active Directory accesso condizionale. È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con Exchange criteri. Altre informazioni sulla Exchange dei dispositivi sono disponibili [qui]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
