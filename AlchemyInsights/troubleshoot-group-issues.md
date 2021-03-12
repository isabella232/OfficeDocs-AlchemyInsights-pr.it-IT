---
title: Risoluzione dei problemi dei gruppi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716109"
---
# <a name="troubleshoot-group-issues"></a>Risoluzione dei problemi dei gruppi

**È necessario assegnare un gruppo ad un ruolo di Azure AD**

Per assegnare a un gruppo Azure Active Directory (AD) ad un ruolo Azure AD, seguire i seguenti passaggi:

1. Creare un nuovo gruppo - Per creare un nuovo gruppo:

    a. Accedere all'interfaccia di amministrazione di Azure AD con un ruolo di amministratore con privilegi o con autorizzazioni di amministratore globale. 
    b. Selezionare Azure Active Directory > Gruppi> Tutti i gruppi > Nuovo gruppo. 
    c. Creare il gruppo.

2. Assegnare il ruolo al gruppo durante la creazione del gruppo o in seguito alla sua creazione.

    a. Per assegnare un ruolo al gruppo al momento della creazione del gruppo, passare ad attivare/disattivare I ruoli Azure AD possono essere assegnati al gruppo e creare il gruppo.
    b. Per assegnare un ruolo al gruppo in seguito alla sua creazione, passare alla scheda Ruoli assegnati per il gruppo appena creato e assegnare il ruolo al gruppo.

**È necessario gestire l'appartenenza di un gruppo che è stato assegnato ad un ruolo Azure AD**

