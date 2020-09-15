---
title: "Risolvere l'errore di accesso AADSTS9000411 in Teams "
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687042"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Risolvere l'errore di accesso AADSTS9000411 in Teams 

Quando si esegue l'accesso a Microsoft Teams, è possibile che venga visualizzato il messaggio di errore: **Si è verificato un problema di accesso di tipo AADSTS9000411: la richiesta non è stata formattata correttamente. Il parametro "login_hint" è stato duplicato.**

Per risolvere il problema, verificare che i client di Microsoft Teams siano aggiornati. Per altre informazioni sull'aggiornamento del client, vedere [Aggiornare Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Se non è possibile aggiornare il client per qualche motivo, disconnettendo il client sarà possibile eliminare la maggior parte dei dati memorizzati nella cache. Tuttavia, se si verificano ancora problemi dopo la disconnessione/connessione, chiudere Teams e cancellare la cache del client eseguendo le operazioni seguenti:
1. Chiudere Microsoft Teams.
2. Passare a: %appdata%\microsoft\teams e cancellare tutti i file.
3. Riaprire Microsoft Teams.
