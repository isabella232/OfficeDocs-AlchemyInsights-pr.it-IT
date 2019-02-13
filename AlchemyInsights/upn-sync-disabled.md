---
title: Sincronizzazione UPN disabilitato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921712"
---
# <a name="upn-sync-disabled"></a>Sincronizzazione UPN disabilitato

Se è stata avviata la sincronizzazione di Azure Active Directory prima di 30 marzo 2016, eseguire il seguente cmdlet PowerShell di Azure Active Directory per abilitare UPN soft è adatto solo l'organizzazione:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-abilitare $True**
  
Corrispondenza soft UPN è attivata automaticamente per le organizzazioni che ha avviato la sincronizzazione di Azure Active Directory o dopo 30 marzo 2016.
  
Per ulteriori informazioni sull'abilitazione di corrispondenza soft UPN e altre funzionalità di sincronizzazione, vedere [caratteristiche del servizio di sincronizzazione Connetti Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

