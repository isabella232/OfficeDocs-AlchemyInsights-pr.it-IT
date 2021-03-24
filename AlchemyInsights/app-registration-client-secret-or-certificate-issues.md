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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123200"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemi relativi al certificato o al segreto client di registrazione app

Il segreto client dell'applicazione scade?

Indipendentemente dalla modalità di creazione dell'applicazione registrata, tramite il processo di registrazione standard nel portale di registrazione delle app o se l'entità servizio è stata creata nel tenant utilizzando il consenso dell'applicazione, sarà necessario creare un nuovo segreto client prima della scadenza di quella corrente e aggiornarne il codice dell'applicazione correlata. Il periodo di validità massimo è 2 anni. Come promemoria, il valore segreto deve essere registrato perché non sarà più visibile dopo aver lasciato la pagina Registrazioni app nel portale. Per altre informazioni, vedi [Guida introduttiva: Registrare un'app nella](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) piattaforma di identità Microsoft e [Procedure consigliate per la piattaforma di identità Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Per altre informazioni, vedi [Creare un'entità](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)servizio & app Azure AD nel portale - Piattaforma di identità Microsoft.
