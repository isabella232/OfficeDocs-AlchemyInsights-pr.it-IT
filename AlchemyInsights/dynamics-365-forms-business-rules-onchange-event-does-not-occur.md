---
title: Dynamics 365 Forms Business Rules - Regola business non in esecuzione per un modulo
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947303"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione

*L'evento OnChange* non si verifica se il campo viene modificato a livello di programmazione utilizzando l'attributo *.* [metodo setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Se vuoi che i gestori eventi per l'evento *OnChange* vengono eseguiti dopo aver impostato il valore, devi usare il metodo [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) dell'attributo *formContext.data.entity* nel codice.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
