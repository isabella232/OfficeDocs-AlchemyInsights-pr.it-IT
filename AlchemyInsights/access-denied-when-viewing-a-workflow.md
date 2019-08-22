---
title: Accesso negato durante la visualizzazione di un flusso di lavoro
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495827"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="666f6-102">Accesso negato durante la visualizzazione di un flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="666f6-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="666f6-103">I flussi di lavoro di SharePoint 2013 che tentano di inviare un messaggio di posta elettronica a un gruppo di SharePoint non possono avere esito positivo se l'appartenenza al gruppo di SharePoint non è impostata su tutti.</span><span class="sxs-lookup"><span data-stu-id="666f6-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="666f6-104">**Per risolvere il problema, eseguire la procedura seguente:**</span><span class="sxs-lookup"><span data-stu-id="666f6-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="666f6-105">Consentire a tutti di visualizzare i membri del gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="666f6-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="666f6-106">Rimuovere il gruppo di SharePoint dalla riga a o CC del messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="666f6-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="666f6-107">Aggiungere in modo esplicito gli utenti alla riga a o CC se la visibilità di appartenenza non può essere modificata per il gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="666f6-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="666f6-108">Per visualizzare ulteriori dettagli, fare riferimento a [http non autorizzato a/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="666f6-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  