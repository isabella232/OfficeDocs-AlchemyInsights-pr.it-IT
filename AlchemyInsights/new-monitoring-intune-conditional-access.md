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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417317"
---
# <a name="monitor-intune-conditional-access"></a>Monitorare l'accesso condizionale di Intune

Gli utenti con accesso condizionale riceveranno un messaggio di posta elettronica di notifica se non soddisfano i requisiti di accesso dell'organizzazione. Per risolvere il problema, è consigliabile utilizzare una o più delle soluzioni seguenti:

1. Se si presume che il dispositivo sia registrato, consigliare all'utente di passare all'app Portale aziendale e verificare che venga visualizzato nel portale aziendale. In caso contrario, l'utente deve registrare il dispositivo.
1. Nel portale di Azure passare a **Conformità dei dispositivi**  >  **di** Intune. 
1. Per visualizzare il report di conformità del dispositivo per verificare che il dispositivo dell'utente sia contrassegnato come conforme, in **Monitoraggio** fare clic su **Conformità dispositivo.**
1. Nel portale di Azure passare a **Conformità dei dispositivi**  >  **di** Intune. In **Gestisci fare clic** su **Criteri.** Nell'elenco dei criteri di conformità, verificare che un profilo sia assegnato al dispositivo dell'utente. Se non è assegnato alcun profilo, Intune non sarà in grado di confermare lo stato di conformità del dispositivo.
1. Modificare l'assegnazione di accesso condizionale dell'utente.
1. Nel portale di Azure passare a Criteri di accesso condizionale di **Intune,** selezionare un criterio dall'elenco e fare clic  >    >  su Utenti **e gruppi.**
1. Per impostare un determinato criterio come destinatario, aggiungerlo **all'elenco Includi.** Per assicurarsi che una persona sia omessa dal criterio, aggiungerla **all'elenco Escludi.**

**Collegamenti utili:**

- [Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Risoluzione dei problemi dell'autorità di certificazione](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Criteri per la risoluzione dei problemi](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitoraggio della conformità dei dispositivi Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Questi passaggi sono utili solo per la risoluzione dei problemi relativi alla funzionalità accesso condizionale di Azure Active Directory. È anche possibile mettere in quarantena un dispositivo che blocca l'accesso alla posta elettronica con i criteri di Exchange. Ulteriori informazioni sulla gestione dei dispositivi di Exchange sono disponibili [**qui.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
