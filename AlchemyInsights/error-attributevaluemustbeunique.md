---
title: Errore AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813764"
---
# <a name="error-attributevaluemustbeunique"></a>Errore: AttributeValueMustBeUnique

Il motivo più comune dell'errore AttributeValueMustBeUnique è che due oggetti con SourceAnchor (immutableId) diversi hanno lo stesso valore per gli attributi ProxyAddresses e/o UserPrincipalName. Per correggere l'errore AttributeValueMustBeUnique:
  
1. Identificare il valore di attributo proxyAddresses, userPrincipalName o di altro tipo duplicato che causa l'errore. Identificare inoltre quali due (o più) oggetti sono coinvolti nel conflitto. Il report generato da Azure AD Connect Health per la sincronizzazione consente di identificare i due oggetti.
    
2. Identificare l'oggetto che deve continuare a avere il valore duplicato e l'oggetto che non deve essere duplicato.
    
3. Rimuovere il valore duplicato dall'oggetto che NON deve avere tale valore. Si noti che è consigliabile apportare la modifica nella directory da cui viene origine l'oggetto. In alcuni casi, potrebbe essere necessario eliminare uno degli oggetti in conflitto.
    
4. Se è stata apportata la modifica nell'AD locale, consentire ad Azure AD Connect di sincronizzare la modifica per l'errore da sistemare.
    

