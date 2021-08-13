---
title: Usare le baseline di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971523"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Usare le baseline di sicurezza di Microsoft Intune per configurare i dispositivi Windows 10

Le baseline di sicurezza di Intune consentono di proteggere utenti e servizi Le baseline di sicurezza sono gruppi di impostazioni preconfigurate di Windows usate per l'applicazione di un gruppo noto di impostazioni e valori predefiniti consigliati dai team di sicurezza pertinenti. Creando un profilo della baseline di sicurezza in Intune, è possibile dare vita a un modello formato da più profili di configurazione dei dispositivi.

Quando vengono implementate baseline di sicurezza a gruppi di utenti o dispositivi, le impostazioni vengono applicate ai dispositivi con Windows 10 o versioni successive. Ad esempio, le baseline di sicurezza della gestione dei dispositivi mobili di Microsoft (1) abilita automaticamente BitLocker per le unità rimovibili, (2) richiede la password per sbloccare un dispositivo e (3) disabilita l'autenticazione di base. Quando un valore predefinito non funziona per il proprio ambiente, è possibile personalizzare la baseline per applicare le impostazioni desiderate.

Le baseline di sicurezza consentono inoltre di stabilire un flusso di lavoro end-to-end in Microsoft 365. Seguono alcuni vantaggi di questa funzionalità:
- Una baseline di sicurezza include procedure ottimali e suggerimenti per le impostazioni che riguardano la sicurezza. Dato che Intune lavora in partnership con il team di sicurezza di Windows che crea le baseline per i criteri di gruppo, questi suggerimenti si basano su linee guida solide e una comprovata esperienza.
- Se non conosci bene Intune e non sai da dove cominciare, le baseline di sicurezza ti aiuteranno a creare e implementare rapidamente un profilo sicuro.
- Se stai usando un criterio di gruppo, la migrazione a Intune per scopi correlati alla gestione è più semplice con le baseline di sicurezza, perché tali baseline di sicurezza sono predefinite in Intune e includono funzionalità per la gestione all'avanguardia.

Per ulteriori informazioni, vedere [Baseline di sicurezza di Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) e [Gestione dispositivi mobili](https://docs.microsoft.com/windows/client-management/mdm/).