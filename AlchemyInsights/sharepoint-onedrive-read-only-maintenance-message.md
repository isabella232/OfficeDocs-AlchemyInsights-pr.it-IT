---
title: Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840519"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="6c4ba-102">Di sola lettura per il messaggio di manutenzione quando si tenta di utilizzare SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="6c4ba-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="6c4ba-103">Gli utenti possono ricevere un messaggio **di sola lettura per la manutenzione** quando si tenta di utilizzare SharePoint o OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="6c4ba-104">In caso affermativo, controllare se è presente una manutenzione attiva sul tenant passando al [centro messaggi](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="6c4ba-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="6c4ba-105">Assicurarsi inoltre di controllare il dashboard dell' [integrità del servizio](https://portal.office.com/adminportal/home#/servicehealth) per verificare la disponibilità di eventuali avvisi/incidenti che potrebbero verificarsi.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="6c4ba-106">Se né il centro messaggi o il dashboard di integrità del servizio hanno rilevato nulla sulla manutenzione corrente per il tenant, potrebbe trattarsi di un problema relativo alla memorizzazione nella cache del browser.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="6c4ba-107">Provare a cancellare la cache del browser prima di passare al sito.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="6c4ba-108">Nel browser Microsoft Edge, selezionare **Impostazioni**, quindi selezionare **privacy e sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="6c4ba-109">In **Pulisci esplorazione**, seleziona **Scegli cosa cancellare**.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="6c4ba-110">Selezionare **cookie e dati del sito Web salvati**e selezionare **Annulla**.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="6c4ba-111">Questa procedura può essere diversa quando si utilizzano altri browser come Mozilla Firefox o Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="6c4ba-112">Un'altra opzione consiste nell'aprire il sito di SharePoint o OneDrive in una nuova finestra di InPrivate.</span><span class="sxs-lookup"><span data-stu-id="6c4ba-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>