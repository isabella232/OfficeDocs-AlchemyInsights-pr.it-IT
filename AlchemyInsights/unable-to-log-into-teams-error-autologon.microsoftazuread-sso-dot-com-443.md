---
title: Non è possibile accedere a Teams a causa di un errore autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038404"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Non è possibile accedere a Teams a causa di un errore autologon.microsoftazuread-sso dot com:443

Se come autenticazione di Office 365 è abilitato l'accesso SSO facile, potrebbe essere necessario aggiungere l'URL "autologon.microsoftazuread-sso.com" ai siti Intranet.  Se in precedenza è stato aggiunto all'elenco Siti attendibili ed è in uso l'accesso SSO facile, deve essere rimosso dai siti attendibili.

Leggere l'[elenco di controllo per la risoluzione dei problemi dell'accesso SSO facile](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Seguire questa procedura per aggiungere un URL all'elenco dei siti Intranet:

1. Aprire Internet Explorer facendo clic sul pulsante **Start**. Nella casella di ricerca digitare Internet Explorer e quindi nell'elenco dei risultati fare clic su **Internet Explorer**.
2. Fare clic su **Strumenti**, quindi su **Opzioni Internet**.
3. Fare clic sulla scheda **Sicurezza**.
4. A questo punto, fare clic su **Intranet locale**, sul pulsante **siti** e quindi sul pulsante **Avanzate**.
5. Immettere l'URL del sito Web e fare clic su **Aggiungi**.
6. Al termine, fare clic su **Chiudi**.

Per altre informazioni, vedere la [documentazione per la distribuzione dell'accesso SSO facile per Office 365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (include il processo basato su criteri per aggiungere un URL ai siti Intranet nel passaggio 3).
