---
title: Accesso condizionale con Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662331"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

Utilizzo di **Access condizionale** con Intune richiede 3 passaggi: 
  
- Creare un **Criterio di accesso condizionale** che definisce le risorse sono protetti e quali condizioni devono essere soddisfatti per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale. 
    
- Creare un **Criterio di conformità** per definire le impostazioni che devono essere soddisfatti prima che il dispositivo è considerato conforme. Ad esempio, un dispositivo deve disporre un pin di almeno 6 cifre prima che sia considerato compatibile. 
    
- Verificare i **Criteri di conformità** e **Criteri di accesso condizionale** destinate ai gruppi di utenti desiderati. Ciò può richiedere la creazione di gruppi di utenti specifici in Azure Active Directory. 
    
Per ulteriori informazioni:
  
- [Procedure consigliate di accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduzione a Access condizionale](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

