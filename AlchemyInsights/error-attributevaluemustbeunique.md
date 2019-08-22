---
title: Errore AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527007"
---
# <a name="error-attributevaluemustbeunique"></a>Errore: AttributeValueMustBeUnique

Il motivo più comune per l'errore AttributeValueMustBeUnique è che due oggetti con SourceAnchor diversi (immutableId) hanno lo stesso valore per gli attributi ProxyAddresses e/o UserPrincipalName. Per correggere l'errore AttributeValueMustBeUnique:
  
1. Identificare il valore di proxyAddresses, userPrincipalName o altri attributi duplicati che causa l'errore. Identificare anche i due (o più) oggetti coinvolti nel conflitto. Il report generato da Azure AD Connect Health for Sync può essere utile per identificare i due oggetti.
    
2. Identificare l'oggetto che deve continuare a utilizzare il valore duplicato e l'oggetto da evitare.
    
3. Rimuovere il valore duplicato dall'oggetto che non deve disporre di tale valore. Si noti che è necessario apportare le modifiche nella directory da cui viene creato l'oggetto. In alcuni casi, potrebbe essere necessario eliminare uno degli oggetti in conflitto.
    
4. Se è stata apportata la modifica nell'annuncio locale, fare in modo che Azure AD Connect connetta la modifica per ottenere la correzione dell'errore.
    

