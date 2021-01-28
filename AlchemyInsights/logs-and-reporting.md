---
title: Registri e report
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031500"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="1f2a5-102">Registri e report</span><span class="sxs-lookup"><span data-stu-id="1f2a5-102">Logs and Reporting</span></span>

<span data-ttu-id="1f2a5-103">Informazioni frequenti su Azure [Active Directory Reporting](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) risposte alle domande frequenti sui report di Azure Active Directory (Azure ad).</span><span class="sxs-lookup"><span data-stu-id="1f2a5-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="1f2a5-104">Per ulteriori informazioni, vedere [report di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="1f2a5-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="1f2a5-105">**Risoluzione dei problemi relativi al controllo**</span><span class="sxs-lookup"><span data-stu-id="1f2a5-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="1f2a5-106">Se si verificano problemi durante la visualizzazione di alcune attività di controllo e l'attività mancante è presente nell' [elenco](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), è necessario presentare un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="1f2a5-107">Se si verificano problemi durante la visualizzazione di eventuali log di controllo nel tenant, è necessario presentare un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="1f2a5-108">Se le attività di controllo non vengono visualizzate immediatamente nel portale di Azure, consultare le [informazioni sulla latenza](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) e archiviare un ticket di supporto se il ritardo supera la latenza documentata.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="1f2a5-109">Conservazione dei registri delle attività di Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f2a5-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="1f2a5-110">Se non si Visualizza tutto il controllo per l'intervallo di date selezionato, è possibile scaricare fino a 250K righe (ordinate in base alla più recente) di accessi dal portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="1f2a5-111">Per ulteriori informazioni, vedere [download delle attività di controllo](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="1f2a5-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="1f2a5-112">**Risoluzione dei problemi relativi agli accessi**</span><span class="sxs-lookup"><span data-stu-id="1f2a5-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="1f2a5-113">Gli ultimi 30 giorni di dati possono essere visualizzati solo se si dispone di una licenza di Azure AD Premium (P1 o P2) per il tenant.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="1f2a5-114">Gli accessi sono disponibili solo per i tenant di Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="1f2a5-115">Non è disponibile per i tenant con licenza gratuita o di base.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="1f2a5-116">Se il tenant ha una licenza Premium P1 e non è possibile visualizzare gli accessi, consultare le [informazioni sulla latenza](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) e archiviare un ticket di supporto se il ritardo supera la latenza documentata.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="1f2a5-117">Se non vengono visualizzati tutti gli accessi per l'intervallo di date selezionato, tenere presente che è possibile scaricare fino a 250K righe (ordinate in base alla più recente) di accessi dal portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="1f2a5-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="1f2a5-118">Per ulteriori informazioni, vedere [download delle attività di accesso](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="1f2a5-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="1f2a5-119">**Risoluzione dei problemi relativi ai rapporti di sicurezza (utenti contrassegnati a rischio, accesso rischioso)**</span><span class="sxs-lookup"><span data-stu-id="1f2a5-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="1f2a5-120">Utenti contrassegnati per il rapporto sulla sicurezza dei rischi</span><span class="sxs-lookup"><span data-stu-id="1f2a5-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="1f2a5-121">Report di accesso rischioso nel portale di Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f2a5-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="1f2a5-122">Eventi di rischio di Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f2a5-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
