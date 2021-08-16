---
title: Monitorare l'accesso condizionale di Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025506"
---
# <a name="monitor-intune-conditional-access"></a>Monitorare l'accesso condizionale di Intune

Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il problema, è consigliabile una o più delle soluzioni seguenti:

1. Se si presume che il dispositivo sia registrato, avvisa l'utente di passare all'app Portale aziendale e verificare che venga visualizzato nella Portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
1. Nel portale di Azure passare a **Conformità dei dispositivi**  >  **intune**. 
1. Per visualizzare il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme, in **Monitor** fare clic su **Conformità dispositivo.**
1. Nel portale di Azure passare a **Conformità dei dispositivi**  >  **intune**. In **Gestisci fare clic** su **Criteri.** Nell'elenco dei criteri di conformità, verificare che al dispositivo dell'utente sia assegnato un profilo. Se non viene assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.
1. Modificare l'assegnazione di accesso condizionale dell'utente.
1. Nel portale di Azure, accedere a Criteri di accesso condizionale di **Intune,** selezionare un  >    >  criterio dall'elenco e fare clic su **Utenti e gruppi.**
1. Per impostare come destinazione un determinato criterio presso un utente, aggiungerli **all'elenco Includi**. Per assicurarsi che una persona sia omessa dal criterio, aggiungerla **all'elenco Escludi**.

**Collegamenti utili:**

- [Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Risoluzione dei problemi relativi a CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Criteri di risoluzione dei problemi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitoraggio della conformità dei dispositivi intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Questi passaggi sono utili solo per la risoluzione dei problemi della Azure Active Directory accesso condizionale. È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con Exchange criteri. Altre informazioni sulla Exchange dei dispositivi sono disponibili [**qui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
