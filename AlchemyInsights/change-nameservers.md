---
title: Cambiare i server dei nomi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 3f39bfc585e8b805424cb7ccac76f81e1b2bfda9dcd1367361fec6a668c545bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017784"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Aggiornare i server dei nomi di dominio a Microsoft

Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.
  
Per configurare il dominio in Microsoft 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.
  
1. Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.
  
2. Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvare le modifiche.

Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi con un registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  