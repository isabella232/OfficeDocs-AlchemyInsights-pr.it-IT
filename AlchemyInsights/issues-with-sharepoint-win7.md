---
title: Problemi con SharePoint sulle macchine Windows 7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066999"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemi con SharePoint sulle macchine Windows 7

Se riscontri errori sui computer Windows 7 mentre lavori con SharePoint o OneDrive, potrebbe essere correlato alla deprecazione di TLS 1.0/1.1. Per altre informazioni, vedere:

- [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- TLS1.2 deve essere abilitato nei client Windows 7 SP1/Windows 8. Per altre informazioni, vedi [Si verificano  errori di autenticazione quando il client non supporta TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installa KB3140245 e crea il valore di registro. Per altre informazioni, vedi  [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocolli sicuri di WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Per i client Windows 7 SP1/Windows 8, bisogna assicurare che le suite di crittografia siano iinstallate.  Per altre informazioni, vedi [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


