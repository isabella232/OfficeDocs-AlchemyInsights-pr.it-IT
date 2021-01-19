---
title: Problemi nell'aggiunta di macchine virtuali
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884585"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="630be-102">Problemi nell'aggiunta di macchine virtuali</span><span class="sxs-lookup"><span data-stu-id="630be-102">Issue joining VMs</span></span>

<span data-ttu-id="630be-103">Per risolvere eventuali problemi che si verificano quando si cerca di aggiungere delle macchine virtuali, seguire questi passaggi:</span><span class="sxs-lookup"><span data-stu-id="630be-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="630be-104">Provare ad accedere usando il formato **UPN** (ad esempio, 'joeuser@contoso.com') al posto del formato **SAMAccountName** ('CONTOSO\joeuser').</span><span class="sxs-lookup"><span data-stu-id="630be-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="630be-105">Verificare di aver abilitato la sincronizzazione tramite password in conformità ai passaggi indicati nella *Guida introduttiva*.</span><span class="sxs-lookup"><span data-stu-id="630be-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="630be-106">Verificare che l'account utente interessato non sia un account esterno nel tenant Azure AD.</span><span class="sxs-lookup"><span data-stu-id="630be-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="630be-107">Gli utenti esterni non possono accedere al dominio gestito dato che Azure AD Domain Services non dispone delle credenziali di tali account utente.</span><span class="sxs-lookup"><span data-stu-id="630be-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="630be-108">Se l'account utente interessato è un account utente solo cloud, verificare che gli utenti abbiano modificato la loro password dopo aver abilitato Azure Active Directory Domain Services.</span><span class="sxs-lookup"><span data-stu-id="630be-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="630be-109">Questo passaggio porta alla generazione degli hash delle credenziali per Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="630be-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="630be-110">Se gli account utente interessati vengono sincronizzati da una directory locale, verificare che sia stata configurata la release consigliata di Azure AD Connect per eseguire una sincronizzazione completa.</span><span class="sxs-lookup"><span data-stu-id="630be-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="630be-111">Se, dopo aver eseguito il Passaggio 4, i problemi dovessero persistere, eseguire i seguenti comandi dal computer di sincronizzazione:</span><span class="sxs-lookup"><span data-stu-id="630be-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="630be-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="630be-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>