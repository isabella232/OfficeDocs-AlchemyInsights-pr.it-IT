---
title: 902 (errori di sincronizzazione a causa di oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420894"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="764c8-102">Errori di sincronizzazione a causa di oggetti duplicati</span><span class="sxs-lookup"><span data-stu-id="764c8-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="764c8-103">Quando la sincronizzazione della directory viene completata, potrebbe essere visualizzato uno dei seguenti messaggi di errore:</span><span class="sxs-lookup"><span data-stu-id="764c8-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="764c8-104">Impossibile aggiornare l'oggetto nei servizi Microsoft online perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nella directory locale.</span><span class="sxs-lookup"><span data-stu-id="764c8-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="764c8-105">Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory dei Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="764c8-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="764c8-106">Non è possibile aggiornare l'oggetto perché i seguenti attributi associati a questo oggetto dispongono di valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="764c8-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="764c8-107">Per identificare e risolvere il problema, scaricare ed eseguire lo strumento di correzione degli [errori di IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="764c8-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="764c8-108">Per ulteriori informazioni, vedere [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="764c8-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
