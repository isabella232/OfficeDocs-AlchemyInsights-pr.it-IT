---
title: Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886636"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Usare Microsoft Intune di sicurezza per configurare Windows 10 dispositivi

Le baseline di sicurezza di Intune consentono di proteggere utenti e servizi Le linee di base di Windows impostazioni preconfigurato utilizzate per applicare un gruppo noto di impostazioni e valori predefiniti consigliati dai team di sicurezza pertinenti. Creando un profilo della baseline di sicurezza in Intune, è possibile dare vita a un modello formato da più profili di configurazione dei dispositivi.

Quando distribuisci linee di base della sicurezza a gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi eseguiti Windows 10 o versioni successive. Ad esempio, la linea di base di sicurezza microsoft per la gestione dei dispositivi mobili (MDM) abilita automaticamente BitLocker per le unità rimovibili, richiede la password per sbloccare un dispositivo e disabilita l'autenticazione di base. Quando un valore predefinito non funziona per il proprio ambiente, è possibile personalizzare la baseline per applicare le impostazioni desiderate.

Le baseline di sicurezza consentono inoltre di stabilire un flusso di lavoro end-to-end in Microsoft 365. Una baseline di sicurezza include procedure ottimali e suggerimenti per le impostazioni che riguardano la sicurezza. Intune collabora con il team Windows sicurezza che crea linee di base per i criteri di gruppo, quindi questi suggerimenti si basano su solide indicazioni ed esperienze approfondite.

Se non si ha una nuova versione di Intune e non si è certi di dove iniziare, le linee di base della sicurezza consentono di creare e distribuire rapidamente un profilo sicuro. Se attualmente usi criteri di gruppo, la migrazione a Intune per scopi di gestione è molto più semplice con le linee di base della sicurezza perché sono integrate in Intune e includono funzionalità di gestione all'avanguardia.

Per altre informazioni, vedi [l'Windows di base della sicurezza](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e Gestione dei dispositivi [mobili.](https://docs.microsoft.com/windows/client-management/mdm/)

