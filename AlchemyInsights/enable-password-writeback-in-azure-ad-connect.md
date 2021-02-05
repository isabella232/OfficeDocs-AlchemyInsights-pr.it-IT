---
title: Abilitare il writeback delle password in Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093359"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="256d3-102">Abilitare il writeback delle password in Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="256d3-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="256d3-103">Per abilitare il writeback della reimpostazione della password in modalità self-service, abilitare prima l'opzione writeback in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="256d3-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="256d3-104">Nel server Azure AD Connect eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="256d3-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="256d3-105">Accedere al server Azure AD Connect e avviare la configurazione guidata di **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="256d3-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="256d3-106">Nella pagina di **benvenuto** fare clic su **Configura**.</span><span class="sxs-lookup"><span data-stu-id="256d3-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="256d3-107">Nella pagina **Attività aggiuntive** selezionare **Personalizza le opzioni di sincronizzazione**, quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="256d3-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="256d3-108">Nella pagina **Connessione ad Azure AD**, immettere le credenziali di amministratore globale per il tenant Azure e fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="256d3-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="256d3-109">Nelle pagine **Connessione delle directory** e **Filtro domini/OU**, fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="256d3-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="256d3-110">Nella pagina **Funzionalità facoltative** selezionare la casella accanto a **Writeback password** e fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="256d3-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="256d3-111">Nella pagina **Pronto per la configurazione**, fare clic su **Configura** e attendere il completamento del processo.</span><span class="sxs-lookup"><span data-stu-id="256d3-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="256d3-112">Quando viene visualizzata la fine della configurazione, fare clic su **Esci**.</span><span class="sxs-lookup"><span data-stu-id="256d3-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="256d3-113">Dopo l’abilitazione dell’opzione writeback delle password in Azure AD Connect, è possibile configurare Azure AD SSPR per il writeback.</span><span class="sxs-lookup"><span data-stu-id="256d3-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="256d3-114">Per abilitare il writeback delle password in reimpostazione della password self-service, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="256d3-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="256d3-115">Accedere al portale di Azure con un account di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="256d3-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="256d3-116">Cercare e selezionare **Azure Active Directory**, fare clic su **Reimpostazione della password** poi fare clic su **Integrazione locale**.</span><span class="sxs-lookup"><span data-stu-id="256d3-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="256d3-117">Impostare l’opzione **Vuoi eseguire il writeback delle password nella directory locale?** su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="256d3-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="256d3-118">Impostare l’opzione per **Vuoi consentire agli utenti di sbloccare gli account senza reimpostare la password?** su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="256d3-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="256d3-119">Al termine fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="256d3-119">When ready, click **Save**.</span></span>

<span data-ttu-id="256d3-120">Per altre informazioni, vedere [Abilitare il writeback della reimpostazione della password in modalità self-service di Azure Active Directory in ambiente locale](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="256d3-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="256d3-121">Quando un amministratore ripristina la password di un utente nel portale di Azure, se l'utente è federato o l’hash delle password è sincronizzato, la password viene scritta di nuovo in locale.</span><span class="sxs-lookup"><span data-stu-id="256d3-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="256d3-122">Questa funzionalità richiede Azure Premium License (P1 or P2) e attualmente non è supportata nel portale Amministrazione di Office.</span><span class="sxs-lookup"><span data-stu-id="256d3-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
