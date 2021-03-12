---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704790"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

**L'uso dell'accesso** condizionale con Intune richiede 3 passaggi:

- Crea un  **criterio di conformità**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve avere un pin di almeno 6 cifre prima di essere considerato conforme.
- Creare un **criterio di accesso**  condizionale che definisce le risorse da proteggere e le condizioni che devono essere soddisfatte per accedere a tali risorse.  [Ad esempio, un dispositivo](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  deve essere conforme prima di accedere alla posta elettronica aziendale.
- Assicurarsi che **i criteri di conformità**  e i criteri di  **accesso**  condizionale siano destinati ai gruppi di utenti desiderati. Questa operazione potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.

**Collegamenti utili:**

[Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi dell'autorità di certificazione](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Criteri per la risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Per proteggere la posta elettronica (Exchange online) dall'accesso da dispositivi non conformi, entrambi i documenti devono essere seguiti:

1. [Proteggere l'accesso alla posta elettronica dai dispositivi tramite EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteggere l'accesso alla posta elettronica da dispositivi che utilizzano client di autenticazione moderna come Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)