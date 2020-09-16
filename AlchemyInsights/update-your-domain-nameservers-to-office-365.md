---
title: Aggiornare i server dei nomi di dominio a Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734915"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Aggiornare i server dei nomi di dominio a Microsoft

Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.
  
Per configurare il dominio con Microsoft, è necessario aggiornare i server dei nomi presso il registrar. Creare o modificare i record dei server dei nomi nel registrar.
  
1. Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.

2. Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvare le modifiche.

È inoltre possibile trovare istruzioni dettagliate in questo articolo: [modificare i server dei nomi per configurare Microsoft 365 con qualsiasi registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  