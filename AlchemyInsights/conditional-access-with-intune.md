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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935943"
---
# <a name="conditional-access-with-intune"></a>Accesso condizionale con Intune

Utilizzo di **Access condizionale** con Intune richiede 3 passaggi: 
  
- Creare un **Criterio di accesso condizionale** che definisce le risorse sono protetti e quali condizioni devono essere soddisfatti per accedere a tali risorse. Ad esempio, un dispositivo deve essere conforme prima di accedere alla posta elettronica aziendale. 
    
- Creare un **Criterio di conformità** per definire le impostazioni che devono essere soddisfatti prima che il dispositivo è considerato conforme. Ad esempio, un dispositivo deve disporre un pin di almeno 6 cifre prima che sia considerato compatibile. 
    
- Verificare i **Criteri di conformità** e **Criteri di accesso condizionale** destinate ai gruppi di utenti desiderati. Ciò può richiedere la creazione di gruppi di utenti specifici in Azure Active Directory. 
    
Per ulteriori informazioni:
  
- [Procedure consigliate di accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introduzione a Access condizionale](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

