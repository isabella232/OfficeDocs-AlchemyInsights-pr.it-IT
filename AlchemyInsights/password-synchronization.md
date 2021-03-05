---
title: Sincronizzazione delle password
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449141"
---
# <a name="password-synchronization"></a><span data-ttu-id="d336c-102">Sincronizzazione delle password</span><span class="sxs-lookup"><span data-stu-id="d336c-102">Password synchronization</span></span>

<span data-ttu-id="d336c-103">**La sincronizzazione dell'hash delle password non funziona affatto**</span><span class="sxs-lookup"><span data-stu-id="d336c-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="d336c-104">Alcuni problemi comuni riscontrati dai clienti quando la sincronizzazione hash delle password non funziona sono:</span><span class="sxs-lookup"><span data-stu-id="d336c-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="d336c-105">All'account di Active Directory usato da Azure AD Connect per  comunicare con Active Directory locale non vengono concesse le autorizzazioni Replica modifiche directory e Replica modifiche **directory tutte,** necessarie per la sincronizzazione delle password. È necessario risolvere il problema concedendo queste autorizzazioni all'account di Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d336c-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="d336c-106">La sincronizzazione dell'hash delle password viene disabilitata dopo che un amministratore ha modificato il metodo user Sign-In da **Sincronizzazione** password a un'altra opzione, ad esempio Federazione con **AD FS** nella procedura guidata di Azure AD Connect. È possibile risolvere il problema ri abilitando la funzionalità di sincronizzazione **dell'hash** delle password nella procedura guidata di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d336c-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="d336c-107">Problema di connettività con Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="d336c-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="d336c-108">Ad esempio, alcuni controller di dominio non sono [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) accessibili da Azure AD Connect o le porte richieste sono bloccate da Firewall. È necessario risolvere il problema assicurando che la connettività tra il server Azure AD Connect e Active Directory locale funzioni correttamente.</span><span class="sxs-lookup"><span data-stu-id="d336c-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="d336c-109">Il server Azure AD Connect è attualmente in modalità di gestione temporanea, il che fa in modo che il server non sia in grado di eseguire gli hash delle password. Per risolvere il problema, seguire la procedura descritta nella sezione Risolvere i problemi di sincronizzazione delle password con la sincronizzazione di [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nessuna password sincronizzata.</span><span class="sxs-lookup"><span data-stu-id="d336c-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="d336c-110">**La sincronizzazione dell'hash delle password non funziona per alcuni utenti**</span><span class="sxs-lookup"><span data-stu-id="d336c-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="d336c-111">Se hai notato che l'hash delle password  non è sincronizzato per un utente, usa l'attività di risoluzione dei problemi in Azure AD Connect per analizzare e risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="d336c-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="d336c-112">Eseguire le attività seguenti:</span><span class="sxs-lookup"><span data-stu-id="d336c-112">Perform the following tasks:</span></span>

    <span data-ttu-id="d336c-113">a.</span><span class="sxs-lookup"><span data-stu-id="d336c-113">a.</span></span> [<span data-ttu-id="d336c-114">Eseguire l'attività di risoluzione dei problemi nella procedura guidata</span><span class="sxs-lookup"><span data-stu-id="d336c-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="d336c-115">b.</span><span class="sxs-lookup"><span data-stu-id="d336c-115">b.</span></span> [<span data-ttu-id="d336c-116">Utilizzare il cmdlet per la risoluzione dei problemi per analizzare il problema di sincronizzazione dell'hash delle password per un utilizzo specifico</span><span class="sxs-lookup"><span data-stu-id="d336c-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="d336c-117">L'oggetto utente di Active Directory locale è abilitato per l'opzione Cambiamento password **all'accesso** successivo.</span><span class="sxs-lookup"><span data-stu-id="d336c-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="d336c-118">Quando questa opzione è abilitata, all'utente viene assegnata una password temporanea e verrà richiesto di modificarla al successivo accesso.</span><span class="sxs-lookup"><span data-stu-id="d336c-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="d336c-119">Azure AD Connect non sincronizza le password temporanee con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d336c-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="d336c-120">Per risolvere il problema precedente, eseguire una delle attività seguenti:</span><span class="sxs-lookup"><span data-stu-id="d336c-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="d336c-121">Chiedere all'utente di accedere all'applicazione locale (ad esempio, Windows Desktop) e modificare la password.</span><span class="sxs-lookup"><span data-stu-id="d336c-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="d336c-122">La nuova password verrà sincronizzata con Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d336c-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="d336c-123">Richiedere a un amministratore di aggiornare la password dell'utente senza abilitare l'opzione Modifica **password** all'accesso successivo e condivisione della nuova password con l'utente.</span><span class="sxs-lookup"><span data-stu-id="d336c-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="d336c-124">L'oggetto utente di Active Directory locale non è configurato **correttamente** per la sincronizzazione degli oggetti o la sincronizzazione delle password.</span><span class="sxs-lookup"><span data-stu-id="d336c-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="d336c-125">Per risolvere questo problema, seguire i passaggi descritti in Risoluzione dei problemi di sincronizzazione hash delle password con la sincronizzazione [di Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="d336c-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







