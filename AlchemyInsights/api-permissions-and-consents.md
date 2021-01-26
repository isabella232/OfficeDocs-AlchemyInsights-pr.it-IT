---
title: Autorizzazioni e autorizzazione API
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951895"
---
# <a name="api-permissions-and-consent"></a>Autorizzazioni e autorizzazione API

Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente agli utenti e agli amministratori di controllare il modo in cui è possibile accedere ai dati. L'implementazione del modello di autorizzazione è stata aggiornata sull'endpoint della piattaforma Microsoft Identity. Viene modificato il modo in cui un'app deve interagire con la piattaforma Microsoft Identity. Le [autorizzazioni e il consenso nell'endpoint della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) riguardano i concetti di base di questo modello di autorizzazione, compresi gli ambiti, le autorizzazioni e il consenso.

Il [Framework di consenso di Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) semplifica lo sviluppo di applicazioni Web multi-tenant e native client. Queste applicazioni consentono l'accesso da parte degli account utente da un tenant di Azure AD diverso da quello in cui è registrata l'applicazione. Potrebbe anche essere necessario accedere alle API Web, ad esempio l'API di Microsoft Graph (per accedere a Azure AD, Intune e servizi in Microsoft 365) e altre API dei servizi Microsoft, oltre alle proprie API Web.

