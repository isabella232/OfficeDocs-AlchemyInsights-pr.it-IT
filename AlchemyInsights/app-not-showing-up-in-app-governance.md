---
title: La mia app non viene visualizzata in Governance app
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362392"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>La mia app non viene visualizzata in Governance app

Se l'applicazione non viene visualizzata in Governance app, controlla quanto segue:

1. Passare ad [Azure AD](https://aad.portal.azure.com/) e trovare l'ID dell'app cercando il nome dell'app nella barra superiore della pagina Panoramica.

1. Accedi Graph Explorer e cerca l'ID app all'interno dell'entità servizio usando questa query e sostituendo con l'ID app pertinente: <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Se non vengono restituiti risultati, cercare l'ID app all'interno dell'applicazione usando questa query e sostituendo con l'ID app pertinente: <appId> < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Se si verificano problemi con la query, vedere [Ottenere supporto](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Per altre informazioni o informazioni dettagliate sulle tue app nella governance delle app, vedi [Informazioni su visibilità e approfondimenti.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Per altre informazioni sulla visualizzazione delle app, vedi [Visualizzare le app.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
