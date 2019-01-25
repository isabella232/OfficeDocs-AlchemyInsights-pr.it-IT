---
title: Errore AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499638"
---
# <a name="error-attributevaluemustbeunique"></a>Errore: AttributeValueMustBeUnique

La causa più comune di errori AttributeValueMustBeUnique è due oggetti con diversi SourceAnchor (immutableId) hanno lo stesso valore per gli attributi ProxyAddresses e/o UserPrincipalName. Per correggere l'errore AttributeValueMustBeUnique:
  
1. Identificare i duplicati proxyAddresses, userPrincipalName o altro valore dell'attributo che ha causato l'errore. Vengono indicati gli oggetti due (o più) coinvolti in conflitto. Il report generati dal Azure Active Directory connessione dello stato di sincronizzazione consentono di identificare i due oggetti.
    
2. Identificare quale oggetto deve continuare il valore di duplicati e quale oggetto non dovrebbe essere.
    
3. Rimuovere il valore duplicato dall'oggetto che non dovrebbe includere tale valore. Si noti che è necessario apportare la modifica nella directory in cui l'oggetto viene originato da. In alcuni casi, è necessario eliminare uno degli oggetti in conflitto.
    
4. Se è stata apportata la modifica in locale in Active Directory, consente Azure Active Directory Connetti sincronizzare la modifica dell'errore da ottenere fissa.
    

