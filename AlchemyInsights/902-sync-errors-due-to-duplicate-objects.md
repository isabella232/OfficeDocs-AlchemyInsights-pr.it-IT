---
title: 902 (gli errori di sincronizzazione a causa di oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919876"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="04aeb-102">Errori di sincronizzazione a causa di oggetti duplicati</span><span class="sxs-lookup"><span data-stu-id="04aeb-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="04aeb-103">Al termine della sincronizzazione della directory, è possibile ricevere uno dei seguenti messaggi di errore:</span><span class="sxs-lookup"><span data-stu-id="04aeb-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="04aeb-104">Non è possibile aggiornare l'oggetto in Microsoft Online Services, in quanto gli attributi seguenti associati all'oggetto hanno i valori che possono essere già associati a un altro oggetto nella directory locale.</span><span class="sxs-lookup"><span data-stu-id="04aeb-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="04aeb-105">Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory di Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="04aeb-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="04aeb-106">Non è possibile aggiornare l'oggetto perché i seguenti attributi associati all'oggetto dispongono di valori che possono essere già associati a un altro oggetto in servizi directory locale: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="04aeb-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="04aeb-107">Per identificare e correggere il problema, scaricare ed eseguire lo [Strumento di risoluzione dei problemi di IdFix DirSync errore](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="04aeb-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="04aeb-108">Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="04aeb-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

