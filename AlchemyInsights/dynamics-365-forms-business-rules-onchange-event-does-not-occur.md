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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747993"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione

L' ** evento OnChange non si verifica se il campo viene modificato a livello di programmazione tramite l' *attributo.* [](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) SetValue, metodo. Se si desidera che i gestori eventi per ** l'evento OnChange vengano eseguiti dopo aver impostato il valore, è necessario utilizzare l' *attributo formContext. Data. Entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) , metodo nel codice.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
