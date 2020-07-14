---
title: Autorizzazioni del calendario
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854008"
---
# <a name="calendar-permissions"></a><span data-ttu-id="601dc-102">Autorizzazioni del calendario</span><span class="sxs-lookup"><span data-stu-id="601dc-102">Calendar Permissions</span></span>

<span data-ttu-id="601dc-103">Gli utenti possono modificare le proprie autorizzazioni di calendario con Outlook sul Web o in altri client, ma anche come amministratore potrebbe essere necessario indagare.</span><span class="sxs-lookup"><span data-stu-id="601dc-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="601dc-104">Con il cmdlet di PowerShell di Exchange viene visualizzata l'autorizzazione per il calendario di un utente:</span><span class="sxs-lookup"><span data-stu-id="601dc-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="601dc-105">Per ulteriori informazioni, vedere quanto segue:</span><span class="sxs-lookup"><span data-stu-id="601dc-105">To see more information see the following:</span></span>

- [<span data-ttu-id="601dc-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="601dc-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="601dc-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="601dc-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="601dc-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="601dc-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="601dc-109">Le autorizzazioni del calendario vengono utilizzate nella condivisione dei calendari, per visualizzare ulteriori informazioni sulla condivisione di un calendario di Outlook, vedere gli articoli seguenti:</span><span class="sxs-lookup"><span data-stu-id="601dc-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="601dc-110">Condividere un calendario di Outlook con altri utenti</span><span class="sxs-lookup"><span data-stu-id="601dc-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="601dc-111">Condivisione del calendario in Outlook sul Web per le aziende</span><span class="sxs-lookup"><span data-stu-id="601dc-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="601dc-112">Per risolvere i problemi di autorizzazione del calendario, è possibile utilizzare lo strumento [Assistente supporto e ripristino](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="601dc-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>