---
title: 1336 cartella RecoverableItems piena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720256"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="202de-102">La cartella elementi ripristinabili è piena</span><span class="sxs-lookup"><span data-stu-id="202de-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="202de-103">Per le cassette postali di Exchange Online, il limite di archiviazione predefinito per la cartella elementi ripristinabili è 30 GB.</span><span class="sxs-lookup"><span data-stu-id="202de-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="202de-104">Il limite di archiviazione per la cartella elementi ripristinabili viene automaticamente aumentato a 100 GB se la cassetta postale è impostata su blocco per controversia legale, eDiscovery Hold o viene assegnata a un criterio di conservazione.</span><span class="sxs-lookup"><span data-stu-id="202de-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="202de-105">Quando la cartella elementi ripristinabili raggiunge il limite di archiviazione, la funzionalità delle cassette postali viene modificata nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="202de-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="202de-106">L'utente non può eliminare gli elementi dalla cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="202de-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="202de-107">Assistente cartelle gestite non può eliminare elementi basandosi sul tag di conservazione o sulle impostazioni delle cartelle gestite.</span><span class="sxs-lookup"><span data-stu-id="202de-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="202de-108">Per le cassette postali a cui è stato abilitato il ripristino di un singolo elemento o che vengono bloccate, il processo di protezione delle pagine copy-on-Write non è in grado di gestire le versioni degli elementi modificati dall'utente</span><span class="sxs-lookup"><span data-stu-id="202de-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="202de-109">Per le cassette postali in cui è abilitata la registrazione di controllo delle cassette postali, non è possibile salvare le voci del registro di controllo della cassetta postale nella cartella elementi ripristinabili.</span><span class="sxs-lookup"><span data-stu-id="202de-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="202de-110">Per le cassette postali che non sono in attesa, gli `Search-Mailbox -SearchDumpsterOnly -DeleteContent` amministratori possono utilizzare il comando in PowerShell di Exchange Online per eliminare gli elementi nella cartella elementi ripristinabili.</span><span class="sxs-lookup"><span data-stu-id="202de-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="202de-111">Per ulteriori informazioni, vedere i seguenti argomenti:</span><span class="sxs-lookup"><span data-stu-id="202de-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="202de-112">Cercare ed eliminare i messaggi</span><span class="sxs-lookup"><span data-stu-id="202de-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="202de-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="202de-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="202de-114">Per le cassette postali che sono in attesa, gli amministratori devono rimuovere il blocco prima che possano eliminare gli elementi dalla cartella elementi ripristinabili.</span><span class="sxs-lookup"><span data-stu-id="202de-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="202de-115">Per ulteriori informazioni, vedere [eliminare gli elementi nella cartella elementi ripristinabili delle cassette postali basate sul cloud in attesa](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="202de-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="202de-116">Per evitare che la cartella elementi ripristinabili diventi completa, gli amministratori possono aumentare il limite di archiviazione della cartella elementi ripristinabili per le cassette postali in attesa e impostare un criterio di conservazione delle cassette postali che sposta gli elementi dalla cartella elementi ripristinabili alla cassetta postale di archiviazione dell'utente.</span><span class="sxs-lookup"><span data-stu-id="202de-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="202de-117">Vedere [aumentare la quota degli elementi ripristinabili per le cassette postali in blocco](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="202de-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
