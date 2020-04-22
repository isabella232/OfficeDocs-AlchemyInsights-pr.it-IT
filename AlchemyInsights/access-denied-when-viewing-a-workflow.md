---
title: Accesso negato durante la visualizzazione di un flusso di lavoro
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687334"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="41a3c-102">Accesso negato durante la visualizzazione di un flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="41a3c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="41a3c-103">I flussi di lavoro di SharePoint 2013 che tentano di inviare un messaggio di posta elettronica a un gruppo di SharePoint non possono avere esito positivo se l'appartenenza al gruppo di SharePoint non è impostata su tutti.</span><span class="sxs-lookup"><span data-stu-id="41a3c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="41a3c-104">**Per risolvere il problema, eseguire la procedura seguente:**</span><span class="sxs-lookup"><span data-stu-id="41a3c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="41a3c-105">Consentire a tutti di visualizzare i membri del gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41a3c-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="41a3c-106">Rimuovere il gruppo di SharePoint dalla riga a o CC del messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="41a3c-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="41a3c-107">Aggiungere in modo esplicito gli utenti alla riga a o CC se la visibilità di appartenenza non può essere modificata per il gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41a3c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="41a3c-108">Per visualizzare ulteriori dettagli, fare riferimento a [http non autorizzato a/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="41a3c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  