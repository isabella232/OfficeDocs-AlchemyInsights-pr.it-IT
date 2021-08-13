---
title: Problemi di prestazioni SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093741"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint o OneDrive lento, inaccessibile o non disponibile per più utenti

Se un sito OneDrive o SharePoint non è disponibile per più utenti che in precedenza avevano accesso, potrebbe verificarsi un problema temporaneo del servizio. [Controllare il dashboard di integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth).

**Aggiungere e aggiungere una licenza all'utente**

Assicurati di [assegnare licenze agli utenti in Microsoft 365 per le aziende.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Assegnare autorizzazioni**

Se all'utente è stata assegnata una licenza di SharePoint e sta ancora ricevendo un messaggio di accesso negato, assicurarsi che abbia il [livello di autorizzazione](https://docs.microsoft.com/sharepoint/understanding-permission-levels) appropriato assegnato.

**Considerare la possibilità di usare la funzionalità di richiesta di accesso**

La [funzionalità di richiesta di accesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) consente agli utenti di richiedere l'accesso a contenuto attualmente non autorizzato a visualizzare.

**Consenti script personalizzato può causare problemi di accesso negato**

Esistono alcuni scenari in cui la *funzionalità Consenti script* personalizzato potrebbe presentare un accesso negato. Per un elenco delle funzionalità interessate, considerazioni sulla sicurezza e sulla possibilità di disabilitarla. Visitare [Consenti o impedisci script personalizzati.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

