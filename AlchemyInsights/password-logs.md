---
title: Registri password
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523086"
---
# <a name="password-logs"></a>Registri password

**Problemi di accesso ai registri di controllo per la reimpostazione password**

Per risolvere i problemi relativi all'accesso ai registri di controllo per la reimpostazione password, eseguire il passaggio seguente:

Assicurarsi di essere autorizzati a visualizzare i registri di controllo. 

Sono autorizzati solo gli utenti con i seguenti ruoli:
 - Amministratore globale
 - Amministratore della sicurezza
 - Ruolo con autorizzazioni di lettura per la sicurezza

**Visualizzazione di tutti gli eventi di controllo di reimpostazione password a partire dalla distribuzione iniziale**

Nei report degli ultimi 30 giorni vengono archiviati fino a 120.000 eventi di reimpostazione/registrazione password. Il limite massimo si applica all'interfaccia utente quando si scarica il file CSV. Tramite PowerShell sono disponibili un milione di eventi.
Per ulteriori informazioni, vedere i seguenti collegamenti:

- [Eventi di reimpostazione della password self-service dall'API Report ed eventi di Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Come scaricare rapidamente gli eventi di registrazione per la reimpostazione della password con PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Altre informazioni sulle funzionalità di creazione di report per la reimpostazione password**

Controllare chi registra o reimposta le password con i registri di controllo di reimpostazione password di Azure AD nel portale di Azure in **Utenti e gruppi**.
Per ulteriori informazioni, vedere i seguenti collegamenti:

- [Panoramica dei report di reimpostazione della password](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Come visualizzare i report di reimpostazione della password nel portale di Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Eventi di reimpostazione della password self-service dall'API Report ed eventi di Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Come scaricare rapidamente gli eventi di registrazione per la reimpostazione della password con PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


