---
title: Problemi relativi al consenso dell'amministratore
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888320"
---
# <a name="admin-consent-issues"></a>Problemi relativi al consenso dell'amministratore

1. Abilitare il [flusso di lavoro consenso](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) amministratore per consentire agli utenti di richiedere l'approvazione dell'amministratore direttamente dalla schermata di consenso.

1. Se l'utente o gli utenti dell'applicazione stanno visualizzando errori imprevisti durante il processo di consenso, vedere questo articolo per la risoluzione dei problemi: [errore imprevisto durante l'esecuzione del consenso a un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Per ulteriori informazioni, vedere [consenso di amministratore sulla piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), modalità di funzionamento del [prompt di consenso](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) e come [valutare una richiesta di autorizzazione di amministratore a livello di tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente agli utenti e agli amministratori di controllare il modo in cui è possibile accedere ai dati. L'implementazione del modello di autorizzazione è stata aggiornata sull'endpoint della piattaforma Microsoft Identity e modifica il modo in cui un'app deve interagire con la piattaforma Microsoft Identity. Per una panoramica di questo modello di autorizzazione, compresi gli ambiti, le autorizzazioni e il consenso, vedere [autorizzazioni e consenso nell'endpoint della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .