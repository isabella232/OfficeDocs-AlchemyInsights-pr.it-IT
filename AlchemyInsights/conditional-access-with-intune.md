---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393545"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

Se si utilizza **l'accesso condizionale** con Intune, è necessario eseguire tre passaggi: 
  
- Creare un **criterio di accesso condizionale** che definisce le risorse protette e quali condizioni devono essere soddisfatte per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale. 
    
- Creare un **criterio di conformità** per definire le impostazioni che devono essere soddisfatte prima che il dispositivo venga considerato conforme. Ad esempio, un dispositivo deve disporre di un pin di almeno 6 cifre prima di essere considerato conforme. 
    
- Garantire che i criteri di **conformità** e i **criteri di accesso condizionale** siano destinati ai gruppi di utenti desiderati. Questo potrebbe richiedere la creazione di gruppi specifici di utenti in Azure Active Directory. 
    
Per ulteriori informazioni, vedere:
  
- [Procedure consigliate per l'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Guida introduttiva all'accesso condizionale](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

