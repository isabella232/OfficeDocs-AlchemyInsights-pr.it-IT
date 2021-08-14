---
title: Problemi di consenso dell'amministratore
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
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952577"
---
# <a name="admin-consent-issues"></a>Problemi di consenso dell'amministratore

1. Abilita il [flusso di lavoro del consenso](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) dell'amministratore per consentire agli utenti di richiedere l'approvazione dell'amministratore direttamente dalla schermata di consenso.

1. Se l'utente o gli utenti dell'applicazione visualizzano errori imprevisti durante il processo di consenso, vedere questo articolo per la procedura di risoluzione dei problemi: Errore imprevisto durante l'esecuzione del [consenso a un'applicazione.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Ulteriori informazioni sul [consenso dell'Microsoft Identity Platform,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)sul [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) funzionamento della richiesta di consenso e su come valutare una richiesta per il consenso dell'amministratore a livello [di tenant.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente a utenti e amministratori di controllare la modalità di accesso ai dati. L'implementazione del modello di autorizzazione è stata aggiornata nell'endpoint Microsoft Identity Platform e cambia il modo in cui un'app deve interagire con l'Microsoft Identity Platform. Vedi [Autorizzazioni e consenso nell'endpoint Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) per una panoramica di questo modello di autorizzazione, inclusi ambiti, autorizzazioni e consenso.