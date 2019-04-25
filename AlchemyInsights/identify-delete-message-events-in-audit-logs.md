---
title: Identificare gli eventi di eliminazione dei messaggi nei registri di controllo
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416714"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="9a8c2-102">Registri di controllo per i messaggi di posta elettronica eliminati</span><span class="sxs-lookup"><span data-stu-id="9a8c2-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="9a8c2-103">A partire da gennaio 2019, Microsoft sta attivando la registrazione di controllo delle cassette postali per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="9a8c2-104">In caso contrario, per esaminare eliminare gli eventi dei messaggi per un utente specifico, è necessario abilitare manualmente le azioni di eliminazione per il controllo.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="9a8c2-105">Se la registrazione di controllo delle cassette postali è già abilitata per l'organizzazione o per l'utente specifico, attenersi alla procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="9a8c2-106">Accedere al [centro conformità _AMP_ sicurezza di Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9a8c2-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9a8c2-107">Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9a8c2-108">Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .</span><span class="sxs-lookup"><span data-stu-id="9a8c2-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9a8c2-109">Specificare il nome utente per gli utenti che si desidera esaminare (l'utente che ha eliminato gli elementi).</span><span class="sxs-lookup"><span data-stu-id="9a8c2-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="9a8c2-110">Nel campo **attività** selezionare **messaggi eliminati dalla cartella Posta eliminata** e **spostare i messaggi nella cartella Posta eliminata**.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="9a8c2-111">Fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-111">Click **Search**.</span></span>

<span data-ttu-id="9a8c2-112">Nei risultati, selezionare un record di controllo.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-112">In the results, select an audit record.</span></span> <span data-ttu-id="9a8c2-113">Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9a8c2-114">Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento quando è stata eliminata, vengono visualizzate nel campo **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="9a8c2-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="9a8c2-115">La proprietà **ClientInfoString** verrà visualizzata se l'eliminazione si è verificata in Outlook, Outlook sul Web (in precedenza noto come Outlook Web App) o qualsiasi altro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="9a8c2-116">Per ulteriori informazioni, vedere [determinare chi ha configurato l'inoltro della posta elettronica per una cassetta postale](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="9a8c2-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="9a8c2-117">**Nota**: non è possibile recuperare gli elementi eliminati utilizzando la caratteristica log di controllo.</span><span class="sxs-lookup"><span data-stu-id="9a8c2-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="9a8c2-118">Per recuperare i messaggi eliminati in Outlook sul Web, vedere [recuperare gli elementi eliminati in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="9a8c2-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
