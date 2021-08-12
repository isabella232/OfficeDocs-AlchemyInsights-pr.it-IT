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
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957104"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Suggerimenti per la risoluzione degli errori di "Prodotto senza licenza"

Per risolvere gli errori relativi a un "Prodotto senza licenza", provare a eseguire le operazioni seguenti:

- Verificare se lo stato dell'abbonamento è scaduto.
- Assicurati di disporre di una sottoscrizione che consenta le licenze client, ad esempio Microsoft 365 Apps for business o Business Premium, e assicurati che all'utente sia assegnata [una licenza](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Assicurati che l'utente abbia effettuato l'accesso Office con lo stesso account a cui è assegnata la licenza.
- Controllare la [pagina Integrità del servizio](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare se sono presenti problemi noti con il servizio.
- Controlla le impostazioni del firewall, del software antivirus e del proxy per verificare che non blocchino Microsoft 365'accesso delle app a Internet. Vedere [URL e intervalli di indirizzi IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

È inoltre possibile provare le azioni di risoluzione dei problemi seguenti: 

- Aprire un app Office [e disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da qualsiasi account utente esistente. [Rimuovere](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [rias assegnare Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenza e quindi accedere a Office [utilizzando](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) l'account utente interessato.
- Eseguire lo [strumento di risoluzione dei problemi di attivazione](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reimposta lo stato di attivazione di Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Eseguire un ripristino online di Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Per ulteriori soluzioni per la risoluzione del problema, vedere: 

- [Errori di attivazione e di tipo Prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)