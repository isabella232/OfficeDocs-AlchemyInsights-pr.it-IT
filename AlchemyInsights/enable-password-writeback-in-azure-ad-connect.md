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
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709731"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="743e4-102">Abilitare il writeback delle password in Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="743e4-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="743e4-103">Per abilitare il writeback della reimpostazione della password in modalità self-service, abilitare prima l'opzione writeback in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="743e4-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="743e4-104">Nel server Azure AD Connect eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="743e4-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="743e4-105">Accedere al server Azure AD Connect e avviare la configurazione guidata di **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="743e4-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="743e4-106">Nella pagina di **benvenuto** fare clic su **Configura**.</span><span class="sxs-lookup"><span data-stu-id="743e4-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="743e4-107">Nella pagina **Attività aggiuntive** selezionare **Personalizza le opzioni di sincronizzazione**, quindi fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="743e4-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="743e4-108">Nella pagina **Connessione ad Azure AD**, immettere le credenziali dell'amministratore globale per il tenant Azure e fare clic su Avanti.</span><span class="sxs-lookup"><span data-stu-id="743e4-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="743e4-109">Nelle pagine **Connessione delle directory** e **Filtro di domini/unità organizzative**, fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="743e4-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="743e4-110">Nella pagina **Funzionalità facoltative** selezionare la casella accanto a **Writeback password** e fare clic su **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="743e4-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="743e4-111">Nella pagina **Pronto per la configurazione**, fare clic su **Configura** e attendere il completamento del processo.</span><span class="sxs-lookup"><span data-stu-id="743e4-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="743e4-112">Quando viene visualizzata la fine della configurazione, fare clic su **Esci**.</span><span class="sxs-lookup"><span data-stu-id="743e4-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="743e4-113">Dopo l’abilitazione dell’opzione writeback delle password in Azure AD Connect, ora è possibile configurare Azure AD SSPR per il writeback.</span><span class="sxs-lookup"><span data-stu-id="743e4-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="743e4-114">Per abilitare il writeback delle password in reimpostazione della password self-service, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="743e4-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="743e4-115">Accedere al portale di Azure con un account di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="743e4-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="743e4-116">Cercare e selezionare **Azure Active Directory**, fare clic su **Reimpostazione della password** e quindi scegliere **Integrazione locale**.</span><span class="sxs-lookup"><span data-stu-id="743e4-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="743e4-117">Impostare l’opzione per **Vuoi eseguire il writeback delle password nella directory locale?** su **Sì**.</span><span class="sxs-lookup"><span data-stu-id="743e4-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="743e4-118">Impostare l’opzione per **Vuoi consentire agli utenti di sbloccare gli account senza reimpostare la password?** su \*\* Sì\*\*.</span><span class="sxs-lookup"><span data-stu-id="743e4-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="743e4-119">Al termine fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="743e4-119">When ready, click **Save**.</span></span>

<span data-ttu-id="743e4-120">Per altre informazioni, vedere [Abilitare il writeback della reimpostazione della password in modalità self-service di Azure Active Directory in un ambiente locale](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="743e4-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
