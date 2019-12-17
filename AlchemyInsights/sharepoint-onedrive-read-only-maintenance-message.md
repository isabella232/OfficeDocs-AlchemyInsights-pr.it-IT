---
title: Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051285"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="45cd4-102">Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="45cd4-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="45cd4-103">Gli utenti possono ricevere un messaggio di **sola lettura per la manutenzione** quando si tenta di utilizzare SharePoint o OneDrive per uno degli scenari seguenti.</span><span class="sxs-lookup"><span data-stu-id="45cd4-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="45cd4-104">Attività di manutenzione pianificata o attiva.</span><span class="sxs-lookup"><span data-stu-id="45cd4-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="45cd4-105">Verificarne la navigazione verso il [centro messaggi](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="45cd4-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="45cd4-106">Incidente di servizio attivo ad alta priorità che potrebbe verificarsi.</span><span class="sxs-lookup"><span data-stu-id="45cd4-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="45cd4-107">Controllare se sono presenti avvisi o eventi indesiderati per l'esplorazione dell' [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="45cd4-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="45cd4-108">Uno scenario di ripristino di correzione automatica secondario che potrebbe verificarsi a causa di eventuali eventi imprevisti nei server che potrebbero durare meno di 30 minuti.</span><span class="sxs-lookup"><span data-stu-id="45cd4-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="45cd4-109">Non sono disponibili messaggi di centro messaggi o di integrità dei servizi per questi rilevamenti di minore entità, ma è consigliabile tornare alla normalità molto presto.</span><span class="sxs-lookup"><span data-stu-id="45cd4-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="45cd4-110">In pochissime occasioni è stato osservato che uno dei tre scenari sopra elencati è stato la causa e il servizio è stato ripristinato, ma la cache del browser degli utenti non è stata cancellata.</span><span class="sxs-lookup"><span data-stu-id="45cd4-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="45cd4-111">Provare a cancellare la cache del browser prima di passare al sito.</span><span class="sxs-lookup"><span data-stu-id="45cd4-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="45cd4-112">Nel browser Microsoft Edge, selezionare **Impostazioni**, quindi selezionare **privacy e sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="45cd4-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="45cd4-113">In **Pulisci esplorazione**, seleziona **Scegli cosa cancellare**.</span><span class="sxs-lookup"><span data-stu-id="45cd4-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="45cd4-114">Selezionare **cookie e dati del sito Web salvati**e selezionare **Annulla**.</span><span class="sxs-lookup"><span data-stu-id="45cd4-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="45cd4-115">Questa procedura può essere diversa quando si utilizzano altri browser come Mozilla Firefox o Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="45cd4-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="45cd4-116">Un'altra opzione consiste nell'aprire il sito di SharePoint o OneDrive in una nuova finestra di InPrivate.</span><span class="sxs-lookup"><span data-stu-id="45cd4-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>