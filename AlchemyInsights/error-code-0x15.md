---
title: Codice di errore 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto, è consigliabile abilitare ADAL modificando il Registro di sistema.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100766"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Errore durante l'Office 2013 in Servizi Desktop remoto

Se si riceve un errore durante l'attivazione di Office 2013 nelle distribuzioni di Servizi Desktop remoto, è consigliabile abilitare ADAL modificando il Registro di sistema.
  
|**Chiave del Registro di sistema**|**Tipo**|**Valore**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Per ulteriori informazioni, vedere [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL è abilitato per impostazione predefinita in Microsoft 365 Apps for enterprise e Office 2016. Servizi Desktop remoto era in precedenza denominato Servizi terminal.
  