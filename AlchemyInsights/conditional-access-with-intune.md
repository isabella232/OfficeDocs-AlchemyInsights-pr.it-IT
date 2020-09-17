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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807663"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

Se si utilizza  **l'accesso condizionale**  con Intune, è necessario eseguire tre passaggi:

- Creare un  **criterio di conformità**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme.
- Creare un **criterio di accesso condizionale**  che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse.  [Ad esempio,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale.
- Verificare che i criteri di **conformità**  e i  **criteri di accesso condizionale**  siano destinati ai gruppi di utenti desiderati. Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory.

**Collegamenti utili:**

[Panoramica della conformità del dispositivo](https://docs.microsoft.com/intune/device-compliance-get-started)

[Risoluzione dei problemi relativi all'autorità di certificazione](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Risoluzione dei problemi relativi ai criteri](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Per proteggere la posta elettronica (Exchange Online) dall'accesso da dispositivi non conformi, è necessario seguire entrambi i documenti:

1. [Protezione dell'accesso alla posta elettronica dai dispositivi tramite EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Protezione dell'accesso tramite posta elettronica da dispositivi che utilizzano client di autenticazione moderni come Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)