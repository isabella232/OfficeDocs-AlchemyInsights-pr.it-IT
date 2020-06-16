---
title: Un proprietario non può creare una sottocartella tramite Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716600"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="f62b7-102">Un proprietario non può creare una sottocartella tramite Outlook</span><span class="sxs-lookup"><span data-stu-id="f62b7-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="f62b7-103">**È presente un problema ancora aperto con i proprietari delle cartelle pubbliche che creano sottocartelle usando Outlook. Il problema verrà risolto a breve.**</span><span class="sxs-lookup"><span data-stu-id="f62b7-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="f62b7-104">Nel frattempo, usare una delle soluzioni alternative seguenti:</span><span class="sxs-lookup"><span data-stu-id="f62b7-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="f62b7-105">Usare Outlook per MAC per creare la sottocartella poiché il problema riguarda solo Outlook desktop per Windows (tutte le versioni)</span><span class="sxs-lookup"><span data-stu-id="f62b7-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="f62b7-106">Chiedere a un amministratore di creare la sottocartella tramite Shell di Exchange Online o l'interfaccia di amministrazione di Exchange</span><span class="sxs-lookup"><span data-stu-id="f62b7-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="f62b7-107">Cambiare la DefaultPublicFolderMailbox/EffectivePublicFolderMailbox dell'utente in una cassetta postale diversa da quella del contenuto che causa il problema.</span><span class="sxs-lookup"><span data-stu-id="f62b7-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="f62b7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="f62b7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="f62b7-109">Attendere un'ora e riavviare il client di Outlook</span><span class="sxs-lookup"><span data-stu-id="f62b7-109">Wait for an hour, restart outlook client</span></span>