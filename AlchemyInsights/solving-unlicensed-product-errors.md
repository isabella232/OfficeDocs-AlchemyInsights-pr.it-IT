---
title: Risoluzione degli errori dei prodotti senza licenza
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786853"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Suggerimenti per la risoluzione degli errori di "Prodotto senza licenza"

Per risolvere gli errori relativi a un "Prodotto senza licenza", provare a eseguire le operazioni seguenti:

- Verificare se lo stato dell'abbonamento è scaduto.
- Assicurati di disporre di una sottoscrizione che consenta le licenze client, ad esempio Microsoft 365 Apps for business o Business Premium, e assicurati che all'utente sia assegnata [una licenza](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Verificare che l'utente abbia effettuato l'accesso a Office con lo stesso account a cui è assegnata la licenza.
- Controllare la [pagina Integrità del servizio](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare se sono presenti problemi noti con il servizio.
- Controllare le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino l'accesso a Internet delle app di Microsoft 365. Vedere [URL e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

È inoltre possibile provare le azioni di risoluzione dei problemi seguenti: 

- Aprire un'app di Office [e disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da qualsiasi account utente esistente. [Rimuovere](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [rias assegnare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licenza di Office, quindi [accedere a Office utilizzando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) l'account utente interessato.
- Eseguire lo [strumento di risoluzione dei problemi di attivazione](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reimposta lo stato di attivazione di Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Eseguire un ripristino online di Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Per ulteriori soluzioni per la risoluzione del problema, vedere: 

- [Errori di attivazione e di tipo Prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)