---
title: Consentire o disabilitare un video IP in Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826347"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="de81b-102">Consentire o disabilitare un video IP in Teams</span><span class="sxs-lookup"><span data-stu-id="de81b-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="de81b-103">**Cambiare o creare un criterio di riunione**</span><span class="sxs-lookup"><span data-stu-id="de81b-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="de81b-104">Per modificare o creare un criterio riunione, passare **all'interfaccia di amministrazione di Microsoft Teams > Riunioni > Criteri di riunione**.</span><span class="sxs-lookup"><span data-stu-id="de81b-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="de81b-105">Selezionare un criterio dall'elenco o fare clic su **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="de81b-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="de81b-106">Se si sta creando un nuovo criterio, aggiungere un nome e una descrizione.</span><span class="sxs-lookup"><span data-stu-id="de81b-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="de81b-107">Il nome non può contenere caratteri speciali o più di 64 caratteri.</span><span class="sxs-lookup"><span data-stu-id="de81b-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="de81b-108">Scegliere le impostazioni desiderate e poi fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="de81b-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="de81b-109">Ad esempio, si supponga di avere molti utenti e di voler limitare la larghezza di banda necessaria per la riunione.</span><span class="sxs-lookup"><span data-stu-id="de81b-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="de81b-110">È possibile creare un nuovo criterio personalizzato denominato "Larghezza di banda limitata" e disabilitare le impostazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="de81b-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="de81b-111">In **Audio e video**:</span><span class="sxs-lookup"><span data-stu-id="de81b-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="de81b-112">Disattivare Consenti registrazione cloud.</span><span class="sxs-lookup"><span data-stu-id="de81b-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="de81b-113">Disattivare Consenti video IP.</span><span class="sxs-lookup"><span data-stu-id="de81b-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="de81b-114">Assegnare poi il criterio agli utenti.</span><span class="sxs-lookup"><span data-stu-id="de81b-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="de81b-115">**Assegnare un criterio riunione agli utenti**</span><span class="sxs-lookup"><span data-stu-id="de81b-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="de81b-116">Nel riquadro di spostamento sinistro dell'interfaccia di amministrazione di Microsoft Teams passare a **Utenti** e quindi fare clic sull'utente.</span><span class="sxs-lookup"><span data-stu-id="de81b-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="de81b-117">Per selezionare l'utente facendo clic a sinistra del nome utente e poi fare clic su **Impostazioni di modifica**.</span><span class="sxs-lookup"><span data-stu-id="de81b-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="de81b-118">In **Criteri riunioni** selezionare il criterio da assegnare e poi fare clic su **Applica**.</span><span class="sxs-lookup"><span data-stu-id="de81b-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="de81b-119">Per altre informazioni, vedere [Gestire i criteri di riunione in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="de81b-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
