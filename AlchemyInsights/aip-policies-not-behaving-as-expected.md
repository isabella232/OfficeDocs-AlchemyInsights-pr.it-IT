---
title: 'AIP: I criteri non funzionano come previsto'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663193"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="a6a60-102">AIP: I criteri non funzionano come previsto</span><span class="sxs-lookup"><span data-stu-id="a6a60-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="a6a60-103">Azure Information Protection: i criteri non funzionano come previsto; vedere le linee guida consigliate seguenti per vari problemi relativi ai criteri:</span><span class="sxs-lookup"><span data-stu-id="a6a60-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="a6a60-104">Se si verificano problemi con i contrassegni visivi, consultare l'articolo che descrive [quando vengono applicati i contrassegni visivi](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="a6a60-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="a6a60-105">Se si verificano problemi con l'etichettatura automatica, consultare [Come configurare le condizioni per la classificazione automatica e consigliata per Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [Cosa individuano le tipologie di informazioni sensibili](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="a6a60-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="a6a60-106">Se si verificano problemi con la protezione di file nativi/Pfile, consultare [Configurazione API file](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="a6a60-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="a6a60-107">Verificare se sono utilizzati criteri con ambito non configurati correttamente: [Come configurare i criteri di Azure Information Protection per utenti specifici tramite criteri con ambito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="a6a60-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="a6a60-108">Se l'etichettatura automatica non funziona per Outlook quando si allega un documento con etichetta, verificare che DRMEncryptProperty non sia definito come descritto qui: [Impostazioni IRM del Registro di sistema per la sicurezza](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="a6a60-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="a6a60-109">Se i problemi persistono, è possibile raccogliere i log del client di Azure Information Protection e allegare i log esportati al ticket.</span><span class="sxs-lookup"><span data-stu-id="a6a60-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="a6a60-110">Aprire un documento di Office o creare un nuovo messaggio di posta elettronica in Outlook.</span><span class="sxs-lookup"><span data-stu-id="a6a60-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="a6a60-111">Fare clic su **Protezione/Riservatezza** > **Guida e feedback**.</span><span class="sxs-lookup"><span data-stu-id="a6a60-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="a6a60-112">Fare clic su **Esporta log**.</span><span class="sxs-lookup"><span data-stu-id="a6a60-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="a6a60-113">Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="a6a60-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="a6a60-114">Risorse aggiuntive:</span><span class="sxs-lookup"><span data-stu-id="a6a60-114">Additional resources:</span></span>

- [<span data-ttu-id="a6a60-115">Come configurare un'etichetta per contrassegni visivi di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6a60-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="a6a60-116">Consultare la documentazione di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6a60-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a6a60-117">Usare le etichette di riservatezza nelle app di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a6a60-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

