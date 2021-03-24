---
title: Trovare le applicazioni mancanti nel pannello Registrazione app
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123155"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Trovare le applicazioni mancanti nel pannello Registrazione app

1. Impossibile trovare le applicazioni nel portale di registrazione app.

    Se un'applicazione è un'applicazione multi-tenant ed è stata registrata in un altro tenant, non verrà visualizzata nel pannello Registrazione app. Tuttavia, è possibile trovarlo nel pannello Applicazioni aziendali dopo aver eseguito l'accesso (dopo essere stato autorizzato) e che l'entità servizio sia stata creata nel tenant. Per altre informazioni, vedi [App & entità servizio in Azure AD - Piattaforma di identità Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Impossibile visualizzare le app nel pannello Registrazione app anche se sei un amministratore.

    Assicurati di essere nella directory giusta nel portale di Azure.
3. L'applicazione non è elencata nel pannello Applicazioni aziendali, ma viene visualizzata quando si esegue una query sul comando di PowerShell.

    A volte, dopo aver eliminato l'applicazione dal portale di Azure, l'applicazione non viene mostrata nel portale, ma potrebbe non essere stata eliminata completamente. Per ulteriori informazioni, vedere:
    - È possibile recuperare l'elenco delle applicazioni eliminate in precedenza e vedere se l'applicazione viene visualizzata nell'elenco utilizzando il comando powershell: **Get-AzureADDeletedApplication**. Per altre informazioni, vedere [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Se si desidera rimuovere completamente l'applicazione, è possibile provare quanto segue in PowerShell: **Remove-AzureADApplication -ObjectId**. Per ulteriori informazioni, vedere [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - In alternativa, è possibile provare a ripristinare l'applicazione eliminata utilizzando il comando powershell seguente: **Restore AzureADDeletedApplication -ObjectId**. Per ulteriori informazioni, vedere [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Impossibile trovare l'elenco di tutte le applicazioni aziendali preinstallato nel nuovo tenant di Azure.

    Non ci sono applicazioni aziendali preinstallato in Azure AD per impostazione predefinita. È necessario aggiungerlo manualmente dall'opzione "Nuova applicazione" esplorando l'applicazione dalla raccolta di Azure AD o aggiungere un'applicazione non raccolta. Per altre informazioni, vedere [Guida introduttiva: Aggiungere un'applicazione al tenant di Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Gli amministratori globali possono accedere facilmente alle app usando l'icona di avvio delle app di [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Impossibile trovare le app dal portale app personali.

    Assicurati che le app non siano nascoste nella pagina Raccolta app personali. Per altre informazioni, vedi [Raccolte (anteprima) nel portale App personali - Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Per avviare le app dal portale App personali, vedere Individuare & usare le app nel portale App personali [- Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. L'app Office 365 Mover non viene visualizzata nel pannello Applicazioni aziendali dopo l'installazione.

    L'applicazione "Office 365 Mover" è un'app multitenant che non deve essere aggiunta ad AAD usando la sezione Applicazioni della raccolta in Registrazione app aziendali. Per accedere all'app Mover di Office 365, accedi semplicemente all'app e richiede il consenso dell'utente per le autorizzazioni. Una volta che l'utente fornisce il consenso, questa app viene aggiunta automaticamente al tenant con l'ID di posta elettronica che hai effettuato l'accesso.

    Dopo aver effettuato l'accesso all'applicazione, dovresti essere in grado di trovare la voce dell'applicazione nel pannello delle applicazioni aziendali in AAD. È necessario cercare l'applicazione digitando il nome completo, ad esempio "Office 365 Mover" o semplicemente "office" e dovrebbe elencare l'app. Per ulteriori informazioni, vedere [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)che è già installato ma non è elencato nella raccolta di applicazioni aziendali.
8. [Guida introduttiva:](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) visualizzare l'elenco delle applicazioni che usano il tenant di Azure Active Directory (Azure AD) per la gestione delle identità mostra come visualizzare le applicazioni, note anche come app, già impostate per l'uso del tenant di Azure AD come provider di identità (IdP).
9. [La risoluzione dei problemi comuni relativi all'aggiunta](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) o alla rimozione di un'applicazione in Azure Active Directory consente di comprendere i problemi comuni che gli utenti devono affrontare durante la visualizzazione delle app in Azure Active Directory.
