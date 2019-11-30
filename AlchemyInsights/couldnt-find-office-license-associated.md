---
title: Fissaggio delle app di Office non è stato possibile trovare il messaggio associato alle licenze
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627922"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Risoluzione delle app di Office "Impossibile trovare il messaggio relativo alle licenze di Office"

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso a Internet alle app di Office. Vedere gli [intervalli di indirizzi IP e URL di Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Rimuovere e [riassegnare la licenza di Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) per l'utente in questione. 
3. Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da tutti gli account utente esistenti.
4. Passare a impostazioni di Windows **>** > account **& di posta elettronica**e rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato.
5. Passare a impostazioni di Windows > **account** > di**accesso al lavoro o all'Istituto di istruzione**e disconnettere tutti gli account di lavoro ad eccezione dell'account danneggiato.
6. Reimpostare lo stato di attivazione di Office. [Procedura](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Accedere](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) utilizzando l'account utente in questione.

Per ulteriori soluzioni per la risoluzione dei problemi, vedere [errori di attivazione e di prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).