---
title: Pensionamento dei servizi di accesso
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747788"
---
# <a name="access-services-retirement"></a><span data-ttu-id="db9e8-102">Pensionamento dei servizi di accesso</span><span class="sxs-lookup"><span data-stu-id="db9e8-102">Access services retirement</span></span>

<span data-ttu-id="db9e8-103">Come annunciato originariamente in MC97576, nel marzo 2017, e ha continuato a comunicare negli ultimi anni, i servizi di accesso vengono ritirati da Office 365.</span><span class="sxs-lookup"><span data-stu-id="db9e8-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="db9e8-104">La fase successiva di questo processo sarà la rimozione dei database di Access Web che utilizzano gli elenchi di SharePoint come archivio dati sottostante.</span><span class="sxs-lookup"><span data-stu-id="db9e8-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="db9e8-105">**In che modo questo ha effetto su di me?**</span><span class="sxs-lookup"><span data-stu-id="db9e8-105">**How does this affect me?**</span></span>

<span data-ttu-id="db9e8-106">A partire da giugno 2019, si smetterà di creare nuovi database di Access in SharePoint Online e arrestare il servizio e le eventuali app restanti entro il 2020 aprile.</span><span class="sxs-lookup"><span data-stu-id="db9e8-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="db9e8-107">**Che cosa è necessario fare per prepararsi a questa modifica?**</span><span class="sxs-lookup"><span data-stu-id="db9e8-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="db9e8-108">Si consiglia di creare un piano di transizione per i database Web di Access dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="db9e8-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="db9e8-109">Gli amministratori possono utilizzare lo [scanner app di SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) per ottenere un inventario delle app di Access utilizzate dai siti.</span><span class="sxs-lookup"><span data-stu-id="db9e8-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="db9e8-110">Esistono diversi modi per eseguire la migrazione dei dati di Access Web database:</span><span class="sxs-lookup"><span data-stu-id="db9e8-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="db9e8-111">Importazione in un database di Access locale (. ACCDB) o in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="db9e8-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="db9e8-112">È inoltre consigliabile esplorare Microsoft PowerApps come piattaforma alternativa per creare soluzioni aziendali senza codice per dispositivi mobili e Web.</span><span class="sxs-lookup"><span data-stu-id="db9e8-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>