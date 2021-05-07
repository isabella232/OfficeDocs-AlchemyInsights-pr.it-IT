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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233538"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="c18e8-102">Distribuzione di componenti aggiuntivi per Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="c18e8-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="c18e8-103">La distribuzione centralizzata è il modo consigliato per distribuire Office componenti aggiuntivi a utenti e gruppi all'interno dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="c18e8-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="c18e8-104">Per distribuire i componenti aggiuntivi, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="c18e8-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="c18e8-105">**Nota:** Per installare i componenti aggiuntivi per Office come singolo utente, vedere Visualizzare, gestire e installare i componenti aggiuntivi [nei Office applicazioni.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="c18e8-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="c18e8-106">Assicurati inoltre che sia abilitata l'acquisizione Office componenti aggiuntivi dello Store.</span><span class="sxs-lookup"><span data-stu-id="c18e8-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="c18e8-107">Per informazioni dettagliate, vedere [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span><span class="sxs-lookup"><span data-stu-id="c18e8-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="c18e8-108">Verificare che l'ambiente soddisfi i requisiti per la distribuzione di componenti aggiuntivi tramite distribuzione centralizzata.</span><span class="sxs-lookup"><span data-stu-id="c18e8-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="c18e8-109">Per informazioni dettagliate, vedere [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="c18e8-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="c18e8-110">Vai a **Impostazioni**  >  **App integrate** Ottieni  >  **app** nell'Microsoft 365 di amministrazione per distribuire i componenti aggiuntivi.</span><span class="sxs-lookup"><span data-stu-id="c18e8-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="c18e8-111">Note:</span><span class="sxs-lookup"><span data-stu-id="c18e8-111">Notes:</span></span> 

- <span data-ttu-id="c18e8-112">Le app integrate richiedono che l'amministratore abbia autorizzazioni di amministratore globale o Exchange amministratore.</span><span class="sxs-lookup"><span data-stu-id="c18e8-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="c18e8-113">Quando si distribuiscono componenti aggiuntivi a più utenti, è consigliabile eseguire assegnazioni utilizzando gruppi anziché singoli utenti.</span><span class="sxs-lookup"><span data-stu-id="c18e8-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="c18e8-114">Per informazioni dettagliate, [vedere Considerazioni sull'assegnazione di](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)un componente aggiuntivo a utenti e gruppi.</span><span class="sxs-lookup"><span data-stu-id="c18e8-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="c18e8-115">La distribuzione centralizzata non supporta gli utenti di gruppi annidati o gruppi con gruppi padre.</span><span class="sxs-lookup"><span data-stu-id="c18e8-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="c18e8-116">Per informazioni dettagliate, vedere [Assegnazioni di utenti e gruppi.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="c18e8-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="c18e8-117">Verificare che il servizio di gestione app di Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') sia abilitato agli utenti per l'accesso.</span><span class="sxs-lookup"><span data-stu-id="c18e8-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="c18e8-118">Per informazioni dettagliate, vedi [Configurare le proprietà dell'app.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="c18e8-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="c18e8-119">Se si verificano problemi di distribuzione dei componenti aggiuntivi tramite le app integrate, provare a eseguire la distribuzione utilizzando [Componenti aggiuntivi](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="c18e8-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="c18e8-120">Per ulteriori informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="c18e8-120">For more information, see:</span></span>

<span data-ttu-id="c18e8-121">[Distribuire componenti aggiuntivi nell'interfaccia di amministrazione](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gestire i componenti aggiuntivi nell'interfaccia di amministrazione](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizzare i cmdlet di PowerShell per la distribuzione centralizzata per gestire i componenti aggiuntivi](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Pubblicare Office componenti aggiuntivi con la](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) distribuzione centralizzata tramite l'Microsoft 365 di amministrazione 
 [Risoluzione dei problemi: l'utente non vede i componenti aggiuntivi](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Risolvere gli errori degli utenti Office componenti aggiuntivi](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="c18e8-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>