---
title: Correzione delle app di Microsoft 365 Impossibile trovare il messaggio associato alle licenze di Office
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816492"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Correzione del messaggio "Impossibile trovare licenze di Office associate" per le app di Microsoft 365

Se viene visualizzato questo messaggio, provare a eseguire le operazioni seguenti:

1. Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet alle app di Microsoft 365. Vedere URL e intervalli di indirizzi [IP di Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Rimuovere e [riassegnare la licenza di Office per](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) l'utente interessato. 
3. Aprire un'app di Office [e disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da qualsiasi account utente esistente.
4. Vai a Impostazioni di Windows > **account e-mail**& account e rimuovi tutti gli account di lavoro ad  >  eccezione dell'account interessato.
5. Vai a Impostazioni di Windows > **account Accedi** all'istituto di istruzione o all'istituto di istruzione e disconnetti tutti gli account di lavoro ad eccezione  >  dell'account interessato.
6. Reimposta lo stato di attivazione di Office. [Procedura](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Accedi con](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) l'account utente interessato.

Per ulteriori soluzioni di risoluzione dei problemi, vedere Errori di attivazione e prodotti senza [licenza in Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)