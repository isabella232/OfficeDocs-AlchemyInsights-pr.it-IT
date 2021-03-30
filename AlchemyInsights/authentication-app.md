---
title: App di autenticazione
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403836"
---
# <a name="authentication-app"></a><span data-ttu-id="9cee5-102">App di autenticazione</span><span class="sxs-lookup"><span data-stu-id="9cee5-102">Authentication app</span></span>

<span data-ttu-id="9cee5-103">Se sei un amministratore globale, puoi scoprire rapidamente cosa è successo o diagnosticare i problemi relativi all'accesso utente usando [Diagnostica accesso.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="9cee5-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="9cee5-104">Avviare la diagnostica facendo clic[sul pulsante](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" Avvia diagnostica ".</span><span class="sxs-lookup"><span data-stu-id="9cee5-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="9cee5-105">Trova l'evento da analizzare immettendo i dettagli relativi all'utente, all'applicazione, all'ora di accesso, all'ID richiesta o all'ID correlazione.</span><span class="sxs-lookup"><span data-stu-id="9cee5-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="9cee5-106">Rivedere i risultati di diagnostica che mostrano i dettagli di quanto accaduto e delle misure da adottare per effettuare eventuali modifiche, se necessario.</span><span class="sxs-lookup"><span data-stu-id="9cee5-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="9cee5-107">**Verificare lo scenario applicabile:**</span><span class="sxs-lookup"><span data-stu-id="9cee5-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="9cee5-108">Se un utente non riceve una notifica push nell'app Microsoft Authenticator, verifica che non siano visualizzati sotto gli utenti bloccati dell'autenticazione a più fattori, come descritto in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="9cee5-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="9cee5-109">Se l'utente non è bloccato per L'autenticazione a più fattori ma non riceve una notifica push, può aprire l'app Microsoft Authenticator, che estrarrà le richieste di approvazione in sospeso.</span><span class="sxs-lookup"><span data-stu-id="9cee5-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="9cee5-110">Come metodo di accesso alternativo, l'utente può anche fare clic su Accedi in un altro modo e scegliere di usare un codice di verifica dalla mia app per dispositivi mobili.</span><span class="sxs-lookup"><span data-stu-id="9cee5-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="9cee5-111">L'app Microsoft Authenticator è l'unico metodo disponibile per molti utenti.</span><span class="sxs-lookup"><span data-stu-id="9cee5-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="9cee5-112">[Per altre informazioni sulle impostazioni predefinite di sicurezza,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)consulta Domande frequenti [sull'app Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) per domande frequenti e su come risolverle.</span><span class="sxs-lookup"><span data-stu-id="9cee5-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="9cee5-113">**Video consigliati**</span><span class="sxs-lookup"><span data-stu-id="9cee5-113">**Recommended Videos**</span></span>

<span data-ttu-id="9cee5-114">[Come configurare l'app Authenticator in un nuovo telefono (2 minuti).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="9cee5-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