1. Per impostazione predefinita, per evitare l'elevazione dei privilegi, solo gli amministratori con ruoli di privilegio e gli amministratori globali possono modificare l'appartenenza di un gruppo che è stato assegnato ad un ruolo. Tuttavia, possono scegliere di assegnare un proprietario per tale gruppo e delegare questa attività. Per ulteriori informazioni vedere, [Usare i gruppi cloud per gestire le assegnazioni di ruolo in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Per domande comuni e suggerimenti per la risoluzione dei problemi per l'assegnazione di ruoli ai gruppi in Azure AD, vedere [Risoluzione dei problemi relativi ai ruoli assegnati a gruppi cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Gruppi dinamici**

1. Se non si riescono a trovare gli attributi utente predefiniti, verificare che l'attributo sia presente nell'elenco delle proprietà supportate.
2. Se si cercano attributi predefiniti per i dispositivi, assicurarsi che l'attributo sia nell'elenco degli attributi del dispositivo 
3. Oltre agli attributi predefiniti per utenti e dispositivi, è anche possibile usare [Attributi dell'estensione](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Dopo la sincronizzazione degli attributi di estensione da AD di Windows Server locale o da un'applicazione SaaS connessa, gli attributi dovrebbero essere visibili nell'elenco a discesa del generatore di regole. Il nome dell'attributo personalizzato è disponibile nell’elenco eseguendo una ricerca sull'attributo di un utente con PowerShell e cercando il nome dell'attributo. Possono essere usate anche quando si creano regole nella sintassi delle regole.
4. Verificare che il tenant abbia la licenza appropriata. I gruppi dinamici richiedono che il tenant abbia una licenza di Azure AD P1 Premium. L'elenco dei piani di licenza di Azure AD è accessibile [qui](https://azure.microsoft.com/pricing/details/active-directory/). I piani di licenza per Enterprise Mobility + Security sono accessibili [qui](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Assicurarsi che il ruolo dell'utente che crea il gruppo dinamico sia un amministratore globale, un amministratore di intune, un amministratore di gruppo o un amministratore utente.
6. Si prega di attendere per consentire il popolamento del gruppo. A seconda delle dimensioni del tenant, il popolamento del gruppo può richiedere fino a 24 ore per la prima volta o dopo la modifica di una regola.
7. Per altre informazioni, vedere [Creare regole basate su attributo per l'appartenenza dinamica ai gruppi](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Come eliminare un gruppo**

1. I gruppi possono essere eliminati dalla directory usando il cmdlet Remove-AzureADGroup nel modulo Azure AD Powershell.
2. Prima di provare a eliminare un gruppo sincronizzato in Azure AD, assicurarsi di aver eliminato tutte le licenze assegnate per evitare errori.
3. Per altre informazioni sull'eliminazione di gruppi, vedere ['eliminazione di un gruppo con una licenza assegnata](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Ripristinare un gruppo eliminato**

1. Se un gruppo di Office 365 viene eliminato, può essere ripristinato solo entro 30 giorni, prima dell'eliminazione definitiva. Una volta eliminato definitivamente, il gruppo non può più essere ripristinato. Altre informazione sul ripristino dei gruppi [qui](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Questa funzionalità non è supportata per i gruppi di sicurezza e i gruppi di distribuzione.
3. Assicurarsi di essere autorizzati a ripristinare un gruppo di Office 365. Gli amministratori globali, gli amministratori di gruppo, gli amministratori degli account utente, gli amministratori dei servizi intune, il supporto dei partner di livello 1 o di livello 2 e il proprietario del gruppo possono essere in grado di ripristinare un gruppo.
4. Quando un gruppo dinamico viene eliminato e poi ripristinato, viene visualizzato come un nuovo gruppo e popolato di nuovo in base alla regola. Questo processo potrebbe richiedere fino a 24 ore.
5. Per ulteriori informazioni su come ripristinare un gruppo eliminato, vedere [Ripristinare un gruppo di Microsoft 365 eliminato in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configurazione dei criteri di scadenza dei gruppi**

1. Questa funzionalità è supportata solo per i gruppi di Office 365, non è supportata per i gruppi di sicurezza e i gruppi di distribuzione.
2. Per configurare e usare i criteri di scadenza per i gruppi di Office 365 è necessaria una licenza di Azure AD Premium.
3. Attualmente è possibile configurare un solo criterio di scadenza per i gruppi di Office 365 in un tenant.
4. Solo gli amministratori globali, gli amministratori di gruppo, gli amministratori utente e il proprietario del gruppo possono rinnovare un gruppo.
5. Se un gruppo di Office 365 è scaduto, può essere ripristinato solo entro 30 giorni, prima dell'eliminazione definitiva. Una volta eliminato definitivamente, il gruppo non può più essere ripristinato. Altre informazione sul ripristino dei gruppi [qui](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Rinnovo automatico basato su attività**

Le attività degli utenti da SharePoint, Outlook e Teams possono attivare il rinnovo automatico di gruppo. Le attività vengono controllate a 35 giorni prima della scadenza di un gruppo. Se ci sono attività durante il ciclo di vita del gruppo corrente, il gruppo verrà rinnovato automaticamente e non verrà inviata una notifica tramite posta elettronica ai proprietari del gruppo.

**Intervallo di notifica per i gruppi scaduti**

1. Le notifiche vengono inviate ai proprietari del gruppo di Office 365 tramite posta elettronica 30 giorni, 15 giorni e 1 giorno prima della scadenza del gruppo.
2. Quando si configura la scadenza per la prima volta, tutti i gruppi precedenti all'intervallo di scadenza vengono impostati su 35 giorni fino alla scadenza.
3. La data di scadenza del gruppo viene calcolata in base alla data di rinnovo del gruppo, non in base alla data di aggiornamento dei criteri. Se i criteri di scadenza vengono aggiornati, la data di scadenza non viene cambiata.
4. Per altre informazioni, vedere, [Criteri di scadenza dei gruppi e messaggi di posta elettronica di rinnovo](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) e [Ripristinare un gruppo di Office 365 eliminato in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Autorizzazione per creare un gruppo**

Verificare che si disponga dell'autorizzazione per creare un nuovo gruppo. Gli amministratori globali possono disabilitare la creazione di gruppi nel portale di Azure o nel riquadro di accesso. Potrebbe essere necessario un amministratore per creare il nuovo gruppo o per farsi assegnare le autorizzazioni appropriate.

1. [Creare un nuovo gruppo e aggiungere membri nel portale di Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Creare gruppi in Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Disabilitare la creazione di gruppi in Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Gestire chi può creare i gruppi di Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Disabilitare la notifica di benvenuto di Office 365 tramite Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Ruoli amministrativi di Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Gestire le autorizzazioni per la creazione di gruppi**

1. Gli amministratori globali possono gestire le autorizzazioni di creazione di gruppi di sicurezza o di Office 365 creati nel portale di Azure o nel riquadro di accesso. Tramite l'impostazione **Gli utenti possono creare gruppi di sicurezza nei portali di Azure** o **Gli utenti possono creare gruppi di Office 365 nei portali di Azure** in **Tutti i gruppi > Generale (impostazioni)**.
2. È anche possibile limitare la creazione di gruppi a uno specifico gruppo di utenti se si ha una licenza di Azure AD P1 Premium.

**Disabilitazione della notifica di benvenuto per i nuovi membri di un gruppo di Office 365**

La notifica di benvenuto inviata agli utenti aggiunti ai gruppi di Office 365 può essere disabilitata impostando `UnifiedGroupWelcomeMessageEnabled` su **Falso** in Powershell. Altre informazioni su questa impostazione [qui](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













