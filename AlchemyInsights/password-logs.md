---
title: Registri password
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523086"
---
# <a name="password-logs"></a><span data-ttu-id="5575c-102">Registri password</span><span class="sxs-lookup"><span data-stu-id="5575c-102">Password logs</span></span>

<span data-ttu-id="5575c-103">**Problemi di accesso ai registri di controllo per la reimpostazione password**</span><span class="sxs-lookup"><span data-stu-id="5575c-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="5575c-104">Per risolvere i problemi relativi all'accesso ai registri di controllo per la reimpostazione password, eseguire il passaggio seguente:</span><span class="sxs-lookup"><span data-stu-id="5575c-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="5575c-105">Assicurarsi di essere autorizzati a visualizzare i registri di controllo.</span><span class="sxs-lookup"><span data-stu-id="5575c-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="5575c-106">Sono autorizzati solo gli utenti con i seguenti ruoli:</span><span class="sxs-lookup"><span data-stu-id="5575c-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="5575c-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="5575c-107">Global administrator</span></span>
 - <span data-ttu-id="5575c-108">Amministratore della sicurezza</span><span class="sxs-lookup"><span data-stu-id="5575c-108">Security administrator</span></span>
 - <span data-ttu-id="5575c-109">Ruolo con autorizzazioni di lettura per la sicurezza</span><span class="sxs-lookup"><span data-stu-id="5575c-109">Security reader</span></span>

<span data-ttu-id="5575c-110">**Visualizzazione di tutti gli eventi di controllo di reimpostazione password a partire dalla distribuzione iniziale**</span><span class="sxs-lookup"><span data-stu-id="5575c-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="5575c-111">Nei report degli ultimi 30 giorni vengono archiviati fino a 120.000 eventi di reimpostazione/registrazione password.</span><span class="sxs-lookup"><span data-stu-id="5575c-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="5575c-112">Il limite massimo si applica all'interfaccia utente quando si scarica il file CSV.</span><span class="sxs-lookup"><span data-stu-id="5575c-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="5575c-113">Tramite PowerShell sono disponibili un milione di eventi.</span><span class="sxs-lookup"><span data-stu-id="5575c-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="5575c-114">Per ulteriori informazioni, vedere i seguenti collegamenti:</span><span class="sxs-lookup"><span data-stu-id="5575c-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="5575c-115">Eventi di reimpostazione della password self-service dall'API Report ed eventi di Azure AD</span><span class="sxs-lookup"><span data-stu-id="5575c-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5575c-116">Come scaricare rapidamente gli eventi di registrazione per la reimpostazione della password con PowerShell</span><span class="sxs-lookup"><span data-stu-id="5575c-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="5575c-117">**Altre informazioni sulle funzionalità di creazione di report per la reimpostazione password**</span><span class="sxs-lookup"><span data-stu-id="5575c-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="5575c-118">Controllare chi registra o reimposta le password con i registri di controllo di reimpostazione password di Azure AD nel portale di Azure in **Utenti e gruppi**.</span><span class="sxs-lookup"><span data-stu-id="5575c-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="5575c-119">Per ulteriori informazioni, vedere i seguenti collegamenti:</span><span class="sxs-lookup"><span data-stu-id="5575c-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="5575c-120">Panoramica dei report di reimpostazione della password</span><span class="sxs-lookup"><span data-stu-id="5575c-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5575c-121">Come visualizzare i report di reimpostazione della password nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="5575c-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5575c-122">Eventi di reimpostazione della password self-service dall'API Report ed eventi di Azure AD</span><span class="sxs-lookup"><span data-stu-id="5575c-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="5575c-123">Come scaricare rapidamente gli eventi di registrazione per la reimpostazione della password con PowerShell</span><span class="sxs-lookup"><span data-stu-id="5575c-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


