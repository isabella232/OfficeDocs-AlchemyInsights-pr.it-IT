---
title: Errore AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709155"
---
# <a name="error-attributevaluemustbeunique"></a>Errore: AttributeValueMustBeUnique

Il motivo più comune per l'errore AttributeValueMustBeUnique è che due oggetti con SourceAnchor diversi (immutableId) hanno lo stesso valore per gli attributi ProxyAddresses e/o UserPrincipalName. Per correggere l'errore AttributeValueMustBeUnique:
  
1. Identificare il valore di proxyAddresses, userPrincipalName o altri attributi duplicati che causa l'errore. Identificare anche i due (o più) oggetti coinvolti nel conflitto. Il report generato da Azure AD Connect Health for Sync può essere utile per identificare i due oggetti.
    
2. Identificare l'oggetto che deve continuare a utilizzare il valore duplicato e l'oggetto da evitare.
    
3. Rimuovere il valore duplicato dall'oggetto che non deve disporre di tale valore. Si noti che è necessario apportare le modifiche nella directory da cui viene creato l'oggetto. In alcuni casi, potrebbe essere necessario eliminare uno degli oggetti in conflitto.
    
4. Se è stata apportata la modifica nell'annuncio locale, fare in modo che Azure AD Connect connetta la modifica per ottenere la correzione dell'errore.
    

