---
title: Importare ed esportare da Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898052"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="28681-102">Importare ed esportare da Yammer</span><span class="sxs-lookup"><span data-stu-id="28681-102">Import and export from Yammer</span></span>

<span data-ttu-id="28681-103">**Importare**</span><span class="sxs-lookup"><span data-stu-id="28681-103">**Import**</span></span>

<span data-ttu-id="28681-104">Le opzioni di importazione utente variano a seconda che la rete Yammer sia disponibile o meno in [Modalità nativa per Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode).</span><span class="sxs-lookup"><span data-stu-id="28681-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="28681-105">**Modalità non nativa**: per importare gli utenti nei gruppi è necessario usare [Aggiungi dalla rubrica](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (massimo 100 utenti) nelle impostazioni del gruppo; per importare gli utenti nella rete, è invece necessario usare [Aggiorna in blocco](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) in Amministrazione rete.</span><span class="sxs-lookup"><span data-stu-id="28681-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="28681-106">**Modalità nativa**: le operazioni di iscrizione a gruppi o reti devono essere eseguite dal [portale di amministrazione di Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), dal [portale di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) oppure usando un'altra opzione di AD.</span><span class="sxs-lookup"><span data-stu-id="28681-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="28681-107">Le reti in modalità nativa non hanno più accesso all'opzione Aggiorna in blocco e ad altre funzionalità legacy.</span><span class="sxs-lookup"><span data-stu-id="28681-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="28681-108">Yammer non supporta mai l'importazione di contenuti da Amministrazione rete, neanche se la funzionalità di esportazione dati è stata usata in un'altra rete.</span><span class="sxs-lookup"><span data-stu-id="28681-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="28681-109">I contenuti possono essere ripubblicati da soluzioni dei partner o dalle API REST di Yammer.</span><span class="sxs-lookup"><span data-stu-id="28681-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="28681-110">**Esportare**</span><span class="sxs-lookup"><span data-stu-id="28681-110">**Export**</span></span>

<span data-ttu-id="28681-111">L'opzione [Esporta i dati della rete in Amministrazione rete](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) consente di esportare contenuti da reti Yammer, inclusi messaggi e file.</span><span class="sxs-lookup"><span data-stu-id="28681-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="28681-112">Poiché gli allegati possono essere di dimensioni notevoli, il completamento delle esportazioni potrebbe richiedere molto tempo.</span><span class="sxs-lookup"><span data-stu-id="28681-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="28681-113">È consigliabile esportare le reti attive usando l'[API di esportazione dati](https://developer.yammer.com/docs/data-export-api) in blocchi giornalieri o settimanali.</span><span class="sxs-lookup"><span data-stu-id="28681-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="28681-114">Il supporto tecnico Microsoft non fornisce script personalizzati per eseguire queste operazioni.</span><span class="sxs-lookup"><span data-stu-id="28681-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="28681-115">È disponibile un'apposita [esportazione GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) per esportare i contenuti per un singolo utente.</span><span class="sxs-lookup"><span data-stu-id="28681-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>