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
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069716"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

**L'uso dell'accesso** condizionale con Intune richiede 3 passaggi:

- Crea criteri **di conformità** ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)Windows ) [per](https://docs.microsoft.com//intune/compliance-policy-create-windows)definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve avere un pin di almeno 6 cifre prima di essere considerato conforme.
- Creare criteri **di accesso condizionale**  che definiscono quali risorse vengono protette e quali condizioni devono essere soddisfatte per accedere a tali risorse.  [Ad esempio, un](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.
- Verificare che **i criteri di conformità**  e i criteri di  **accesso**  condizionale siano destinati ai gruppi di utenti desiderati. Potrebbe essere necessario creare gruppi specifici di utenti in Azure Active Directory.

**Collegamenti utili:**

[Panoramica della conformità dei dispositivi](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi relativi a CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Criteri di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Per proteggere la posta elettronica (Exchange online) dall'accesso da dispositivi non conformi, entrambi i documenti devono essere seguiti:

1. [Proteggere l'accesso alla posta elettronica dai dispositivi tramite EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteggere l'accesso alla posta elettronica da dispositivi che utilizzano client di autenticazione moderni come Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)