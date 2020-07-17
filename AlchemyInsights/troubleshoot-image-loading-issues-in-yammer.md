---
title: Risoluzione dei problemi di caricamento delle immagini in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146773"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="76cd0-102">Risoluzione dei problemi di caricamento delle immagini in Yammer</span><span class="sxs-lookup"><span data-stu-id="76cd0-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="76cd0-103">Se si verificano problemi con le anteprime di foto e file in Yammer, risolvere i problemi controllando se il problema avviene per tutti gli utenti, su dispositivi mobili e se è riproducibile durante il caricamento degli allegati.</span><span class="sxs-lookup"><span data-stu-id="76cd0-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="76cd0-104">**Problemi con la foto profilo**</span><span class="sxs-lookup"><span data-stu-id="76cd0-104">**Profile photo issues**</span></span>  

<span data-ttu-id="76cd0-105">Se gli utenti finali accedono a Yammer tramite Microsoft 365, devono cambiare il profilo, incluse le foto del profilo.</span><span class="sxs-lookup"><span data-stu-id="76cd0-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="76cd0-106">Se gli utenti non dispongono delle autorizzazioni per aggiornare il profilo, un amministratore potrà eseguire l'aggiornamento per conto loro.</span><span class="sxs-lookup"><span data-stu-id="76cd0-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="76cd0-107">Per ulteriori informazioni, vedere [Visualizzare e aggiornare il profilo in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="76cd0-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="76cd0-108">Per informazioni sulla modifica del profilo, incluse le foto del profilo, vedere [Cambiare il profilo e le impostazioni di Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="76cd0-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="76cd0-109">Le foto del profilo aggiornate vengono sincronizzate in modo diverso rispetto agli attributi del profilo.</span><span class="sxs-lookup"><span data-stu-id="76cd0-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="76cd0-110">Gli utenti devono accedere per avviare una sincronizzazione della foto del profilo.</span><span class="sxs-lookup"><span data-stu-id="76cd0-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="76cd0-111">Per informazioni, vedere [Le immagini del profilo vengono aggiornate da Office 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="76cd0-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="76cd0-112">Per informazioni sul ciclo di vita degli utenti per Yammer, vedere [Gestire gli utenti di Yammer per l'intero ciclo di vita da Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="76cd0-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="76cd0-113">Per informazioni dettagliate su come funziona la sincronizzazione delle immagini del profilo in Microsoft 365, vedere [Informazioni sulla sincronizzazione delle immagini del profilo in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="76cd0-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="76cd0-114">**Problemi relativi alle anteprime di documenti e miniature di immagini**</span><span class="sxs-lookup"><span data-stu-id="76cd0-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="76cd0-115">Quando file o immagini vengono pubblicati in Yammer, le anteprime potrebbero non essere visualizzate perché:</span><span class="sxs-lookup"><span data-stu-id="76cd0-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="76cd0-116">Il file è danneggiato e non può essere elaborato.</span><span class="sxs-lookup"><span data-stu-id="76cd0-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="76cd0-117">Il file non è stato caricato di recente in SharePoint Online o Yammer ha metadati non validi per altri motivi.</span><span class="sxs-lookup"><span data-stu-id="76cd0-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="76cd0-118">Gli URL necessari per caricare le immagini di anteprima sono bloccati.</span><span class="sxs-lookup"><span data-stu-id="76cd0-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="76cd0-119">L'anteprima del file è stata rimossa dall'utente prima di pubblicarla.</span><span class="sxs-lookup"><span data-stu-id="76cd0-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="76cd0-120">Un problema di servizio ha impedito la generazione di un'anteprima.</span><span class="sxs-lookup"><span data-stu-id="76cd0-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="76cd0-121">**Nota** Le anteprime per i collegamenti e i caricamenti di file potrebbero comportarsi in modo diverso.</span><span class="sxs-lookup"><span data-stu-id="76cd0-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="76cd0-122">È possibile che i collegamenti a file su Internet o collegamenti che richiedono ulteriore autenticazioni non vengano visualizzati correttamente.</span><span class="sxs-lookup"><span data-stu-id="76cd0-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="76cd0-123">Per altre informazioni, vedere [Allegare un file o un'immagine a un messaggio di Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="76cd0-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 