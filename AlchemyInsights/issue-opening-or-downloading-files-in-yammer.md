---
title: Problemi nell'aprire o scaricare file in Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146818"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="4c159-102">Problemi nell'aprire o scaricare file in Yammer</span><span class="sxs-lookup"><span data-stu-id="4c159-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="4c159-103">Classic Yammer supporta più opzioni per caricare i file in messaggi e gruppi.</span><span class="sxs-lookup"><span data-stu-id="4c159-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="4c159-104">A seconda della configurazione della rete, per impostazione predefinita i file vengono archiviati in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4c159-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="4c159-105">La selezione file nel nuovo Yammer non supporta ancora tutte le opzioni disponibili nella versione classica di Yammer.</span><span class="sxs-lookup"><span data-stu-id="4c159-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="4c159-106">Un aggiornamento futuro aggiungerà altre funzionalità.</span><span class="sxs-lookup"><span data-stu-id="4c159-106">A future update will add additional features.</span></span> <span data-ttu-id="4c159-107">Per altre informazioni, vedere [Allegare un file o un'immagine a un post di conversazione di Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="4c159-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="4c159-108">**Non è possibile aprire o scaricare un file**</span><span class="sxs-lookup"><span data-stu-id="4c159-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="4c159-109">Un file può essere caricato in Yammer, ma è anche possibile creare un collegamento a un file in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4c159-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="4c159-110">Per risolvere il problema, è necessario prima di tutto determinare il percorso del file.</span><span class="sxs-lookup"><span data-stu-id="4c159-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="4c159-111">Se il file è stato caricato in Yammer, avrà un URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="4c159-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="4c159-112">Assicurarsi che gli URL e gli indirizzi IP necessari vengano sbloccati.</span><span class="sxs-lookup"><span data-stu-id="4c159-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="4c159-113">Per altre informazioni, vedere il post di blog [Usare gli indirizzi IP hardcoded per Yammer non è consigliabile](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="4c159-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="4c159-114">Verificare se un utente che è anche un amministratore globale può scaricare il file.</span><span class="sxs-lookup"><span data-stu-id="4c159-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="4c159-115">Se il file è privato, potrebbe essere necessario usare la Modalità contenuto privato.</span><span class="sxs-lookup"><span data-stu-id="4c159-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="4c159-116">Per altre informazioni, vedere [Monitorare il contenuto privato in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="4c159-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="4c159-117">**Guest e file di Yammer a livello di rete in SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="4c159-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="4c159-118">[Gli utenti Guest a livello di rete in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) non usano Azure AD B2B e sono interni al servizio Yammer, quindi non possono accedere ai file di Yammer archiviati in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4c159-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="4c159-119">Creare un utente AAD B2B esterno che possa accedere alle raccolte documenti in SharePoint Online usando tale identità.</span><span class="sxs-lookup"><span data-stu-id="4c159-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="4c159-120">Per informazioni sul supporto futuro per guest di Azure AD B2B in Yammer, vedere [Supporto business-to-business (B2B) nell'anteprima di Yammer: condizioni per i clienti e domande frequenti](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="4c159-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>