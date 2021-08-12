---
title: Autorizzazioni API e consenso
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932101"
---
# <a name="api-permissions-and-consent"></a>Autorizzazioni API e consenso

Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente a utenti e amministratori di controllare la modalità di accesso ai dati. L'implementazione del modello di autorizzazione è stata aggiornata nell Microsoft Identity Platform endpoint. Cambia il modo in cui un'app deve interagire con il Microsoft Identity Platform. [Le autorizzazioni e il consenso nell Microsoft Identity Platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) illustrano i concetti di base di questo modello di autorizzazione, inclusi ambiti, autorizzazioni e consenso.

Il [framework Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) semplifica lo sviluppo di applicazioni client web e native multi-tenant. Queste applicazioni consentono l'accesso da parte di account utente da un tenant di Azure AD diverso da quello in cui l'applicazione è registrata. Potrebbe anche essere necessario accedere alle API Web, ad esempio l'API di Microsoft Graph (per accedere ad Azure AD, Intune e ai servizi in Microsoft 365) e altre API di servizi Microsoft, oltre alle API Web.

