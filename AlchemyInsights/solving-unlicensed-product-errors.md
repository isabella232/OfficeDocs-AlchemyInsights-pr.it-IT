---
title: Risoluzione degli errori di prodotto non concessi in licenza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737957"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Suggerimenti per la risoluzione degli errori di "prodotto senza licenza"

Per risolvere gli errori relativi a un prodotto privo di licenza, provare a eseguire le operazioni seguenti:

- Controllare se lo stato della sottoscrizione è scaduto.
- Assicurarsi di disporre di un abbonamento che consenta licenze client, ad esempio Microsoft 365 Apps for business o Business Premium, e [assicurarsi che l'utente disponga di una licenza assegnata](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Verificare che l'utente sia abilitato all'accesso a Office con lo stesso account a cui è assegnata la licenza.
- Controllare la [pagina integrità del servizio](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare la presenza di eventuali problemi noti con il servizio.
- Controllare il firewall, il software antivirus e le impostazioni proxy per confermare che non bloccano l'accesso di Microsoft 365 Apps a Internet. Vedere [URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

È inoltre possibile provare le seguenti azioni per la risoluzione dei problemi: 

- Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) da tutti gli account utente esistenti. [Rimuovere](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [riassegnare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licenza di Office, quindi [accedere a Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) utilizzando l'account utente in questione.
- Eseguire lo strumento di [risoluzione dei problemi di attivazione](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Reimposta lo stato di attivazione di Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Eseguire una riparazione online di Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Per ulteriori soluzioni per la risoluzione del problema, vedere: 

- [Errori di attivazione e di tipo Prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)