---
title: Uso dell'accesso condizionale con Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529362"
---
# <a name="using-conditional-access-with-intune"></a>Uso dell'accesso condizionale con Intune

L'uso dell'accesso condizionale con Intune richiede 3 passaggi:

- [Crea un criterio di conformità per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve avere un pin di almeno 6 cifre prima di essere considerato conforme.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Creare un criterio di accesso condizionale che definisce le risorse da proteggere e le condizioni che devono essere soddisfatte per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Assicurarsi che i criteri di conformità e i criteri di accesso condizionale siano destinati ai gruppi di utenti desiderati. Questa operazione potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Altre informazioni...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
