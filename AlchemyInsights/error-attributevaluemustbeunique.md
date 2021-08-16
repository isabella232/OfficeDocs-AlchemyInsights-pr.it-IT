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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002124"
---
# <a name="error-attributevaluemustbeunique"></a>Errore: AttributeValueMustBeUnique

Il motivo più comune dell'errore AttributeValueMustBeUnique è che due oggetti con SourceAnchor (immutableId) diversi hanno lo stesso valore per gli attributi ProxyAddresses e/o UserPrincipalName. Per correggere l'errore AttributeValueMustBeUnique:
  
1. Identificare il valore di attributo proxyAddresses, userPrincipalName o di altro tipo duplicato che causa l'errore. Identificare inoltre quali due (o più) oggetti sono coinvolti nel conflitto. Il report generato da Azure AD Connessione Health per la sincronizzazione può aiutare a identificare i due oggetti.
    
2. Identificare l'oggetto che deve continuare a avere il valore duplicato e l'oggetto che non deve essere duplicato.
    
3. Rimuovere il valore duplicato dall'oggetto che NON deve avere tale valore. Si noti che è consigliabile apportare la modifica nella directory da cui viene origine l'oggetto. In alcuni casi, potrebbe essere necessario eliminare uno degli oggetti in conflitto.
    
4. Se hai apportato la modifica nell'AD locale, consenti ad Azure AD di Connessione la modifica per la correzione dell'errore.
    

