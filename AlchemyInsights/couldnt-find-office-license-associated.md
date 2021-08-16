---
title: Correzione di Microsoft 365 app Non è stato possibile trovare il messaggio associato alle licenze di Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069608"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Correzione del messaggio Microsoft 365 app "Impossibile trovare le licenze di Office associate"

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controlla le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet Microsoft 365 app. Vedere [Microsoft 365 URL e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Rimuovere e [riassegnare la licenza Office per](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) l'utente interessato. 
3. Aprire un app Office [e disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da qualsiasi account utente esistente.
4. Vai a Windows Impostazioni > **Account Email**& account e rimuovi tutti gli account di lavoro ad eccezione  >  dell'account interessato.
5. Passare a Account Windows Impostazioni > **Accedere** all'istituto di istruzione o all'istituto di istruzione e disconnettere tutti gli account di  >  lavoro ad eccezione dell'account interessato.
6. Reimposta lo stato di attivazione di Office. [Procedura](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Accedi con](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) l'account utente interessato.

Per ulteriori soluzioni di risoluzione dei problemi, vedere Errori di attivazione e prodotti [senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).