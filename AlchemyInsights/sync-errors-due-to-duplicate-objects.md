---
title: 902 (Errori di sincronizzazione a causa di oggetti duplicati)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708066"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="c782c-102">Errori di sincronizzazione dovuti a oggetti duplicati</span><span class="sxs-lookup"><span data-stu-id="c782c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="c782c-103">Al termine della sincronizzazione della directory in Microsoft 365, potrebbe essere visualizzato uno dei seguenti messaggi di errore:</span><span class="sxs-lookup"><span data-stu-id="c782c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="c782c-104">Impossibile aggiornare questo oggetto in Microsoft Online Services perché gli attributi seguenti associati a questo oggetto hanno valori che potrebbero essere già associati a un altro oggetto nella directory locale.</span><span class="sxs-lookup"><span data-stu-id="c782c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="c782c-105">Un oggetto sincronizzato con lo stesso indirizzo proxy esiste già nella directory Microsoft Online Services locale.</span><span class="sxs-lookup"><span data-stu-id="c782c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="c782c-106">Impossibile aggiornare questo oggetto perché gli attributi seguenti associati a questo oggetto hanno valori che potrebbero essere già associati a un altro oggetto nei servizi directory locali: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c782c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="c782c-107">Per identificare e risolvere il problema, scaricare ed eseguire lo strumento di correzione degli errori [di DirSync idFix.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="c782c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="c782c-108">Per ulteriori informazioni, vedere [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="c782c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
