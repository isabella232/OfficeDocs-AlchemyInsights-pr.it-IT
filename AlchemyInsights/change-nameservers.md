---
title: Cambiare i server dei nomi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736653"
---
# <a name="update-your-domain-nameservers-to-office-365"></a>Aggiornare i server dei nomi di dominio a Office 365

Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.
  
Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.
  
1. Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.
  
2. Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvare le modifiche.

Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  