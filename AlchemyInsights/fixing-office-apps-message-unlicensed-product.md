---
title: Non è possibile attivare Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 50939456df57920994e464db20e5da54f45f197a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744630"
---
# <a name="unable-to-activate-office"></a>Non è possibile attivare Office

- Verificare se lo stato dell'abbonamento risulti scaduto.
- Assicurarsi di avere un abbonamento che consenta licenze client, ad esempio Office 365 Business o Business Premium, e [assicurarsi che all'utente sia assegnata una licenza](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Assicurarsi che l'utente acceda a Office con lo stesso account a cui è assegnata la licenza.
- Controllare la [pagina sull'integrità dei servizi di Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare se sono presenti problemi noti con il servizio.
- Controllare le impostazioni del firewall, del software antivirus e del proxy per confermare che non stanno bloccando l'accesso delle app di Microsoft 365 a Internet. Vedere [URL e intervalli di indirizzi IP per Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalli di indirizzi IP e URL di Office 365").

Utilizzare le seguenti opzioni di risoluzione dei problemi:

- Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) dagli account utente esistenti. [Rimuovere](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [riassegnare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licenza di Office, quindi [accedere a Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con l'account utente interessato.
- Eseguire lo [strumento di risoluzione dei problemi di attivazione.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Reimpostare lo stato di attivazione di Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reimpostare lo stato di attivazione di Office")
- [Eseguire un ripristino online di Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Per ulteriori soluzioni per la risoluzione del problema, vedere:  

- [Errori di attivazione e di tipo Prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)