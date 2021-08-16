---
title: Distribuzione di componenti aggiuntivi per Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031410"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Distribuzione di componenti aggiuntivi per Microsoft 365 Apps

La distribuzione centralizzata è il modo consigliato per distribuire Office componenti aggiuntivi a utenti e gruppi all'interno dell'organizzazione. Per distribuire i componenti aggiuntivi, attenersi alla procedura seguente:

**Nota:** Per installare i componenti aggiuntivi per Office come singolo utente, vedere Visualizzare, gestire e installare i componenti aggiuntivi [nei Office applicazioni.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Assicurati inoltre che sia abilitata l'acquisizione Office componenti aggiuntivi dello Store. Per informazioni dettagliate, vedere [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Verificare che l'ambiente soddisfi i requisiti per la distribuzione di componenti aggiuntivi tramite distribuzione centralizzata. Per informazioni dettagliate, vedere [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Vai a **Impostazioni**  >  **App integrate** Ottieni  >  **app** nella interfaccia di amministrazione di Microsoft 365 per distribuire i componenti aggiuntivi. 

Note: 

- Le app integrate richiedono che l'amministratore abbia autorizzazioni di amministratore globale o Exchange amministratore.

- Quando si distribuiscono componenti aggiuntivi a più utenti, è consigliabile eseguire assegnazioni utilizzando gruppi anziché singoli utenti. Per informazioni dettagliate, [vedere Considerazioni sull'assegnazione di](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)un componente aggiuntivo a utenti e gruppi.

- La distribuzione centralizzata non supporta gli utenti di gruppi annidati o gruppi con gruppi padre. Per informazioni dettagliate, vedere [Assegnazioni di utenti e gruppi.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Verificare che il servizio di gestione app di Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') sia abilitato agli utenti per l'accesso. Per informazioni dettagliate, vedi [Configurare le proprietà dell'app.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Se si verificano problemi di distribuzione dei componenti aggiuntivi tramite le app integrate, provare a eseguire la distribuzione utilizzando [Componenti aggiuntivi](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Per altre informazioni, vedere:

[Distribuire componenti aggiuntivi nell'interfaccia di amministrazione](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gestire i componenti aggiuntivi nell'interfaccia di amministrazione](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizzare i cmdlet di PowerShell per la distribuzione centralizzata per gestire i componenti aggiuntivi](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Pubblicare Office componenti aggiuntivi utilizzando la](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) distribuzione centralizzata tramite 
 interfaccia di amministrazione di Microsoft 365 [Risoluzione dei problemi: l'utente non vede i componenti aggiuntivi](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Risolvere gli errori degli utenti Office componenti aggiuntivi](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)