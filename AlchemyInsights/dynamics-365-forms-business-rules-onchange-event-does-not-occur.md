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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529023"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="0ebd1-102">L'evento OnChange non si verifica se il campo viene modificato a livello di programmazione</span><span class="sxs-lookup"><span data-stu-id="0ebd1-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="0ebd1-103">L' \*\* evento OnChange non si verifica se il campo viene modificato a livello di programmazione tramite l' *attributo.* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) SetValue, metodo.</span><span class="sxs-lookup"><span data-stu-id="0ebd1-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="0ebd1-104">Se si desidera che i gestori eventi per \*\* l'evento OnChange vengano eseguiti dopo aver impostato il valore, è necessario utilizzare l' *attributo formContext. Data. Entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) , metodo nel codice.</span><span class="sxs-lookup"><span data-stu-id="0ebd1-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
