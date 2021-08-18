---
title: Non è possibile attivare Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327850"
---
# <a name="unable-to-activate-office"></a>Non è possibile attivare Office

**Nota**: se si sta usando una versione precedente di Windows (Ad esempio, Windows 7), assicurarsi che TLS 1.2 sia abilitato per impostazione predefinita. Per ulteriori informazioni, vedere [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocollo di protezione predefinito in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

- Verificare se lo stato dell'abbonamento risulti scaduto.
- Assicurarsi di avere un abbonamento che consenta licenze client, ad esempio Office 365 Business o Business Premium, e [assicurarsi che all'utente sia assegnata una licenza](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Assicurarsi che l'utente acceda a Office con lo stesso account a cui è assegnata la licenza.
- Controllare la [pagina sull'integrità dei servizi di Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) per verificare se sono presenti problemi noti con il servizio.
- Controllare le impostazioni del firewall, del software antivirus e del proxy per confermare che non stanno bloccando l'accesso delle app di Microsoft 365 a Internet. Vedere [URL e intervalli di indirizzi IP di Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Intervalli di indirizzi IP e URL di Office 365").

**Suggerimento:** nei computer Windows è possibile diagnosticare e risolvere automaticamente diversi problemi comuni di accesso a Office. Scaricare ed eseguire l'**[Assistente supporto e ripristino di Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** per usare il tool automatizzato.

Utilizzare le seguenti opzioni di risoluzione dei problemi:

- Aprire un'app di Office e [disconnettersi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) dagli account utente esistenti. [Rimuovere](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) e [riassegnare](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) la licenza di Office, quindi [accedere a Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) con l'account utente interessato.
- Eseguire lo [strumento di risoluzione dei problemi di attivazione.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Reimpostare lo stato di attivazione di Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Reimpostare lo stato di attivazione di Office")
- [Eseguire un ripristino online di Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Per ulteriori soluzioni per la risoluzione del problema, vedere:  

- [Errori di attivazione e di tipo Prodotto senza licenza in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Errore "Non è possibile connettersi a questo account. Riprovare più tardi" all'attivazione di Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)