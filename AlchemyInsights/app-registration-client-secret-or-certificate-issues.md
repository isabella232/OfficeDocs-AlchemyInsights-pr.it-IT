---
title: Problemi relativi al certificato o al segreto client di registrazione app
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951497"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemi relativi al certificato o al segreto client di registrazione app

Il segreto client dell'applicazione scade?

Indipendentemente dalla modalità di creazione dell'applicazione registrata, tramite il processo di registrazione standard nel portale di registrazione delle app o se l'entità servizio è stata creata nel tenant utilizzando il consenso dell'applicazione, sarà necessario creare un nuovo segreto client prima della scadenza di quella corrente e aggiornarne il codice dell'applicazione correlata. Il periodo di validità massimo è 2 anni. Come promemoria, il valore segreto deve essere registrato perché non sarà più visibile dopo aver lasciato la pagina Registrazioni app nel portale. Per altre informazioni, vedi [Guida introduttiva: Registrare un'app](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) nel Microsoft Identity Platform e [Procedure consigliate per](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)il Microsoft Identity Platform .

Per altre informazioni, vedere [Create an Azure AD app & service principal in the portal - Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
