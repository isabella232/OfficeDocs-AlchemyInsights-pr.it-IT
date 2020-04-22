---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706025"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

Se si utilizza **l'accesso condizionale** con Intune, è necessario eseguire tre passaggi: 
  
- Creare un **criterio di accesso condizionale** che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale. 
    
- Creare un **criterio di conformità** per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme. 
    
- Garantire che i criteri di **conformità** e i **criteri di accesso condizionale** siano destinati ai gruppi di utenti desiderati. Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory. 
    
Per ulteriori informazioni, vedere:
  
- [Procedure consigliate per l'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Guida introduttiva all'accesso condizionale](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

