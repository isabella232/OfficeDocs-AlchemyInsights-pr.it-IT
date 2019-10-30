---
title: Dynamics 365 Forms Business Rules-Business Rule not infornation for a form
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769343"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione

L'evento *OnChange* non si verifica se il campo viene modificato a livello di programmazione tramite l' *attributo.* [SetValue, metodo.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se si desidera che i gestori eventi per l'evento *OnChange* vengano eseguiti dopo aver impostato il valore, è necessario utilizzare il metodo *formContext. Data. Entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) Attribute nel codice.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
