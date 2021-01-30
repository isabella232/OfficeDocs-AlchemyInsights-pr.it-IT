---
title: Problemi con le credenziali
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052949"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="d4574-102">Problemi con le credenziali</span><span class="sxs-lookup"><span data-stu-id="d4574-102">Issues with credentials</span></span>

<span data-ttu-id="d4574-103">Microsoft Identity Platform e il flusso delle credenziali [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrivono come programmare direttamente in base al flusso di concessione delle credenziali client OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="d4574-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="d4574-104">**Come si gestiscono le credenziali della password o del certificato di un'applicazione?**</span><span class="sxs-lookup"><span data-stu-id="d4574-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="d4574-105">Nell'interfaccia cli di Azure puoi usare le credenziali [dell'app](https://docs.microsoft.com/cli/azure/ad/app/credential) pubblicitaria az per eliminare, elencare o reimpostare la password o le credenziali del certificato di un'applicazione.</span><span class="sxs-lookup"><span data-stu-id="d4574-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="d4574-106">**In che modo gli utenti reimpostano le password?**</span><span class="sxs-lookup"><span data-stu-id="d4574-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="d4574-107">Gli utenti devono [registrarsi per la reimpostazione della password self-service](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) prima di poter reimpostare le password.</span><span class="sxs-lookup"><span data-stu-id="d4574-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="d4574-108">Dopo la registrazione, un utente può seguire le istruzioni riportate in questo articolo per reimpostare la password: Reimpostare la password dell'istituto di [istruzione o dell'istituto di istruzione.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="d4574-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="d4574-109">**In che modo gli utenti cambiano le password?**</span><span class="sxs-lookup"><span data-stu-id="d4574-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="d4574-110">Gli utenti possono seguire i passaggi descritti in questo articolo per cambiare le password: [Come modificare la password.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="d4574-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="d4574-111">Possono anche gestire [le password delle app per la verifica in due passaggi.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="d4574-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="d4574-112">**L'utente riceve un errore durante la modifica o la reimpostazione della password**</span><span class="sxs-lookup"><span data-stu-id="d4574-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="d4574-113">Questo collegamento fornirà informazioni sui problemi comuni che possono verificarsi quando un utente tenta di reimpostare la password: [problemi comuni e relative soluzioni](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="d4574-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="d4574-114">**Si è verificato un problema durante la reimpostazione della password di un utente**</span><span class="sxs-lookup"><span data-stu-id="d4574-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="d4574-115">Assicurarsi di essere autorizzati a reimpostare le password.</span><span class="sxs-lookup"><span data-stu-id="d4574-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="d4574-116">*Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.*</span><span class="sxs-lookup"><span data-stu-id="d4574-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d4574-117">Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.</span><span class="sxs-lookup"><span data-stu-id="d4574-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="d4574-118">Assicurarsi di comprendere i requisiti di licenza:</span><span class="sxs-lookup"><span data-stu-id="d4574-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="d4574-119">È necessario disporre di almeno una licenza assegnata nell'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="d4574-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="d4574-120">**Utenti solo cloud** - Qualsiasi SKU a pagamento di Office 365 (O365) o Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="d4574-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="d4574-121">**Utenti cloud e/o** locali : Azure AD Premium P1 o P2, Enterprise Mobility + Security (EMS) o Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="d4574-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="d4574-122">Per altre informazioni sui requisiti di licenza, vedere [Requisiti di licenza per la reimpostazione della password in modalità self-service di Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="d4574-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="d4574-123">Per reimpostare la password di un utente, trova l'utente in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d4574-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="d4574-124">Quindi, nel pannello di panoramica per l'utente, fare clic sul pulsante "reimposta password".</span><span class="sxs-lookup"><span data-stu-id="d4574-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="d4574-125">**Il pulsante di reimpostazione della password è in grigio**</span><span class="sxs-lookup"><span data-stu-id="d4574-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="d4574-126">Non si è autorizzati a reimpostare **le password** di questo utente.</span><span class="sxs-lookup"><span data-stu-id="d4574-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="d4574-127">*Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.*</span><span class="sxs-lookup"><span data-stu-id="d4574-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d4574-128">Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.</span><span class="sxs-lookup"><span data-stu-id="d4574-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d4574-129">**Il pannello di reimpostazione della password non è visualizzato**</span><span class="sxs-lookup"><span data-stu-id="d4574-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="d4574-130">Non si è autorizzati a reimpostare le password.</span><span class="sxs-lookup"><span data-stu-id="d4574-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="d4574-131">*Solo gli amministratori globali, delle password e degli utenti possono reimpostare le password degli utenti.*</span><span class="sxs-lookup"><span data-stu-id="d4574-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="d4574-132">Gli amministratori globali possono anche reimpostare le password di altri amministratori con privilegi.</span><span class="sxs-lookup"><span data-stu-id="d4574-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="d4574-133">**Il pannello di integrazione locale non viene visualizzato nella reimpostazione della password**</span><span class="sxs-lookup"><span data-stu-id="d4574-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="d4574-134">Il pannello di integrazione locale viene visualizzato solo negli ambienti ibridi, ovvero si utilizza il writeback delle password per modificare le password degli utenti locali.</span><span class="sxs-lookup"><span data-stu-id="d4574-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="d4574-135">Questo pannello non viene visualizzato se:</span><span class="sxs-lookup"><span data-stu-id="d4574-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="d4574-136">Non si utilizza il writeback delle password</span><span class="sxs-lookup"><span data-stu-id="d4574-136">You are not using password writeback</span></span>
  - <span data-ttu-id="d4574-137">Si è verificato un problema con l'installazione/connettività del writeback delle password</span><span class="sxs-lookup"><span data-stu-id="d4574-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="d4574-138">Si è verificato un problema con l'installazione/connettività di Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d4574-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="d4574-139">Per ulteriori procedure di risoluzione dei problemi relativi al writeback delle password, vedere [Risolvere i problemi relativi al writeback delle password](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="d4574-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="d4574-140">**Non so come reimpostare la password di un utente**</span><span class="sxs-lookup"><span data-stu-id="d4574-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="d4574-141">Accedere al portale di Azure come amministratore appropriato.</span><span class="sxs-lookup"><span data-stu-id="d4574-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="d4574-142">Passare al pannello **Utenti e gruppi,** selezionare **Tutti gli utenti.**</span><span class="sxs-lookup"><span data-stu-id="d4574-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="d4574-143">Selezionare un utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d4574-143">Select a user from the list.</span></span>
4. <span data-ttu-id="d4574-144">Per l'utente selezionato, selezionare **Panoramica** e quindi nella barra dei comandi selezionare **Reimposta password.**</span><span class="sxs-lookup"><span data-stu-id="d4574-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="d4574-145">Seleziona il **pulsante Reimposta password** e segui le istruzioni visualizzate sullo schermo.</span><span class="sxs-lookup"><span data-stu-id="d4574-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="d4574-146">Solo le reimpostazioni eseguite tramite il **portale di Azure supportano** il writeback delle password.</span><span class="sxs-lookup"><span data-stu-id="d4574-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="d4574-147">**Reimpostazione della password di un utente locale dal portale di amministrazione di Office 365 o dall'applicazione per dispositivi mobili di Office 365, ma l'utente non è ancora in grado di accedere**</span><span class="sxs-lookup"><span data-stu-id="d4574-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="d4574-148">Il writeback delle password non è supportato in questo portale.</span><span class="sxs-lookup"><span data-stu-id="d4574-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="d4574-149">Reimpostare di nuovo la password dell'utente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="d4574-149">Reset the user's password again in the Azure portal.</span></span>
