---
title: Abilitare l'autenticazione SMTP e la risoluzione dei problemi
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077655"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="8f02c-102">Abilitare l'autenticazione SMTP e la risoluzione dei problemi</span><span class="sxs-lookup"><span data-stu-id="8f02c-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="8f02c-103">Se si vuole abilitare l'autenticazione SMTP per una cassetta postale o si riceve un errore "Client non autenticato", "Autenticazione non riuscita" o "SmtpClientAuthentication" con codice 5.7.57 o 5.7.3 o 5.7.139 quando si prova a inoltrare la posta elettronica autenticando un dispositivo o un'applicazione con Microsoft 365, eseguire queste tre azioni per risolvere il problema:</span><span class="sxs-lookup"><span data-stu-id="8f02c-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="8f02c-104">Disabilitare le [impostazioni predefinite per la sicurezza di Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) impostando **Abilita le impostazioni predefinite per la sicurezza** su **No**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="8f02c-105">a.</span><span class="sxs-lookup"><span data-stu-id="8f02c-105">a.</span></span> <span data-ttu-id="8f02c-106">Accedere al portale di Azure come Amministratore della sicurezza, Amministratore di accesso condizionale o Amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="8f02c-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="8f02c-107">b.</span><span class="sxs-lookup"><span data-stu-id="8f02c-107">b.</span></span> <span data-ttu-id="8f02c-108">Passare ad Azure Active Directory> **Proprietà**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="8f02c-109">c.</span><span class="sxs-lookup"><span data-stu-id="8f02c-109">c.</span></span> <span data-ttu-id="8f02c-110">Selezionare **Gestire le impostazioni predefinite per la sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="8f02c-111">d.</span><span class="sxs-lookup"><span data-stu-id="8f02c-111">d.</span></span> <span data-ttu-id="8f02c-112">Impostare **Abilita le impostazioni predefinite per la sicurezza** su **No**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="8f02c-113">e.</span><span class="sxs-lookup"><span data-stu-id="8f02c-113">e.</span></span> <span data-ttu-id="8f02c-114">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-114">Select **Save**.</span></span>

2. <span data-ttu-id="8f02c-115">[Abilitare l'invio del protocollo SMTP del client](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) nella cassetta postale con licenza.</span><span class="sxs-lookup"><span data-stu-id="8f02c-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="8f02c-116">a.</span><span class="sxs-lookup"><span data-stu-id="8f02c-116">a.</span></span> <span data-ttu-id="8f02c-117">Nell'interfaccia di amministrazione di Microsoft 365 passare a **Utenti attivi** e selezionare l’utente.</span><span class="sxs-lookup"><span data-stu-id="8f02c-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="8f02c-118">b.</span><span class="sxs-lookup"><span data-stu-id="8f02c-118">b.</span></span> <span data-ttu-id="8f02c-119">Passare alla scheda Posta e in **App di posta elettronica** selezionare **Gestire le applicazioni di posta elettronica**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="8f02c-120">d.</span><span class="sxs-lookup"><span data-stu-id="8f02c-120">d.</span></span> <span data-ttu-id="8f02c-121">Verificare che l’opzione **SMTP autenticato** sia selezionata (abilitata).</span><span class="sxs-lookup"><span data-stu-id="8f02c-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="8f02c-122">e.</span><span class="sxs-lookup"><span data-stu-id="8f02c-122">e.</span></span> <span data-ttu-id="8f02c-123">Selezionare **Salva modifiche**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="8f02c-124">[Disabilitare l'autenticazione a più fattori (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) nella cassetta postale con licenza.</span><span class="sxs-lookup"><span data-stu-id="8f02c-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="8f02c-125">a.</span><span class="sxs-lookup"><span data-stu-id="8f02c-125">a.</span></span> <span data-ttu-id="8f02c-126">Passare all’interfaccia di amministrazione di Microsoft 365 e, nel riquadro di spostamento sinistro, selezionare **Utenti** > **Utenti attivi**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="8f02c-127">b.</span><span class="sxs-lookup"><span data-stu-id="8f02c-127">b.</span></span> <span data-ttu-id="8f02c-128">Selezionare **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="8f02c-129">c.</span><span class="sxs-lookup"><span data-stu-id="8f02c-129">c.</span></span> <span data-ttu-id="8f02c-130">Selezionare l'utente e disabilitare **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="8f02c-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
