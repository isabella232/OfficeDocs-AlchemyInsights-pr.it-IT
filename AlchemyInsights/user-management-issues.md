---
title: Problemi di gestione utenti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971461"
---
# <a name="user-management-issues"></a>Problemi di gestione utenti

**Cosa succede agli utenti attualmente assegnati all’applicazione se viene disabilitata la proprietà ‘Assegnazione utenti obbligatoria’ (proprietà impostata su No)?**

La disattivazione della **Assegnazione utenti obbligatoria** NON influisce sugli utenti attualmente assegnati. La disattivazione di questa proprietà consentirà a tutti gli utenti di accedere all’applicazione.  Tutti gli utenti elencati e gli utenti assegnati a gruppi nell’applicazione continueranno ad essere validi.

- Per limitare l’app a uno specifico gruppo di utenti, vedere [Limitare l’app Azure AD a un gruppo di utenti - Microsoft Identity Platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Per l’assegnazione di utenti e gruppi ad applicazioni aziendali in Azure Active Directory (Azure AD), dal portale di Azure o utilizzando PowerShell, vedere [Gestire l’assegnazione di utenti ad una app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Per delegare le autorizzazioni per la creazione e la gestione di applicazioni, vedere [Delegare le autorizzazioni di amministratore per la gestione di applicazioni - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Nascondere specifiche app aziendali agli utenti** - Eseguire i seguenti passaggi per nascondere tutte le app di Microsoft 365 dal pannello **App personali**. Le app saranno ancora visibili nel portale di Office 365.

 1. Accedere al portale di Azure come amministratore globale della directory. 
 2. Selezionare **Azure Active Directory**. 
 3. Selezionare **Utenti**. 
 4. Selezionare **Impostazioni utente**. 
 5. In **Applicazioni aziendali**, fare clic su **Gestire come gli utenti finali avviano e visualizzano le applicazioni**. 
 6. Per **Gli utenti possono vedere solo le app di Office 365 nel portale di Office 365**, fare clic su **Sì**. 
 7. Fare clic su **Salva**. 
 8. Per altri dettagli, vedere [Nascondere un’applicazione aziendale dall’esperienza dell’utente in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Se si offre una applicazione SaaS (Software come servizio) a diverse organizzazioni, è possibile configurare l’app in modo che accetti gli accessi da qualsiasi tenant Azure Active Directory (Azure AD). Questa configurazione è chiamata "applicazione multi-tenant". Gli utenti in qualsiasi tenant Azure AD potranno accedere all’app dopo aver acconsentito a utilizzare il proprio account nell’app. Per altre informazioni, vedere [Creare app che consentono l’accesso ad utenti Azure AD - Microsoft Identity Platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **In che modo un utente finale può accedere all’applicazione una volta che è stato assegnato all’applicazione?**

Ogni app nel pannello Applicazioni aziendali contiene un collegamento per l’accesso degli utenti finali. Gli utenti possono accedere facilmente all’app anche attraverso il portale **App personali**.

- **Si vuole sapere quali applicazioni e tipi di applicazioni sono in uso da parte degli utenti?**

È possibile scaricare i report degli accessi degli ultimi 30 giorni da **portal.azure.com > Azure Active Directory> Accessi> scarica i report**.

- Informazioni su come [Concedere al tenant un ampio consenso amministratore per una applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) e [Configurare come gli utenti finali concedono l’autorizzazione alle applicazioni](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Informazioni su [come funziona l’autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) e [Gestire l’autorizzazione per le applicazioni](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


