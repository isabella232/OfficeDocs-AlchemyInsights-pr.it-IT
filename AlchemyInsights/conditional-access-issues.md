---
title: Problemi di accesso condizionale
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013952"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="3a2c1-102">Problemi di accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="3a2c1-102">Conditional access issues</span></span>

<span data-ttu-id="3a2c1-103">**Risolvere i problemi con la diagnostica di accesso**</span><span class="sxs-lookup"><span data-stu-id="3a2c1-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="3a2c1-104">È possibile scoprire rapidamente cosa è successo o diagnosticare i problemi relativi all'accesso dell'utente utilizzando la [diagnostica di accesso](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="3a2c1-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="3a2c1-105">Avviare la Diagnostica di accesso.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="3a2c1-106">Individuare l'evento da analizzare immettendo i dettagli sull'utente, l'applicazione, l'ora di accesso, l'ID richiesta o l'ID di correlazione.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="3a2c1-107">Esaminare i risultati diagnostici in cui vengono illustrati i dettagli relativi a ciò che è accaduto e le azioni che è possibile eseguire per apportare modifiche (se sono necessarie modifiche).</span><span class="sxs-lookup"><span data-stu-id="3a2c1-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="3a2c1-108">**Passaggi per la risoluzione dei problemi di accesso**</span><span class="sxs-lookup"><span data-stu-id="3a2c1-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="3a2c1-109">Passare alla pagina di accesso di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="3a2c1-110">Filtrare gli accessi in base all'utente, l'intervallo di tempo, l'applicazione, lo stato, l'app client e così via.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="3a2c1-111">Selezionare un evento di accesso e visualizzare la scheda Access condizionale per vedere quali criteri sono stati valutati.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="3a2c1-112">Fare clic sulla riga di un criterio per visualizzare i dettagli del criterio e comprendere il motivo per cui è stata applicata.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="3a2c1-113">**Strumenti per la risoluzione di un criterio di accesso condizionale**</span><span class="sxs-lookup"><span data-stu-id="3a2c1-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="3a2c1-114">La modalità solo report consente di valutare un criterio senza influire sugli utenti.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="3a2c1-115">Lo strumento What-If consente di simulare gli eventi di accesso e di vedere quali criteri si applicano.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="3a2c1-116">La cartella di lavoro Insights and Reporting Visualizza l'impatto in tempo reale di ogni criterio.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="3a2c1-117">**Criteri di protezione di base**</span><span class="sxs-lookup"><span data-stu-id="3a2c1-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="3a2c1-118">I criteri di protezione di base sono stati deprecati.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="3a2c1-119">Non vengono più applicate e verranno presto rimossi dal portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="3a2c1-120">È consigliabile abilitare le [impostazioni predefinite](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="3a2c1-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="3a2c1-121">Per ulteriori informazioni sull'accesso condizionale, vedere:</span><span class="sxs-lookup"><span data-stu-id="3a2c1-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="3a2c1-122">[Procedure consigliate per l'accesso condizionale in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condizioni per l'accesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 condizionale [Controlli in accesso](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 condizionale [Posizioni in accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="3a2c1-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
