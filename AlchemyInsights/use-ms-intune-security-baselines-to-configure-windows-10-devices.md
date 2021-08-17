---
title: Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104348"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi

Le baseline di sicurezza di Intune consentono di proteggere utenti e servizi Le baseline di sicurezza sono gruppi di impostazioni preconfigurate di Windows usate per l'applicazione di un gruppo noto di impostazioni e valori predefiniti consigliati dai team di sicurezza pertinenti. Creando un profilo della baseline di sicurezza in Intune, è possibile dare vita a un modello formato da più profili di configurazione dei dispositivi.

Quando distribuisci linee di base di sicurezza a gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi eseguiti Windows 10 o versioni successive. Ad esempio, MDM Security Baseline automaticamente (1) abilita BitLocker per le unità rimovibili, (2) richiede la password per sbloccare un dispositivo e (3) disabilita l'autenticazione di base. Quando un valore predefinito non funziona per l'ambiente, personalizza la linea di base per applicare le impostazioni necessarie.

Le baseline di sicurezza consentono inoltre di stabilire un flusso di lavoro end-to-end in Microsoft 365. Di seguito sono riportati alcuni vantaggi:

- Una baseline di sicurezza include procedure ottimali e suggerimenti per le impostazioni che riguardano la sicurezza. Dato che Intune lavora in partnership con il team di sicurezza di Windows che crea le baseline per i criteri di gruppo, questi suggerimenti si basano su linee guida solide e una comprovata esperienza.
- Se non conosci bene Intune e non sai da dove cominciare, le baseline di sicurezza ti aiuteranno a creare e implementare rapidamente un profilo sicuro.
- Se attualmente si usano criteri di gruppo, la migrazione a Intune per scopi di gestione è molto più semplice con le linee di base della sicurezza, perché sono integrate in Intune e includono funzionalità all'avanguardia per la gestione.

Per altre informazioni, vedi le [Windows di sicurezza](https://go.microsoft.com/fwlink/?linkid=2141503) e Gestione dei dispositivi [mobili.](https://go.microsoft.com/fwlink/?linkid=2141701)