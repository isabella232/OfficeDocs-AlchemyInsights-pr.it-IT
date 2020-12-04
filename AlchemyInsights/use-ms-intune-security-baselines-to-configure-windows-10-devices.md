---
title: Utilizzare le linee di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571897"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utilizzare le linee di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10

Le previsioni di sicurezza di Intune consentono di proteggere utenti e dispositivi. Le linee di base per la sicurezza sono gruppi preconfigurati delle impostazioni di Windows utilizzati per applicare un gruppo conosciuto di impostazioni e valori predefiniti consigliati dai team di sicurezza rilevanti. Creando un profilo di base di sicurezza in Intune, è possibile creare un modello costituito da più profili di configurazione dei dispositivi.

Quando si distribuiscono le linee di base di sicurezza ai gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi eseguiti in Windows 10 o versioni successive. Ad esempio, la linea di base di sicurezza MDM automaticamente (1) Abilita BitLocker per le unità rimovibili, (2) richiede la password per sbloccare un dispositivo e (3) disattiva l'autenticazione di base. Quando un valore predefinito non funziona per l'ambiente in uso, personalizzare la linea di base per applicare le impostazioni necessarie.

Le linee di base per la sicurezza consentono inoltre di stabilire un flusso di lavoro sicuro end-to-end in Microsoft 365. Di seguito sono riportati alcuni vantaggi:

- Una previsione di sicurezza include le procedure consigliate e consigli per le impostazioni che influiscono sulla sicurezza. Poiché Intune è partner del team di sicurezza di Windows che crea linee di base per i criteri di gruppo, questi suggerimenti si basano su una guida solida e un'esperienza estensiva.
- Se si è nuovi di Intune e non si è sicuri di dove iniziare, quindi le linee di sicurezza di protezione consentiranno di creare e distribuire rapidamente un profilo sicuro.
- Se attualmente si utilizza un criterio di gruppo, la migrazione a Intune per scopi di gestione è molto più semplice con le linee di base di sicurezza, perché sono integrate in Intune e comprendono funzionalità all'avanguardia per la gestione.

Per ulteriori informazioni, vedere [previsioni di sicurezza di Windows](https://go.microsoft.com/fwlink/?linkid=2141503) e [gestione dei dispositivi mobili](https://go.microsoft.com/fwlink/?linkid=2141701).