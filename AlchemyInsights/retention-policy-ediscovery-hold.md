---
title: 2609-conservazione-o-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994074"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="1ae38-102">Impossibile eliminare gli elementi in SharePoint Online o OneDrive for business</span><span class="sxs-lookup"><span data-stu-id="1ae38-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="1ae38-103">L'utente o gli utenti potrebbero non essere in grado di eliminare gli elementi in SharePoint Online o OneDrive for business perché un criterio di conservazione, un'etichetta di conservazione o un blocco eDiscovery viene applicato a un SharePoint del sito di OneDrive o a un elemento specifico.</span><span class="sxs-lookup"><span data-stu-id="1ae38-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="1ae38-104">Ciò include la possibilità di eliminare un documento, una versione di un documento, una cartella, una raccolta documenti, un elenco, un'app, un sito o una raccolta siti.</span><span class="sxs-lookup"><span data-stu-id="1ae38-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="1ae38-105">Di seguito sono riportati alcuni esempi dei messaggi di errore che possono essere ricevuti se si tenta di eliminare un elemento che viene conservato:</span><span class="sxs-lookup"><span data-stu-id="1ae38-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="1ae38-106">"Questo sito non può essere eliminato perché è incluso in un criterio di conservazione o blocco di eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="1ae38-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="1ae38-107">"Questo sito ha un criterio di conformità impostato per bloccare l'eliminazione"</span><span class="sxs-lookup"><span data-stu-id="1ae38-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="1ae38-108">"Un criterio di conformità sta attualmente bloccando l'eliminazione di questo sito"</span><span class="sxs-lookup"><span data-stu-id="1ae38-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="1ae38-109">"Questa raccolta siti non può essere eliminata perché contiene siti inclusi in un criterio di conservazione o blocco di eDiscovery"</span><span class="sxs-lookup"><span data-stu-id="1ae38-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="1ae38-110">"È necessario eliminare tutti gli elementi presenti in questa cartella prima di eliminare la cartella"</span><span class="sxs-lookup"><span data-stu-id="1ae38-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="1ae38-111">"Le versioni di questo elemento non possono essere eliminate perché è in attesa o criteri di conservazione"</span><span class="sxs-lookup"><span data-stu-id="1ae38-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="1ae38-112">"L'elemento non può essere eliminato mentre è in attesa"</span><span class="sxs-lookup"><span data-stu-id="1ae38-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="1ae38-113">"L'etichetta applicata a questo elemento impedisce la modifica o l'eliminazione"</span><span class="sxs-lookup"><span data-stu-id="1ae38-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="1ae38-114">"L'elenco non può essere eliminato durante il blocco o il criterio di conservazione"</span><span class="sxs-lookup"><span data-stu-id="1ae38-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="1ae38-115">"L'elenco non può essere eliminato se è bloccato o se è stato applicato un criterio di conservazione"</span><span class="sxs-lookup"><span data-stu-id="1ae38-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="1ae38-116">Per eliminare gli elementi in uno di questi scenari, è necessario rimuovere il criterio di conservazione, l'etichetta di conservazione o il blocco eDiscovery (oppure è necessario escludere un sito da un criterio di conservazione).</span><span class="sxs-lookup"><span data-stu-id="1ae38-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="1ae38-117">È necessario disabilitare o escludere il blocco corrispondente che causa questo problema.</span><span class="sxs-lookup"><span data-stu-id="1ae38-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="1ae38-118">Dopo la rimozione di un criterio di conservazione o di un blocco, potrebbero essere necessarie fino a 24 ore per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="1ae38-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="1ae38-119">Per informazioni sulle diverse funzionalità di conservazione e archiviazione che è possibile applicare a siti di SharePoint e account di OneDrive, vedere uno degli argomenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="1ae38-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="1ae38-120">Panoramica dei criteri di conservazione</span><span class="sxs-lookup"><span data-stu-id="1ae38-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="1ae38-121">Panoramica delle etichette di conservazione</span><span class="sxs-lookup"><span data-stu-id="1ae38-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="1ae38-122">Gestione delle esenzioni in Advanced eDiscovery</span><span class="sxs-lookup"><span data-stu-id="1ae38-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="1ae38-123">eDiscovery contiene</span><span class="sxs-lookup"><span data-stu-id="1ae38-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="1ae38-124">Criteri di eliminazione e chiusura dei siti legacy</span><span class="sxs-lookup"><span data-stu-id="1ae38-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
