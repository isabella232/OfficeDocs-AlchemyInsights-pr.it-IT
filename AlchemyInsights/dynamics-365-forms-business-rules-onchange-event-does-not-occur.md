---
title: Dynamics 365 Forms Business Rules-Business Rule not infornation for a form
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711495"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="589e9-102">L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione</span><span class="sxs-lookup"><span data-stu-id="589e9-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="589e9-103">L'evento *OnChange* non si verifica se il campo viene modificato a livello di programmazione tramite l' *attributo.* [SetValue, metodo.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)</span><span class="sxs-lookup"><span data-stu-id="589e9-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="589e9-104">Se si desidera che i gestori eventi per l'evento *OnChange* vengano eseguiti dopo aver impostato il valore, è necessario utilizzare il metodo *formContext. Data. Entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) Attribute nel codice.</span><span class="sxs-lookup"><span data-stu-id="589e9-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
