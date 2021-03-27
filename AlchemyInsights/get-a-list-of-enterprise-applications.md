---
title: Ottenere un elenco di applicazioni aziendali
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379850"
---
# <a name="get-a-list-of-enterprise-applications"></a>Ottenere un elenco di applicazioni aziendali

1. Per **ottenere un elenco** di applicazioni aziendali (tutte le applicazioni o filtrate per nome visualizzato, ID, URI identificatore e così via) tramite il comando powershell, vedere [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Per ottenere un elenco di oggetti entità servizio (tutti gli oggetti o filtrati in base all'ID) tramite il comando powershell, vedere [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Se si desidera ottenere **un elenco delle app configurate saml, gli script di PowerShell** seguenti possono essere utili:

    Ogni applicazione che si tratta di un'app OAuth o SAML (sia app di raccolta che di app non di raccolta) avrebbe due oggetti creati in AAD quando viene eseguita la registrazione. Uno è denominato oggetto Application e l'altro è l'oggetto Entità servizio. Quando si esegue il dump delle proprietà di un oggetto entità servizio tramite PowerShell, si scoprirebbe che a ogni applicazione è associato un determinato numero di tag, ad esempio:

    - Le app OAuth avrebbero un tag denominato "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Raccolta App SAML con un tag denominato "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Le app SAML non della raccolta avrebbero un tag denominato "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Di conseguenza, puoi usare questi tag e scoprire che tipo di app si tratta. Il tag "**WindowsAzureActiveDirectoryIntegratedApp**" è comune a tutti i tipi di app. Puoi usare il frammento di codice seguente per elencare tutte le app SAML (sia raccolta che non raccolta):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Per altre informazioni, vedi [Identificare le app abilitate per SAML in Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Trovare ed elencare solo le applicazioni Web:** utilizzare il comando seguente per ottenere tutte le applicazioni di Azure AD con il tipo di applicazione "App Web/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Trovare ed elencare solo le** applicazioni native: eseguire il comando seguente per ottenere tutte le applicazioni client native (desktop/dispositivo mobile).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Export All Registered Azure AD Application Details to CSV**: Il comando seguente esporta tutte le app di Azure AD con i dettagli necessari in un file CSV:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Necessità di esportare un elenco di app di Azure inutilizzate** - Report di controllo

    Azure AD può visualizzare i log delle applicazioni solo per un massimo di 30 giorni, purché si abbia una licenza di Azure AD Premium.
    Sono disponibili due opzioni per conservare i dati per più di 30 giorni. Puoi usare le [API per la creazione di report](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) di Azure AD per recuperare i dati a livello di programmazione e archiviarli in un database. In alternativa, è possibile integrare i log di controllo in un sistema SIEM di terze parti.

    Puoi anche scaricare l'elenco delle app per tutte le applicazioni e le applicazioni di proprietà in Azure Active directory>App Registrations>Download>Tutte le applicazioni/Applicazioni di proprietà.

    Per ottenere un elenco delle applicazioni tramite MS Graph, vedere [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and application resource type - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application).
