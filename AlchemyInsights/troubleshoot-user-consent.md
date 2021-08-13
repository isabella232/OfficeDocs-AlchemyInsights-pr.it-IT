---
title: Risolvere i problemi relativi al consenso degli utenti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007902"
---
# <a name="troubleshoot-user-consent"></a>Risolvere i problemi relativi al consenso degli utenti

1. È possibile configurare il modo in cui gli utenti finali acconsentino alle applicazioni tramite il portale di Azure o PowerShell. Per [altre informazioni, vedi Impostazioni di consenso](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) dell'utente.
1. Un amministratore può anche usare [l'API microsoft Graph per](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) concedere il consenso alle autorizzazioni delegate per conto di un singolo utente. Per ulteriori informazioni, vedere [Ottenere l'accesso per conto di un utente.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Errori di consenso dell'utente](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): in questo articolo vengono illustrati gli errori che possono verificarsi durante il processo di consenso a un'applicazione. Se stai risoluzione dei problemi relativi a richieste di consenso impreviste che non contengono messaggi di errore, vedi [Scenari di autenticazione per Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)