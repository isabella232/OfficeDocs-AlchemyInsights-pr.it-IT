---
title: Aggiunta di utenti esterni a un gruppo di distribuzione
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737877"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="114ce-102">Aggiungere utenti esterni a un gruppo di distribuzione</span><span class="sxs-lookup"><span data-stu-id="114ce-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="114ce-103">L'aggiunta di un contatto esterno a un gruppo di distribuzione (DG) è un processo in due fasi:</span><span class="sxs-lookup"><span data-stu-id="114ce-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="114ce-104">Creare un contatto di posta per l'utente esterno:</span><span class="sxs-lookup"><span data-stu-id="114ce-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="114ce-105">Nell'interfaccia di amministrazione, andare alla pagina \*\*\*\* > [contatti](https://admin.microsoft.com/adminportal/home#/Contact) utenti.</span><span class="sxs-lookup"><span data-stu-id="114ce-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="114ce-106">Selezionare **Aggiungi un contatto**.</span><span class="sxs-lookup"><span data-stu-id="114ce-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="114ce-107">Digitare le informazioni per il contatto e selezionare **Aggiungi**.</span><span class="sxs-lookup"><span data-stu-id="114ce-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="114ce-108">Aggiungere il contatto di posta elettronica alla DG:</span><span class="sxs-lookup"><span data-stu-id="114ce-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="114ce-109">Nell'interfaccia di amministrazione, andare alla[](https://admin.microsoft.com/adminportal/home#/groups)  > pagina **gruppi.**</span><span class="sxs-lookup"><span data-stu-id="114ce-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="114ce-110">Individuare la DG alla quale si desidera aggiungere l'utente esterno e selezionarla per aprire la finestra di dialogo Modifica.</span><span class="sxs-lookup"><span data-stu-id="114ce-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="114ce-111">Nella scheda **membri** selezionare **Visualizza tutti i membri e Gestisci**.</span><span class="sxs-lookup"><span data-stu-id="114ce-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="114ce-112">Selezionare **Aggiungi membri**.</span><span class="sxs-lookup"><span data-stu-id="114ce-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="114ce-113">Selezionare il contatto di posta creato nel passaggio precedente e quindi fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="114ce-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="114ce-114">Se dopo aver seguito questi passaggi gli utenti esterni non possono inviare messaggi di posta elettronica alla DG o non ricevono messaggi di posta elettronica, potrebbe essere che la DG sia contrassegnata solo per consentire l'invio di messaggi di posta elettronica da parte di utenti interni.</span><span class="sxs-lookup"><span data-stu-id="114ce-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="114ce-115">È possibile controllare questa configurazione e correggerla seguendo le istruzioni riportate [di seguito.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="114ce-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="114ce-116">**Nota:** Queste istruzioni non si applicano se il tipo del gruppo è "Office 365 Group" invece di "gruppo di distribuzione".</span><span class="sxs-lookup"><span data-stu-id="114ce-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="114ce-117">In caso contrario, è possibile aggiungere l'utente esterno direttamente al gruppo da Outlook.</span><span class="sxs-lookup"><span data-stu-id="114ce-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="114ce-118">Informazioni dettagliate sui gruppi di Office 365 i clienti e le istruzioni per l'aggiunta di ospiti esterni sono disponibili in [questo articolo](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="114ce-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  