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
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918832"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="eb2ae-102">Accesso negato durante la visualizzazione di un flusso di lavoro</span><span class="sxs-lookup"><span data-stu-id="eb2ae-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="eb2ae-103">SharePoint 2013 i flussi di lavoro tenta di inviare un messaggio di posta elettronica a un gruppo di SharePoint può non riuscire con un messaggio di errore "Accesso negato" se l'appartenenza del gruppo di SharePoint non è impostata su tutti gli utenti.</span><span class="sxs-lookup"><span data-stu-id="eb2ae-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="eb2ae-104">**Per risolvere questo problema, eseguire la procedura seguente:**</span><span class="sxs-lookup"><span data-stu-id="eb2ae-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="eb2ae-105">Consentire a tutti i partecipanti di visualizzare i membri del gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb2ae-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="eb2ae-106">Rimuovere il gruppo di SharePoint da a o CC riga del messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="eb2ae-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="eb2ae-107">Aggiungere esplicitamente gli utenti a o CC linea se non può essere modificata la visibilità l'appartenenza al gruppo di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eb2ae-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="eb2ae-108">Per visualizzare ulteriori informazioni, consultare [HTTP non autorizzato a /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="eb2ae-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

